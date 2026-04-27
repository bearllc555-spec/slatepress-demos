# Plumbing Design References — Four-Reference DNA

The four sites Anthony has filed as the design DNA for plumbing demos. Stated 2026-04-27.
Each site is the *anchor* for a specific quality we want: visual ceiling, information
architecture, conversion density, human warmth.

**Important precedent:** the first time these references were used to build De Vito v013–v016,
I (Claude) only scraped the page text and inferred design from archetype memory. The result:
all four mockups were wrong on palette, with v016 being a complete miss. This document captures
what I actually observed when I screenshot + viewed source for each reference. **It is the
authoritative read** — when palette/type/move questions come up in a future session, read this
before guessing.

---

## 1. Visual ceiling — Plumbing X (BRIX / Webflow Marketplace)

**URL:** https://plumbingtemplate-showcase.webflow.io/home

**What I actually saw:**
- **Palette:** white background, single high-saturation royal-blue accent (looks like ~#3F4DFF
  / Pantone reflex blue). Bright. No dark mode, no gradients, no gold.
- **Type:** bold heavy-weight sans-serif display ("Best plumbing & repair solutions" — almost
  black weight, very wide tracking on small caps eyebrow "PLUMBERS").
- **Photography:** large high-quality residential portraits — a smiling worker in a blue hard
  hat under a kitchen faucet fills the right half of the hero. Not stock-feeling, the lighting
  is studio-bright but believable.
- **Layout:** clean utility bar at top (email + phone + address + social row). Centered nav
  with cart counter (it's actually a Webflow *ecommerce* template, hence the cart). One big
  blue CTA button "Get a quote" pill-rounded-rectangle. Hero is a 50/50 split, text-left
  photo-right, with massive type taking the height.
- **Distinguishing moves:**
  - The blue is *one* accent. It carries everything — the logo, the eyebrow, the CTA. No
    secondary accents.
  - Eyebrow text is small, all-caps, blue, with letter-spacing.
  - Drop logo is a stylized blue water-drop icon.
  - Heavy display type doing all the heavy lifting (no tagline, no kicker beyond the blue
    eyebrow).

**The transferable lesson:** "visual ceiling" here doesn't mean dark/luxe/magazine. It means
**a single confident accent + heavy display type + great photography**. Restraint, not
maximalism. Less is more.

**Where v013 went wrong:** I shipped dark navy + electric cyan + gold + serif display ("magazine
luxury" archetype). That's a different visual ceiling — closer to a SaaS landing page than to
this template. The actual Plumbing X target is *bright minimal-ish corporate*, not *dark
editorial*.

---

## 2. Information architecture — Plumbly (Framer)

**URL:** https://plumbly.framer.website/

**What I actually saw:**
- **Palette:** vivid royal-blue (~#1A66E5) hero color block + white sections + black type +
  yellow accent (used for the "Get 50% OFF All Access" template-marketplace promo button — that
  yellow is *probably* not part of the real plumbing brand, it's the Framer template hawking
  sticky). Real brand palette = vivid blue + white + black.
- **Type:** very bold geometric sans-serif headlines, near-black weight, on light backgrounds.
  Body text appears to be a clean modern grotesque (Inter or similar).
- **Photography:** real-feeling tradesperson portrait — a graying plumber in white tee + blue
  overalls + tool belt, kneeling next to an under-sink repair. Filling the right half of hero.
- **Layout:** asymmetric split-hero — solid blue color block left half, photo right half, with
  organic lighter-blue *wave* shapes on the blue side as decoration. White nav floating top of
  the blue. Pill-pill-pill nav links + black "Book a Free Consultation" pill button.
- **Distinguishing moves:**
  - Wave/blob shapes in pale-blue on the dark-blue hero — adds movement without animation.
  - Round-avatar trust stack: "10,500+ Individuals who trusted Plumbly" with three overlapping
    customer-portrait circles.
  - Below-fold trust trio: three icon-circles ("By Satisfied Customers," "Transparent
    pricing," "24/7 Support"), each a blue circle with a white icon, paired with a bold black
    h3 + 3-line description. **Strong pattern worth lifting.**
  - "Why Choose Our Plumbing Team" — section eyebrow + bold black 2-line headline. Clean IA
    sequence: rating-chip → hero → trust-trio → why-choose-us → services → about → team →
    testimonials → process → gallery → FAQ → contact form.

**The transferable lesson:** Plumbly's gift is *page sequence and section rhythm*. You always
know where you are in the page; sections breathe; trust signals are placed where decisions get
made. **Lift the structure, not the palette** — though the vivid blue + black + white triad
does work.

**Where v014 went wrong:** I shipped pastel cream + sage + peach + sky-blue ("soft Framer
pastel lifestyle" archetype). The actual Plumbly is *vivid, saturated, confident* — not
pastel. The IA was right (3-pillar trust trio, process band, etc.) but the palette was a
miss in the wrong direction.

---

## 3. Feature density / conversion — ProHauz (BoldThemes WordPress)

**URL:** https://prohauz.bold-themes.com/plumbing/

**What I actually saw:**
- **Palette:** dark corporate navy-to-mid-blue gradient hero + white content sections + RED
  CTA ("Request Job Estimate" button is solid red, partially hidden behind the popup ad in my
  screenshot but visible). Bright cyan-blue accent for the noun in headlines ("The **Plumber**
  You Deserve"). Black/dark-grey body type. NOT orange, NOT industrial.
- **Type:** bold heavy sans-serif headlines with the keyword in bright cyan-blue. Service
  blocks use **ALL-CAPS uppercase** service names ("TOILET LEAKING," "OVERFLOWING TOILET")
  paired with small line-art icons.
- **Photography:** confident smiling bearded plumber in blue overalls right-side of hero,
  blurred plumbing-tools photo behind. Below: 3-up grid of action shots (different plumbers
  doing different repairs).
- **Layout:** thin nav bar with **slash separators** between links ("HOME / ABOUT / BLOG /
  SHOP / ELEMENTS"). Logo + brand on far left, phone number and BOOK SERVICE CTA on far right.
  Hero with overlay text + photo. Then 3-photo grid. Then service blocks.
- **Distinguishing moves:**
  - **Isometric grayscale illustrations** of houses/rooms used in technical sections (huge,
    fills half a column). Distinctive — not photographic, not flat-line, not full-color.
  - Plus-mark grid pattern (`+ + + +`) decorative texture in side margins.
  - All-caps service names with small icons — packed list of common problems
    ("LEAKY FAUCET", "BURST PIPE", "OVERFLOWING TOILET") rather than "categories."
  - Slash separators in nav — a typographic detail that reads "industrial trade."

**The transferable lesson:** density doesn't have to mean orange/loud. ProHauz is *confident
corporate blue* with red/cyan punctuation, but it packs *more* into the page than the others —
the isometric illustrations, the plus-mark grid, the all-caps service list, the marketing
banners. Conversion density = "every section sells something specific."

**Where v015 went wrong:** I shipped orange + black + cream + Barlow-Condensed ("trade
contractor with marketing budget" archetype). The actual ProHauz is **blue/red corporate**.
The conversion-density structural moves I added (offers strip, from-pricing, guarantees band)
are right; the palette is wrong.

---

## 4. Human warmth / social proof — Anderson Plumbing, Heating & Air (real local site)

**URL:** https://www.andersonplumbingheatingandair.com/

**What I actually saw:**
- **Palette:** **hot magenta/pink** (~#D9176F territory) + black + white as primary palette.
  Yellow gold accent for the rating circle. Subtle pink decorative shapes and divider lines.
  This is the biggest surprise — I expected patriotic red/white/blue and got bold
  pink/black/white instead.
- **Type:** bold black **italic** display headlines ("Nobody wows clients like we do!®") with
  a registered trademark mark — italic, very bold, almost editorial-condensed. Black sans nav.
  Pink eyebrow text for "Serving the Greater San Diego Area Since 1978."
- **Photography:** **their actual fleet van** as the hero — bright-pink-painted Anderson
  Plumbing Ford Transit electric, with their stylized rose-flower logo on the side, parked in
  front of a desaturated San Diego skyline. This is the killer move: not stock, not generic,
  *the actual identifying brand element*.
- **Layout:** thin top utility bar (current promo banner left + AMP-Member / About / Resources
  / Careers / Contact / search right). Below: classic three-column header (logo center-left
  with vintage-stamp framing + "Since 1978" + "PLUMBING HEATING & AIR" stacked, star-rating
  next, then "24/7 Emergency Support" + phone + pink "Schedule Online" pill on the right).
  Then a black mega-nav with 8 service categories (Plumbing, Sewer & Drain, Water Quality,
  Heating, Air Conditioning, HVAC, Indoor Air Quality, Commercial), each with a dropdown
  caret. Hero below: italic black headline left + van photo right + yellow circular 4.8-rating
  badge top-right.
- **Distinguishing moves:**
  - **Vintage-stamp logo treatment** — "Since 1978" above, "ANDERSON" in a bordered black box,
    "PLUMBING HEATING & AIR" below. Reads heritage without being old-fashioned.
  - **Their painted fleet van as hero photography** — high-impact and impossible for
    competitors to copy.
  - **Registered trademark on the tagline** ("Nobody wows clients like we do!®") — claims the
    phrase as IP. Confident.
  - **8-category mega-nav** — Anderson sells WAY more services than a single-trade plumber.
    For De Vito (single trade, residential), this is too many; **lift the dropdown structure
    but not the count**.
  - **Yellow circular rating badge with gold stars + "out of 4,462 reviews"** — concrete
    review count is the trust hook, not a vague "trusted by thousands."
  - **Promo banner** at top ("Beat the Heat - Summer's arrived early! Schedule a tune-up
    now!") — running marketing fed straight into the chrome.
  - **Pill-shaped CTAs with leading icons** (calendar for Schedule, phone for Call) — soft
    pink, generous padding, white text.

**The transferable lesson:** "human warmth" here doesn't mean American-flag-patriotic. It means
**a brand that owns its identity**: their own van, their own tagline (with ®), their own
44-year history written into the logo, their own pink color choice that's not in the
typical-trade-service playbook. Warmth is *specificity*, not template-traditional.

**Where v016 went wrong:** I shipped patriotic navy + red + gold + cream + serif (Source Serif
4) + family-multi-generation lore + "AMP-style membership block." Those structural moves are
fine — but I projected "American heritage trade business" onto a brand that's actually doing
something far more distinctive. Real Anderson would never use navy/red/gold; they're confident
enough to own pink.

---

## How to use this document

**Before any future De Vito design pass** (or any plumbing design pass):

1. Read this file first.
2. If a new reference is added, navigate to it, screenshot it, view source, and append a new
   entry here following the same structure (palette, type, photography, layout, distinguishing
   moves, transferable lesson, where prior attempts went wrong).
3. When picking a palette for the new design, sample directly from the screenshots in this
   doc (or re-screenshot if you're worried the source has changed). **Do not invent palettes
   from archetype memory.**
4. When proposing a design direction, *cite this document*: "v0XX takes the
   single-confident-blue-accent move from Plumbing X plus the trust-trio structure from
   Plumbly's IA." If you can't cite it, you're guessing.

## Companion specs in this folder

- [text-motion-spec.md](./text-motion-spec.md) — five non-negotiable text-animation rules
- [reference-handling-protocol.md](./reference-handling-protocol.md) — always-screenshot rule
- [verified-library-spec.md](./verified-library-spec.md) — image library scheme
