# Reference-Handling Protocol

Working-style rule stated by Anthony 2026-04-27 after v013–v016 shipped without him noticing
that I (Claude) had never actually *looked at* the four reference sites — I only scraped the
text and inferred the design from archetype memory.

> **Rule, in Anthony's words:** "Whenever I give you a website as a reference, always take a
> screenshot and view the code. This way, you have a full understanding of what I'm trying to
> convey."

## What "always" means concretely

When Anthony provides a URL as design or content inspiration — whether it's one URL or a list —
the FIRST tool calls before any creative work are:

1. **Screenshot the page.** Use Chrome MCP: `navigate` → `computer` action `screenshot` (or
   the equivalent screenshot command on whatever browser tool is connected). View the
   screenshot. The image is *the* primary input — palette, typography, layout density,
   photography style, motion cues from how elements are arranged.

2. **View the source HTML/CSS.** Use Chrome MCP `get_page_text` for the rendered text content
   AND `read_page` (or `javascript_tool` to grab `document.documentElement.outerHTML`) for the
   actual markup. Not just text — actual structure, class names, inline styles, web fonts in
   `<link>` tags, image URLs.

3. **Optionally fetch the raw page source** via `mcp__workspace__web_fetch` for the
   pre-rendered HTML if the site is mostly server-rendered. This catches things JavaScript-only
   tools sometimes miss.

This applies to every reference URL, every time. Not "if it seems important" or "if I'm not sure
of the archetype." Always.

## Why

Working from text-only or from archetype memory produces designs that are *plausibly* in the
spirit of the reference but visually disconnected from it. The four design-direction mockups
(v013–v016) shipped with palettes and structural moves that came from my prior knowledge of
"BRIX templates" / "Framer aesthetics" / "ProHauz feel" / "Anderson plumbing vibe" — not from
the actual sites. Some hit closer than others, but the mismatch was real and Anthony spotted
it inside one round of feedback.

The cost of doing this right is small (one extra `screenshot` call per reference, ~5 seconds)
and the cost of skipping it is high (an entire round of redesign).

## What this does NOT mean

- Not "scrape every link on the page." Just the URL Anthony pointed at.
- Not "perfectly replicate." Anthony usually wants inspiration, not a clone — but the
  inspiration must come from actual visual + code evidence, not from an archetype guess.
- Not a license to skip the brief. If Anthony says "different palette per design," palette
  still varies — but the *structural moves* and the *density/feel* should reference what's
  actually on the site.

## Reporting back

After looking at the references and before building, surface what was actually observed in
each: palette (sampled colors), type pairing, image style, layout density, distinguishing
moves. This gives Anthony a chance to correct or redirect before the design work starts.
Pattern to use:

> "Here's what I saw on each reference:
>  - Plumbing X: [observed palette], [observed type], [observed layout]
>  - Plumbly: ...
> Based on that, here's what I'm planning for v0XX: ..."

If I'm describing *vibes* in that report and not *concrete observations*, I haven't actually
looked yet.

## Companion specs

- `text-motion-spec.md` — Anthony's five non-negotiable text-animation rules
- `verified-library-spec.md` — DATA_TAG_MAP image library scheme

All three live in `references/` and should be read before any design pass.
