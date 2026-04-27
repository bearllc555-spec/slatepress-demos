# How to Design a Plumbing Website

*A thesis derived from the Slatepress Plumbing Design References — Plumbing X, Plumbly, ProHauz, and Anderson Plumbing.*

*Written 2026-04-27 by Claude in collaboration with Anthony, after deep-pass observation (screenshots + computed source) on all four reference sites. Companion to [plumbing-design-references.md](./plumbing-design-references.md).*

---

## I. The decision you're designing for

A plumbing website is not a brand experience. It is not a portfolio. It is not a place where users wander, browse, and "discover." It is a **30-second triage tool** for somebody whose kitchen is flooding, whose water heater just died at 9pm, or whose kid's birthday party is tomorrow and the toilet is overflowing.

That visitor is in a state of mild-to-acute stress. They are scrolling on their phone, with one eye on the problem and one eye on the screen. They have already decided, before landing, that they want a real plumber to show up — fast. The website's only job is to compress the distance between *"I have a problem"* and *"I just called somebody who can fix it."*

Every design choice in this thesis flows from that single insight. If a move helps the visitor make the call faster or with more confidence, it earns its place. If it doesn't, it gets cut.

The four reference sites — three high-end Webflow / Framer / WordPress templates and one real local plumber (Anderson Plumbing in San Diego) — converge on the same playbook because they all understand this. They are optimizing for the same human moment, and the moves that win are remarkably consistent.

---

## II. The structural floor: what every great plumbing site does

There are fifteen non-negotiable patterns shared by all four references. Treat them as the floor — a design that omits any of them is incomplete.

**One brand color, committed.** Pick a single saturated brand color and use it everywhere — logo, eyebrow text, icon pills, primary CTA, stat callouts, footer accent. White carries the breathing room. Black or deep navy handles contrast text and one emphasis section. Three of the four references use blue; Anderson uses hot magenta. The point is not "pick blue" — it's "pick *one* and commit." Pastel palettes and three-color compromises read as templates.

**Bold sans-serif typography, single family.** Heavy display weights (700–800), no serifs, no scripts, no italic flourishes. Body text in a softer neutral than pure black so headlines read calm-confident rather than shouty. Plumbing X uses Outfit at 68px / weight 700 for the H1 and `#6E7891` slate for body — that softness is what keeps the page from feeling aggressive.

**A 50/50 hero with one dominant image.** Text on the left, one big image on the right. The image is either a real plumber, a real fleet vehicle, or both. Eyebrow → display H1 with one keyword highlighted in brand color → 40-to-60-word lede → primary CTA + phone CTA + star rating with review count. Everything needed to convert lives above the fold. No sliders. No video backgrounds. One image, one decision.

**The phone is a primary CTA in three places.** Top utility bar, hero, footer. Pill button or large numerical display, brand-colored. The phone is the thing that closes the deal — never a tertiary footer afterthought. Anderson puts it twice in the header alone. Plumbing X puts it in the utility bar AND the hero. ProHauz makes the phone number sticky.

**A trust trio or 4-up benefits row early in the page.** Three or four short value props with thin-stroke line-icons in brand color, bold heading, and 2–3 lines of explanation. Pick the four claims that match the brand: *Licensed / 24-7 / Up-front pricing / Family-run.* All four references have this section, in roughly the same place — right after the hero.

**Big-number stats somewhere on the page.** Concrete numbers at 60–100px+ display weight: *Years in business. Jobs done. Response time. Review count.* Anderson's "4.8 out of 4,462 reviews" is the gold standard — the number is so specific it cannot be invented. Vague *"trusted by thousands"* is what templates write. A real plumber writes the number.

**Section background shifts for rhythm.** None of the four references is a wall of white. Each alternates white with one or two emphasis backgrounds (deep navy, brand-color band, black, yellow band). Each section reads as a chapter, not a scroll. The eye gets cues that something new is happening.

**Soft-rounded CTAs in brand color.** Pill or 10px-radius rectangle, generous padding (Plumbing X measures 26px × 38px), brand-colored fill, white text. Calendar or phone icon optional. No sharp corners on any primary action — sharp edges read as 2008.

**Concrete social proof with platform attribution.** Star rating + review count + the actual Google or Yelp logo. Anderson uses the Google G logo on every review card, with Google's default colored-initial avatars (G, J, A in colored circles) preserved faithfully. *Don't fight Google's avatar style — it's a credibility cue.* Avoid generic "loved by neighbors" — use the platform mark.

**Service area shown as a graphic, not a list.** Anderson's embedded Google Map with ~25 pink-colored pins beats a comma-separated list of towns every time. Visual proof of "we cover this area."

**Membership or guarantee block.** An explicit ongoing-relationship offer, not just a one-time service pitch. Anderson's AMP Plan. A "100% Satisfaction Guaranteed" promise. A maintenance-tune-up plan card. The page should make at least one offer beyond the immediate emergency.

**Service cards with real action photography.** Each card is real photo of the work + small overlay icon in brand color + bold service name + 1–2 line description + "Read more" or "Schedule" link. Stock-flat illustrations don't work; real photos of chrome faucets being repaired, hands on wrenches, drains being cleaned do.

**A repeat hero CTA in the footer.** Phone + Schedule pill + tagline + 24/7 promise. Catch the bottom-of-page reader who scrolled past everything else and is still deciding.

**One signature decorative motif.** Pick a graphic mark and let it recur: ProHauz's `+ + +` plus-grid pattern, Plumbly's pale-blue wave shapes, Anderson's pink wedge-blob bleeds at section transitions, Plumbing X's amber `+`-symbol stat highlights. Each gives the brand a fingerprint without distracting. A site without one feels generic.

**Stylized line-iconography everywhere.** Water drops, wrenches, faucets, drains, certificates, trucks, calendars, dollar signs, clocks. Always thin-stroke line, always brand-colored, often inside circular pills. Used for services, trust pillars, and footer link-clusters. Replaces clip-art and stock SVG.

These fifteen are the floor. Hit them all and you have a competent plumbing website. Miss any one of them and you have a website that converts measurably worse than its peers.

---

## III. The specificity ceiling: what separates Anderson from the templates

Three of the four references are pretty templates pretending to be plumbers. Plumbing X, Plumbly, and ProHauz are commercial templates sold to anyone with a credit card — their photos are stock-feeling commissioned shoots, their copy is lorem ipsum, their "team" portraits in Plumbly's case appear to be AI-generated. They hit the structural floor. They get an A on the 15 rules.

Anderson Plumbing is a real plumber pretending to be a brand. Their photography shows their actual painted-pink fleet van against the actual San Diego skyline. Their About section shows their actual technician *Ferreira* — name visible on his uniform, American flag patch on his sleeve, standing in front of one of their actual open vans. Their tagline ("Nobody wows clients like we do!®") is registered as their own intellectual property. Their review count is "4,462," not "thousands." Their service-area map shows the specific neighborhoods they serve, not a vague radius.

Anderson is the only one of the four references that a competitor cannot copy by buying a template. **Specificity is unfakeable.**

This is the central thesis on what separates a forgettable plumbing website from a memorable one: *the structure is the floor, but specificity is the wedge.*

Specificity in plumbing-web design takes five forms:

1. **Real fleet photography.** The actual truck, painted in the brand color, in the actual local geography. (Anderson's pink van + San Diego skyline.)
2. **Named technicians.** Real names on real uniforms. Not "our team" — *Ferreira, Frank Sr., Frank Jr., Anthony.*
3. **Concrete review counts with platform logos.** Not "5-star service" — *"4.8 across 4,462 verified Google reviews"* with the Google G mark.
4. **Awards as graphic proof.** Anderson's strip of six real third-party awards (BBB Torch, Best of San Diego, Angi Super Service, etc.) renders as visual credibility a template can't fake without lying.
5. **A registered tagline.** "Nobody wows clients like we do!®" is brand territory. The ® mark is a signal that the company has invested in their identity beyond a website.

A new plumber demo can't hit all five on day one. But every demo should be designed *to make room* for them — placeholder slots for the real fleet photo, the real technician portraits, the real review count. When the customer fills in the specifics, the site upgrades from template-pretty to brand-specific without redesign.

---

## IV. Image grammar: photography is the real differentiator

If you read one section of this thesis, read this one.

**Stock photography is the "I'm a template" tell.** A homeowner who has been on three plumbing-company websites in the last 10 minutes can spot stock-feeling photos instantly. The composition is too perfect. The lighting is too flat. The plumber's beard is too groomed. The chrome is too polished. The instinct fires: *this isn't a real local guy, this is a corporate website.* And the visitor closes the tab.

**Real photography is the "I'm a real local plumber" tell.** Even if the photos are amateur — phone shots, slightly off-center, with normal-looking lighting — the visitor's instinct fires the other way: *this is a real person who actually does this work in my neighborhood.* And the phone call follows.

This is the single highest-leverage decision in plumbing-website design. The 15 structural rules can be hit by anyone with a template. The image grammar — *real photos of the real fleet, real people, and real work* — is what wins the click.

For a customer that doesn't yet have professional photography, the move is: shoot the fleet (a phone shot of the truck parked in front of the shop is enough), shoot the owner (in uniform, against the shop wall), shoot one or two recent jobs (a kitchen sink they fixed last week — the homeowner gave permission). Three real photos beat thirty stock ones.

### The category-coding test

**The hero photo is a category badge.** Visitors classify what kind of business a website is from the image *before* they read the headline. A pool photo says pool contractor. A pizza shot says pizzeria. A stethoscope says doctor. A pristine countertop says kitchen remodel. *A gloved hand on a clean chrome surface says maid service.* If the photo signal contradicts the headline signal, the visitor's gut wins, the headline loses, and they bounce.

The diagnostic: **a returning visitor who can't read English should still know what kind of business this is from the hero photo alone.** If the image could plausibly belong to an adjacent category — cleaning service, HVAC, hardware store, kitchen remodeler, real estate listing, generic-construction, landscaping — the photo is wrong, no matter how nice it looks.

For a plumbing site, the hero photo MUST show ONE of two things — and nothing else qualifies:

1. **A full plumber.** A person — face/body visible — who is either holding plumbing tools, wearing a branded plumbing uniform, or actively working on plumbing fixtures. The reference sites prove this: Plumbing X = worker in blue hardhat against kitchen plumbing; Plumbly = silver-haired plumber kneeling at a sink; ProHauz = bearded plumber holding a tablet next to plumbing tools. Three of four references hit this.

2. **A branded fleet vehicle.** A van or truck with the plumbing company's wrap, logo, or branded panels visible. Anderson is the canonical example — their painted-pink Ford Transit against the San Diego skyline. One of four references hits this.

Bonus combo if you can find it: **a plumber standing next to their fleet vehicle** (Anthony's update 2026-04-27 — this is the strongest possible hero because it stacks both signals).

What does NOT qualify — even when the content is technically plumbing-coded:

- **Hands-only shots.** Gloved hands wrapping a wrench on a pipe, hands on a boiler control panel, hands installing a fixture. Plumbing-coded but missing the human/service element. The visitor needs to see WHO is doing the work, not just the work. Failure case: v017–v020 first attempt used `7859953` (hands on Grundfos boiler) for v019. Looked plumbing-y, didn't pass.
- **Bare fixtures.** A clean chrome faucet, a pristine bathroom, a stainless sink. Even if the fixture is unambiguously plumbing, no person means no service signal. Failure case: v020 first attempt used `4494662` (chrome faucet + blue pipe). Tested perfectly for "plumbing fixture," tested zero for "plumber I should call."
- **Tools alone.** A pipe wrench on a wood floor, a row of tools on a bench. Equipment without operator reads as "hardware store" or "stock photo library."
- **Decorative cutaways or illustrations.** Same problem — no human service-provider on screen.

The deeper insight, refined: **plumbing-coded content alone isn't enough. The hero has to answer the visitor's two questions simultaneously: (a) what kind of business is this (plumbing) AND (b) who's doing the work (a plumber, or my plumber's truck pulling up to my house).** A bare fixture answers (a) but not (b). A pair of hands answers (a) but not (b). A full plumber or a branded van answers both.

What does NOT category-code as plumbing AT ALL — these are the harder failures:

- A gloved hand wiping a clean chrome surface → cleaning / maid service
- A pristine bathroom with no work happening → real estate listing / bathroom remodel
- A worker in generic hardhat without plumbing tools or pipes visible → construction
- A landscape or mountain photo (yes, this happened — a mis-tagged stock library entry) → tourism
- Foliage / green plants → landscaping
- An empty kitchen sink → kitchen remodel
- A man holding a tablet in business clothes → tech / consulting

The deeper insight: **photographic content does category recognition before language does.** This is why stock plumbing libraries fail so reliably — most "plumbing" stock photos are actually category-ambiguous chrome shots that could be cleaning, kitchen, or real estate. When picking from any stock library (Pexels, Unsplash, paid), apply the can't-read-English test on every candidate. Reject anything that doesn't pass.

This rule is also why specificity wins. Anderson's painted-pink fleet van against the San Diego skyline is unambiguously a plumbing service vehicle — no other category looks like that. Real fleet beats curated stock for the same reason: nobody mistakes a branded plumber's van for anything else.

---

## V. Anti-patterns: what kills conversion

The negative space of this thesis. Things to refuse, even when the customer requests them:

- **Pastel-palette compromises.** "Make it soft and modern with cream and sage and dusty blue." No. Pick one saturated color. Soft pastels read as wedding-vendor or wellness-clini