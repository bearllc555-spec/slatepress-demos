# Text-Motion Spec — Slatepress Demo Sites

Authoritative ruleset for how text moves on every Slatepress-built demo site (plumbers and
beyond). Stated explicitly by Anthony 2026-04-27. **Treat as non-negotiable design DNA, not a
nice-to-have.** If a new design ships without these, it's incomplete.

> "Text effects" in Anthony's vocabulary means **animation**, NOT typography. He has typography
> opinions too but those live elsewhere.

## The five rules

### 1. Word-by-word fade-up on hero headlines

Each word slides up from a clip-mask with stagger. The H1 is split into `.word` spans containing
`.word-inner` spans; the inner translates from `translateY(110%)` to `0` with a `.9s` ease-out
cubic-bezier and a per-word delay of `i * 70ms`. The `.word` parent has `overflow:hidden` so the
clip-mask shows.

### 2. Letter-by-letter reveal on section H2s as they scroll into viewport

Each H2 with class `fx-letters` is split into `.letter` spans. Letters fade in (`opacity 0 → 1`)
and translate up (`translateY(.5em) → 0`) with a per-letter delay of `i * 22ms`, on a `.5s` ease.
Triggered when the H2 enters the viewport via IntersectionObserver, NOT on page load — that
keeps the effect feeling fresh as the user scrolls.

### 3. Scroll-triggered row reveal with stagger on lists, cards, paragraphs

Any element with class `fx-row` and a `data-row-delay="<ms>"` attribute fades up
(`opacity 0 + translateY(20px) → opacity 1 + 0`) when it enters the viewport. The delay is
per-element so a list of six items with delays `[0, 50, 100, 150, 200, 250]` cascades. Use this
on: bulleted lists, service cards, review cards, hours rows, paragraph blocks under H2s.

### 4. Subtle kicker-pulse on small accent dots

Tiny indicator dots (e.g. the green dot before "Open right now · 24 hours") pulse opacity from
`1 → 0.4 → 1` on a `1.4s` infinite loop. Used sparingly — only on live-status indicators, not
decorative dots.

### 5. Restrained, premium feel — not frenetic, not gimmicky

Cumulative tone test: a returning visitor scrolling slowly should feel like the page is *aware
of them*, not *performing for them*. If the page feels like a slideshow or a TikTok edit, you've
overdone it. Cut count, slow timings, drop the most aggressive effect first.

Concretely:
- No bouncy spring physics, no overshoot, no rotate animations
- No parallax beyond very subtle (≤ 4px) scroll-tied transforms
- Don't animate buttons, icons, or trust badges
- Don't reveal the same H2 twice if the user scrolls back up
- Honor `prefers-reduced-motion` — set transform/opacity to neutral and skip transitions

## Reference implementation

The canonical CSS+JS lives in `assets/template.html` (the v011/v012 design migrated to a Mustache
template). When retrofitting an older design or building a new variant, copy these blocks
verbatim:

### CSS block

```css
.fx-words .word{display:inline-block;overflow:hidden;vertical-align:top;padding-bottom:.08em;margin-bottom:-.08em}
.fx-words .word-inner{display:inline-block;transform:translateY(110%);transition:transform .9s cubic-bezier(.215,.61,.355,1);transition-delay:calc(var(--i,0) * 70ms)}
.fx-words.in .word-inner{transform:translateY(0)}
.fx-letters .letter{display:inline-block;opacity:0;transform:translateY(.5em);transition:opacity .5s ease, transform .5s cubic-bezier(.215,.61,.355,1);transition-delay:calc(var(--i,0) * 22ms)}
.fx-letters.in .letter{opacity:1;transform:translateY(0)}
.fx-row{opacity:0;transform:translateY(20px);transition:opacity .8s ease,transform .8s cubic-bezier(.215,.61,.355,1);transition-delay:var(--row-delay,0ms)}
.fx-row.in{opacity:1;transform:none}
.kicker-pulse{animation:kicker-pulse 1.4s ease-in-out infinite}
@keyframes kicker-pulse{0%,100%{opacity:1}50%{opacity:.4}}
@media(prefers-reduced-motion:reduce){
  .fx-words .word-inner,.fx-letters .letter,.fx-row{transition:none;transform:none;opacity:1}
  .kicker-pulse{animation:none}
}
```

### JS block (place at end of `<body>`)

```js
<script>
function splitWords(root){
  const walk=(parent)=>{const out=document.createDocumentFragment();
    for(const node of Array.from(parent.childNodes)){
      if(node.nodeType===Node.TEXT_NODE){const words=node.textContent.split(/(\s+)/);
        for(const w of words){
          if(/^\s+$/.test(w)){out.appendChild(document.createTextNode(w));continue}
          if(w==="")continue;
          const word=document.createElement('span');word.className='word';
          word.style.setProperty('--i',root._wordIdx++);
          const inner=document.createElement('span');inner.className='word-inner';inner.textContent=w;
          word.appendChild(inner);out.appendChild(word);
        }
      } else if(node.nodeType===Node.ELEMENT_NODE){
        const clone=node.cloneNode(false);clone.appendChild(walk(node));out.appendChild(clone);
      }
    }
    return out;
  };
  root._wordIdx=0;const replaced=walk(root);root.innerHTML='';root.appendChild(replaced);
}
function splitLetters(root){
  const text=root.textContent;root.textContent='';let i=0;
  for(const ch of text){
    if(ch===' '){root.appendChild(document.createTextNode(' '));continue}
    const span=document.createElement('span');span.className='letter';
    span.style.setProperty('--i',i++);span.textContent=ch;root.appendChild(span);
  }
}
document.querySelectorAll('.fx-words').forEach(splitWords);
document.querySelectorAll('.fx-letters').forEach(splitLetters);
document.querySelectorAll('.fx-row').forEach(el=>{
  const d=el.getAttribute('data-row-delay');if(d)el.style.setProperty('--row-delay',d+'ms');
});
const io=new IntersectionObserver((entries)=>{
  entries.forEach(e=>{if(e.isIntersecting){e.target.classList.add('in');io.unobserve(e.target);}});
},{threshold:0.15,rootMargin:'0px 0px -10% 0px'});
document.querySelectorAll('.fx-words, .fx-letters, .fx-row').forEach(el=>io.observe(el));
</script>
```

## Where to apply each class

| Element | Class |
|---|---|
| Hero H1 | `fx-words` |
| Section H2 | `fx-letters` |
| Hero lede paragraph | `fx-row` with `data-row-delay="500"` |
| Each service card | `fx-row` with cascading delays (`0, 80, 160, 240, 320, 400`) |
| Each review card | `fx-row` with `data-row-delay="0"` and `"180"` |
| Service-area list items | `fx-row` with `0, 50, 100, 150, 200, 250` |
| Hours list items | `fx-row` with `0, 40, 80, 120, 160, 200, 240` |
| Trust-badge row | `fx-row` with `data-row-delay="400"` |
| Live-status accent dot | `kicker-pulse` |

## What this spec does NOT cover

- Typography choices (font families, sizes, weights, leading) — separate concern
- Color palette — varies per design direction
- Photography or illustration style — varies per design direction
- Page-load animations beyond the initial hero (we don't do those)
- Hover micro-interactions on buttons (those are per-design choices)

## Why this is written down

The first four "design direction" mockups (de-vito-plumbing v013–v016) shipped without any of
these effects because the brief said "different palettes, different overall designs" and motion
wasn't named explicitly. Anthony noticed immediately. This spec exists so a future session can
read it during any design pass and not make the same omission. Reference it from the
plumbing-site-generator skill's SKILL.md and from the blog skill if/when a refresh of those
designs touches motion.
