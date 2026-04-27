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

## Reference index

Anthony assigns short Ref IDs as we go. Use these in conversation when picking which DNA to
apply ("v0XX takes Ref 001's hero pattern + Ref 002's IA").

| Ref ID | Site | DNA tag | Status |
|---|---|---|---|
| **Ref 001** | Plumbing X (BRIX / Webflow) | Visual ceiling | Documented (deep pass 2026-04-27) |
| _unassigned_ | Plumbly (Framer) | Information architecture | Documented (light pass 2026-04-27) |
| _unassigned_ | ProHauz (BoldThemes WP) | Feature density / conversion | Documented (light pass 2026-04-27) |
| _unassigned_ | Anderson Plumbing | Human warmth / social proof | Documented (light pass 2026-04-27) |

---

## Ref 001 — Visual ceiling — Plumbing X (BRIX / Webflow Marketplace)

**URL:** https://plumbingtemplate-showcase.webflow.io/home
**Last verified:** 2026-04-27 (screenshots + source extracted via Chrome MCP)

### Observed palette (from computed styles)

- **Page background:** `#FFFFFF` white — primary canvas
- **Accent / CTA / links:** `#3083FF` royal-blue (rgb 48, 131, 255). Used for Get-a-quote
  button, "PLUMBERS" eyebrow, water-drop logo, email/phone/location utility-bar icons in pale
  pill backgrounds, and slider-arrow circles.
- **Display headline color:** `#182944` deep navy (rgb 24, 41, 68). H1 + H2 text on light
  sections.
- **Body text:** `#6E7891` soft slate-gray (rgb 110, 120, 145) — NOT pure black. Body copy is
  noticeably softer than headlines, which gives the page a calm-confident feel.
- **Dark section background:** `#182944` same deep navy (sections used for "About — We focus
  on customer satisfaction and quality" and "Our work" — used for emphasis blocks, not the
  whole page).
- **Yellow micro-accents:** amber/yellow (~#F5A523 territory) on stat `+` signs (alternating
  with blue) and the "OUR WORK" eyebrow against dark navy. Easy to miss but it's a real third
  hue.
- **Pale-blue tint:** light sky-blue (~#E1ECFF territory) used for circular icon-pill
  backgrounds in service cards and the "Visit our office" trio.

So the palette is **not** "single accent" as I first wrote — it's actually **white +
royal-blue + deep navy + soft slate + amber + pale sky-tint**, with the dark navy used as
an alternating-section background for emphasis.

### Observed typography (from computed styles)

- **Family:** `Outfit, sans-serif` — modern geometric sans, used for body AND display. Single
  family throughout.
- **H1:** 68px, weight 700 (bold), color #182944 deep navy. Letter-spacing tight.
- **Eyebrows:** small all-caps, blue or yellow depending on background, with wide tracking.
- **Body copy:** ~17–18px, weight 400, color #6E7891 slate.
- **No serif anywhere.** No display alternate, no italic, no condensed.

### Observed CTA shape

- **Primary button:** background #3083FF royal-blue, white text, **border-radius 10px**
  (soft rectangle, NOT a pill, NOT square), padding 26px 38px (very generous — buttons feel
  big and tappable).
- **Secondary button:** transparent fill, royal-blue text, royal-blue 1px stroke, same
  border-radius and padding. Sits next to primary as a row.

### Observed photography

One large hero portrait spanning the full right column:
- Worker in a bright royal-blue hard hat (matching the palette) at top
- Continues down through chest with arms crossed, blue work overalls, mustard-yellow gloves
- Composed against a real kitchen with a curly chrome flexible faucet/sprayer arm and white
  cabinetry
- Lighting is studio-bright but believable — feels professional, not over-glossy stock

In the **About** section (dark navy bg): bearded man, white hard hat, navy work jacket, giving
a thumbs-up directly to camera. Mid-40s, friendly, real-feeling.

In the **Services 3-card slider**:
- Card 1 — chrome wall-tap with bright blue PEX pipe leading in, against textured concrete-gray
- Card 2 — two hands on a chrome pipe wrench at a P-trap/supply-line, white sink edge visible
- Card 3 — top-down white sink with chrome faucet, hand in royal-blue glove around drain hole

Each card photo sits above a circular icon-pill (faucet / crossed-tools / drain) in pale-blue.

In the **Our Work** section (dark navy bg): video thumbnail with a circular white play-button
+ blue play triangle. Thumbnail shows a white-hard-hat worker gesturing while holding a
clipboard. Implies an embedded YouTube/Vimeo intro video.

**Photography style overall:** real-feeling stock or commissioned shoots. Bright studio
lighting, mid-shallow depth of field, slightly warmer-than-neutral white balance. People
center-frame, looking at camera or absorbed in work — never staged-corporate-fake.

### Observed iconography

- **Logo mark:** stylized royal-blue water-drop SVG, paired with bold dark-navy "Plumbing X"
  wordmark.
- **Utility bar icons:** small line-icons (envelope, phone, location-pin) in pale-blue
  circular backgrounds. Plus a row of social icons (Facebook, Twitter, Instagram, Yelp, Google)
  in dark-gray on the right.
- **Service-card icons:** royal-blue line-art (faucet, crossed-tools, drain) on pale-blue
  circular pills.
- **Slider controls:** royal-blue circular buttons with white arrow icons, sitting outside the
  card row.

### Observed layout / structure

- **Top utility bar** (white): contact email · phone · address · social icons. Subtle, sits
  above the main nav.
- **Main nav** (white, sticky-feeling): logo left, centered nav links (Home / About /
  Services / Pages dropdown / Cart counter), royal-blue "Get a quote" CTA right.
- **Hero**: 50/50 split, text left + photo right. Eyebrow + 68px H1 + lede paragraph + two-
  button row. Photo is full-bleed-into-rounded-frame on the right.
- **About section** (dark navy): same 50/50 split, photo left (thumbs-up plumber) + text
  right with stat trio (25+ Years / 500+ Happy clients / 20+ Qualified experts) + "Get a
  quote" CTA.
- **Services slider** (white): 3-up card carousel with prev/next arrow controls. Each card is
  photo + circular icon-pill + bold dark-navy title + 2-line lorem body.
- **"Our work" section** (dark navy): 50/50 split, text left + video thumbnail right with
  play overlay.
- **Subsequent sections (not screenshot this pass):** "Having a problem? We'll fixed it
  today!", "What our clients say" (testimonials), "Check our lastest articles" (blog cards).
  H2 count = 6 total. Source confirms these exist; I haven't visually inspected them yet.
- **Webflow promo strip** at the bottom of every screenshot (purple "Like Plumbing X
  Webflow Template? Buy Now") and the "Made in Webflow" badge are the marketplace preview
  wrapper, NOT part of the design. Ignore.

### Source observations

- **HTML:** ~109 KB total, 264 unique CSS classes (Webflow-heavy, includes ecommerce cart
  classes since this is technically a Webflow Ecommerce template).
- **Stylesheet:** single hashed Webflow CSS file.
- **Class taxonomy worth knowing:** `btn-primary` / `btn-secondary` / `btn-circle-primary` /
  `btn-circle-secondary`, `badge-primary`, `bg-neutral-800` (the dark-navy section bg),
  `card-testimonial-v1`, `blog-card-*`. Suggests they think of buttons in primary/secondary
  pairs and have a neutral-darkest token at the 800 weight.

### Distinguishing moves (what makes this site recognizable)

1. **Two-tone alternating sections** — white hero, navy emphasis section, white services,
   navy "Our work." Repeats. This breaks the page into chapters without dividers.
2. **Single typeface (Outfit) for everything** — display *and* body. Simplifies the type
   system and gives the page a uniform geometric voice.
3. **Soft-rectangle buttons** (10px radius, generous padding) — not pill, not square. Feels
   modern but not trendy.
4. **Stat trio with `+` signs** (25+ / 500+ / 20+) where the `+` alternates yellow / blue /
   yellow — small graphic treatment that adds personality without busying the page.
5. **Pale-blue icon pills** as secondary visual rhythm — used in utility bar AND in service
   cards. Creates continuity.
6. **One vertical hero photo spanning the full right column** — instead of a centered-and-
   cropped landscape image, the worker stretches floor-to-ceiling, which makes the page
   feel anchored.
7. **Body copy in soft slate, NOT black** — calmer feel than typical trade-template "every
   word maximum-contrast."

### Transferable lesson

"Visual ceiling" here means **a confident two-color base (white + royal-blue) with a third
deep-navy used for emphasis sections, single-typeface restraint (Outfit), generous soft-
rectangle CTAs, and one strong vertical hero photo**. The yellow + pale-sky micro-accents add
detail without breaking the calm. Restraint, not maximalism — but more textured than "single
accent on white" undersells.

### Where v013 went wrong (to fix on a redo)

- Shipped dark-navy + electric-cyan + gold serif display (SaaS-luxe magazine direction).
  Should have been white-base + royal-blue + selectively-navy-emphasis with a single sans
  family.
- Used Bricolage Grotesque + Inter pair. Should have been a single Outfit-style geometric
  sans throughout.
- Used full-bleed dark-navy hero. Should have been white hero with photo on right, navy
  reserved for the About / Our Work emphasis sections.
- Missed the `+` -sign stat trio entirely. Missed the pale-blue icon-pill rhythm.

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