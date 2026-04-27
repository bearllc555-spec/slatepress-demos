# Slatepress Plumbing Design System — v1.0

*Locked 2026-04-27 by Anthony and Claude. Single canonical reference for every plumbing demo Slatepress builds. Future rule additions become v1.1, v1.2, etc., with a changelog at the bottom of this file.*

---

## 0. What this is

This document is the **single source of truth** for how Slatepress builds plumbing websites. Every demo (De Vito v017+, future plumber prospects, eventual self-service-app output) MUST conform to v1.0. The thesis, the references doc, the text-motion-spec, and the reference-handling-protocol are all companion docs that supply detail. **This file is the definitive index. Read it first.**

## 1. What's locked vs what flexes per customer

**Locked across every plumbing demo** — break any of these and the design is non-conforming:

- The 15 structural rules (§ 3)
- The hero-photo category-coding rule (§ 4)
- The text-motion engine and its 5 timing/easing values (§ 5)
- The reference-handling protocol when given new design URLs (§ 6)
- The required sections inventory (§ 8)
- The pricing/specificity conventions (§ 9)

**Flexes per customer or per design direction** — pick freely within the constraints above:

- **Brand color** — one saturated hue. White carries the breathing room. Black or deep navy for emphasis sections. (See § 3.1)
- **Type family** — one bold sans-serif. Outfit, Plus Jakarta Sans, Inter, geometric grotesques all qualify. No serifs, no scripts. Italic is allowed for display only.
- **Hero structure** — 50/50 text-left photo-right is the default per the 15 rules; split-blue-block-hero (Plumbly DNA) and dark-gradient-hero (ProHauz DNA) are also conforming. Pick what fits.
- **Decorative motif** — every brand needs one signature graphic mark. Plus-grid, wave shapes, magenta wedges, `+`-sign stat highlights — pick one and let it recur.
- **Layout/section order** — the 11 required sections (§ 8) can reorder slightly to fit each customer's emphasis, but all 11 must appear.
- **Photography** — within the category-coding rule, pick the specific shots. v017 used a plumber in blue overalls, v020 used a plumber-by-van. Both qualify.

The four-reference DNA (§ 7) is the **starting palette** — pick which DNA leads your design (visual ceiling / IA / conversion / warmth) before you start specializing.

## 2. The two questions every visitor's gut asks

Before any rule, the underlying premise. Plumbing-website conversion is a **30-second triage event**. The visitor is in mild-to-acute stress (kitchen flooding, water heater dead, toilet overflowing). They scroll fast. They want to know:

1. **What kind of business is this?** (plumbing — answered by photo before language)
2. **Who's doing the work?** (a plumber, or my plumber's truck pulling up to my house)

Every rule in v1.0 exists to compress the time between those two questions and the phone call. If a move helps, it's in. If not, it's out.

## 3. The 15 structural rules (the floor)

Every plumbing demo MUST hit all 15. Cite them by number when reviewing.

### 3.1 — One brand color, used confidently
Pick a single saturated hue. Show it on logo, eyebrow, icon-pills, primary CTA, stat callouts, footer accent. White carries breathing room. Black or deep navy for contrast text and one emphasis section. Pastels and three-color compromises are forbidden.

### 3.2 — Bold sans-serif typography, single family
Heavy display weight (700–800), no serifs, no scripts, no italic flourishes (italic display is allowed but rare). Body text in a softer neutral than pure black so headlines feel calm-confident, not shouty. Reference: `#6E7891` slate, not `#000`.

### 3.3 — 50/50 hero with one dominant image
Text on the left, one big image on the right. Eyebrow → display H1 with one keyword highlighted in brand color → 40-60 word lede → primary CTA + phone CTA + ★ rating with review count. Above-the-fold conversion stack complete.

### 3.4 — Phone is a primary CTA in three places
Top utility bar AND in the hero AND in the footer. Pill button or large numerical display, brand-colored. The phone closes the deal.

### 3.5 — Trust trio or 4-up benefits row early in the page
3–4 short value props with thin-stroke line-icons in brand color, bold heading, 2–3 line description.

### 3.6 — Big-number stats somewhere on the page
Concrete numbers at 60–100px+ display weight: years in business, jobs done, response time, review count. Vague "trusted by thousands" never beats a specific number.

### 3.7 — Section background shifts for rhythm
Alternate white with one or two emphasis backgrounds (deep navy, brand-color band, black, yellow band). Each section reads as a chapter, not a scroll.

### 3.8 — Soft-rounded CTAs in brand color
Pill or 10px-radius rectangle. Generous padding. Brand-colored fill, white text. Calendar or phone icon optional.

### 3.9 — Concrete social proof with platform attribution
Star rating + review count + actual Google or Yelp logo. Real third-party award logos where applicable. Avoid generic "loved by neighbors."

### 3.10 — Service area shown as a graphic
Either a Google Map with pinned coverage or a clean town list with pin icons. Visual proof of "we cover this area."

### 3.11 — Membership or guarantee block
An explicit ongoing-relationship offer (annual maintenance plan, 100% satisfaction guarantee, etc.) — not just a one-time service pitch.

### 3.12 — Service cards with real action photography
Real photo of the work + small overlay icon in brand color + bold service name + 1–2 line description + "Read more" or "Schedule" link.

### 3.13 — Repeat hero CTA in the footer
Phone + Schedule pill + tagline + 24/7 promise. Catch the bottom-of-page reader.

### 3.14 — One signature decorative motif that recurs
Pick a graphic mark and let it recur — pink wedges, plus-grid, wave shapes, isometric houses, `+`-sign stat highlights. Each brand needs a fingerprint without being distracting.

### 3.15 — Stylized line-iconography everywhere
Water drops, wrenches, faucets, drains, certificates, trucks, calendars, dollar signs, clocks. Always thin-stroke line, always brand-colored, often inside circular pills.

## 4. The category-coding test (image rule)

**The hero photo MUST show one of two things:**

1. **A full plumber.** Face/body visible, with plumbing tools or in branded uniform or actively working on plumbing fixtures.
2. **A branded fleet vehicle.** Van or truck with plumbing company wrap, logo, or branded panels visible.

**Bonus combo (strongest possible hero):** a plumber standing next to their fleet vehicle. Stacks both signals.

**The diagnostic test:** a returning visitor who can't read English should still know what kind of business this is from the hero photo alone. If they could mistake it for cleaning, HVAC, hardware, kitchen remodel, real estate, or landscaping — the photo is wrong, no matter how nice it looks.

**Forbidden as hero photos**, even when plumbing-coded:
- Hands-only shots (gloved hands wrapping a wrench, hands on a boiler control panel)
- Bare fixtures (pristine chrome faucet, clean bathroom, stainless sink)
- Tools alone (pipe wrench on a wood floor, tools on a bench)
- Decorative cutaways or illustrations

**Why:** plumbing-coded content alone isn't enough. The hero has to answer both visitor questions simultaneously: (a) plumbing and (b) who's doing it. Bare fixtures answer (a) but not (b).

**The four references prove the rule:** Plumbing X / Plumbly / ProHauz all show full plumbers (3/4). Anderson shows the painted-pink fleet van (1/4). None use bare fixtures or hands-only shots.

Apply the test on every candidate before committing. **Visit the URL in a browser, look at the actual image** — don't trust HEAD-checks or alt text alone. (See § 6.)

## 5. The text-motion engine

Every plumbing demo MUST include the text-motion engine, with the **IO + setTimeout fallback + scroll fallback + 2.5s hard-reveal** pattern. The pure-IO version is forbidden — it silently fails in some browsers and leaves content invisible. Full canonical CSS+JS lives in `text-motion-spec.md`. Five rules:

1. **Word-by-word fade-up on hero H1** — clip-mask `translateY(110%) → 0` with `i * 70ms` per-word stagger.
2. **Letter-by-letter reveal on section H2s** — `opacity 0 + translateY(.5em) → 0` with `i * 22ms` per-letter stagger, viewport-triggered.
3. **Scroll-triggered row reveal with stagger** — `.fx-row` + `data-row-delay`, `opacity 0 + translateY(20px) → 0`. Apply to lists, cards, paragraphs, list items, hours rows.
4. **Subtle kicker-pulse on live-status accent dots** — opacity `1 → 0.4 → 1` on a 1.4s loop. Only on live-status indicators.
5. **Restrained, premium feel** — no bouncy spring physics, no overshoot, no rotate animations, no parallax > 4px, no animation on buttons/icons/badges, honor `prefers-reduced-motion`.

The engine has four execution paths in v1.0:
- IntersectionObserver (preferred)
- 700ms `setTimeout` fallback for elements in viewport that IO missed
- Scroll handler for elements coming into view
- 2.5s hard guarantee that reveals everything regardless of viewport

## 6. The reference-handling protocol

When given any URL as design inspiration, the FIRST tool calls before any creative work:

1. **Screenshot the page** (Chrome MCP `navigate` + `computer screenshot`). View the image.
2. **View the source** (Chrome MCP `read_page` or `javascript_tool` reading `document.documentElement.outerHTML` or `mcp__workspace__web_fetch`). View the markup.
3. **Report back observations** — palette (sampled), type pairing, image style, layout density, distinguishing moves — *before* building.

If you describe vibes ("premium dark luxe") instead of citing concrete observations ("bg `rgb(255,255,255)`, accent `#3083FF`, Outfit at 68px/700"), you haven't actually looked. The rule was stated 2026-04-27 after v013–v016 shipped using archetype memory instead of observation. Full ruleset in `reference-handling-protocol.md`.

## 7. The four-reference DNA index

Pick which DNA leads your design before you start specializing. Each is anchored to one observed reference site.

| Ref ID | Site | DNA | When to lead with it |
|---|---|---|---|
| **Ref 001** | Plumbing X (BRIX) | Visual ceiling | When the customer wants premium, restrained, magazine-feel |
| _unassigned_ | Plumbly (Framer) | Information architecture | When the customer has lots of services and needs clear page sequence + section rhythm |
| _unassigned_ | ProHauz (BoldThemes) | Feature density / conversion | When the customer wants offers, FAQs, embedded video, awards strip — packed for conversion |
| _unassigned_ | Anderson Plumbing | Human warmth / social proof | When the customer has real fleet/team specifics that beat any template (fleet van, named techs, Since-YYYY heritage) |

Full per-reference deep-pass observations (palette, type, layout, distinguishing moves) live in `plumbing-design-references.md`. Future Refs (002, 003, 004) get assigned by Anthony with a deep-pass.

## 8. Required sections inventory

Every plumbing demo MUST contain all 11 sections in roughly this order. Order can adjust slightly to fit each customer; presence is non-negotiable.

1. **Top utility bar** — open-now status, address, phone, social icons.
2. **Sticky main nav** — logo, nav links, primary CTA pill on the right.
3. **Hero** — eyebrow, display H1, lede, button row, ★ rating chip, dominant photo (per § 4).
4. **Trust trio or 4-up benefits row** — 3–4 short value props with line-icons (per § 3.5).
5. **Services grid or slider** — 3 or 6 cards with real action photography + line-icon overlay + name + 1-2 line description (per § 3.12).
6. **About / "Why us"** — anchored by a person photo + stat block + tagline. Two generations / since-year framing welcome.
7. **Big-number stats** — 4-up or 3-up at 60–100px+ display weight (per § 3.6).
8. **Special offers / current promotions** — 3 or 4 offer cards with $ amounts + brand-colored CTAs (per § 9 for pricing).
9. **Reviews / social proof** — carousel or grid of Google/Yelp reviews with platform attribution (per § 3.9).
10. **Service area + hours** — graphic map or list + open-24-7 weekly grid (per § 3.10).
11. **Final CTA + footer** — repeat phone + Schedule pill + tagline (per § 3.13), then footer with address, phone, hours, services links, locations, and "Site by Slatepress" credit.

Optional but encouraged: a membership/maintenance-plan block (per § 3.11) lives between sections 6 and 7 or between 8 and 9.

## 9. Pricing and specificity conventions

**Pricing on offers and services.** Demo sites can include illustrative prices ($49 tune-up, $500 off water heater, "from $129" service tiers) IF the page footer includes a small italic disclaimer:

> *Pricing illustrative. Final pricing confirmed in your written estimate before any work begins. Demo by Slatepress.*

When the customer signs and provides real pricing, the disclaimer comes out and the prices update. This is non-negotiable — never ship a demo without the disclaimer if any prices are placeholder.

**Specificity slots.** Every demo has spots where real-customer assets should slot in (real fleet van photo, real technician portraits, real review count from Google API, real awards). Mark these with HTML comments:

```html
<!-- [SPEC: replace with real photo of De Vito work van] -->
<div class="hero-visual" style="background-image:url('https://images.pexels.com/photos/13821194/...')"></div>
```

The Pexels stock is a stand-in. The `[SPEC: ...]` comment tells the next session what to swap. When the customer provides real assets, do a search-replace on `[SPEC]` markers and ship the upgraded version.

## 10. Versioning policy

This document is **v1.0 as of 2026-04-27**. Future changes:

- **v1.1, v1.2, etc.** — additive changes (new rule, new convention, additional reference DNA). Append to relevant section, update the changelog, bump the version.
- **v2.0** — breaking changes (rule overturned, new structural section required). Discuss with Anthony first.
- **The four companion docs** (thesis, references, motion-spec, protocol) stay as living docs. When they change in a way that affects v1.0, bump v1.0 accordingly.

**Changelog**

- **v1.0 (2026-04-27)** — initial lock-down. Consolidates the 15-rule ruleset (stated mid-day after v013–v016 shipped wrong on palette), the photo category-coding rule (stated after v017's gloved-hand-on-chrome read as maid service), the tightened photo rule (full plumber OR fleet vehicle, after v019/v020 first-pass shipped with hands-only and faucet-alone), the text-motion engine with IO+fallback (after the original IO-only engine silently failed across all of v013–v020), the reference-handling protocol (after v013–v016 shipped from archetype memory), the four-reference DNA index, the required sections inventory, the pricing/specificity conventions, and the four deployed demos as worked examples (v017–v020).

## 11. Companion documents

| Doc | What it has that v1.0 doesn't |
|---|---|
| [plumbing-website-design-thesis.md](./plumbing-website-design-thesis.md) | The strategic argument behind every rule — why crisis-decision design, why specificity is the wedge, why image grammar is the differentiator. Read for the "why." |
| [plumbing-design-references.md](./plumbing-design-references.md) | Per-site deep-pass observations on Plumbing X, Plumbly, ProHauz, Anderson — palette hex codes, type families, distinguishing moves, where prior De Vito mockups went wrong. Read when picking which DNA to lift. |
| [text-motion-spec.md](./text-motion-spec.md) | The canonical CSS+JS for the motion engine. Copy-paste source. |
| [reference-handling-protocol.md](./reference-handling-protocol.md) | The always-screenshot-and-view-source rule with the exact tool calls. Read when handed a new reference URL. |

## 12. The starter scaffold

The locked v1.0 starter HTML scaffold lives at:

`outputs/plumbing-site-generator/assets/scaffold-v1.html`

It bakes in:
- Single brand-color CSS variable (`--brand`) — change one line to recolor the whole site
- Inter as the default type family
- The IO+fallback motion engine
- All 11 required sections in the default order
- Mustache placeholders for content (`{{BUSINESS_NAME}}`, `{{PHONE_TEL}}`, `{{TOWN}}`, etc.)
- `[SPEC: ...]` comments at every photo slot
- Pricing-illustrative disclaimer in the footer
- Default photo URLs that pass the category-coding test (plumber portraits + fleet-van shot)

To start a new design direction:
1. Copy `scaffold-v1.html` to `customers/<slug>/dist/v0XX.html`
2. Set the `--brand` CSS variable to the target color
3. Pick one font family (Outfit / Plus Jakarta Sans / Inter / etc.) — change one `<link>` and one `font-family`
4. Add the customer's signature decorative motif (wedges, plus-grid, waves, etc.)
5. Fill in the Mustache placeholders from the customer's brand.json
6. Pick photo IDs from the verified library that pass the category test (per § 4 — visit each candidate URL before committing)
7. Apply the can't-read-English diagnostic on every hero photo before shipping

The scaffold is the floor. Specialize on top of it.

---

*v1.0 locked 2026-04-27. Anthony Slatepress + Claude.*
