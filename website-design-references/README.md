# Website Design References

Working specs and design rules for every plumbing website Slatepress builds. **Locked at v1.0 as of 2026-04-27.**

## Read this first

| File | What it is |
|---|---|
| **[plumbing-design-system-v1.0.md](./plumbing-design-system-v1.0.md)** | **The canonical lock.** Single source of truth for the system: 15 structural rules, photo category-coding rule, motion engine, reference-handling protocol, four-reference DNA index, required sections, pricing/specificity conventions, versioning policy. **Read this before any plumbing design pass.** |

## Companion specs (supply detail behind v1.0)

| File | What it has | When to read |
|---|---|---|
| [plumbing-website-design-thesis.md](./plumbing-website-design-thesis.md) | The strategic argument behind every rule — why crisis-decision design, why specificity is the wedge, why image grammar is the differentiator. | When you need the "why" behind a rule, or when explaining the system to a customer. |
| [plumbing-design-references.md](./plumbing-design-references.md) | Per-site deep-pass observations on Plumbing X / Plumbly / ProHauz / Anderson — palette hex codes, type families, distinguishing moves, where prior De Vito mockups went wrong on each. | When picking which reference DNA to lift for a new design. |
| [text-motion-spec.md](./text-motion-spec.md) | The canonical CSS+JS for the motion engine. | When implementing motion in a new design (or copy from `assets/scaffold-v1.html`). |
| [reference-handling-protocol.md](./reference-handling-protocol.md) | The always-screenshot-and-view-source rule with the exact tool calls. | When handed a new reference URL by Anthony. |

## Starter scaffold

The locked v1.0 starter HTML scaffold lives at:

`outputs/plumbing-site-generator/assets/scaffold-v1.html`

Fork this when starting a new design direction. All 15 rules baked in, motion engine fixed, all 11 required sections present, Mustache placeholders for content, photo defaults that pass the category-coding test, pricing disclaimer footer.

## How this gets used

Before any new design pass — a new plumber demo direction, a refresh of an existing version, a redesign of the main site, anything visual:

1. Read **plumbing-design-system-v1.0.md** in full.
2. Pick which reference DNA leads (visual ceiling / IA / conversion / warmth) — see § 7 of the system doc.
3. Fork `scaffold-v1.html`. Set `--brand` to the target color. Pick one font family.
4. Specialize: add the customer's signature decorative motif, fill in Mustache placeholders, replace `[SPEC: ...]` photo URLs with verified library picks (apply the category test on every hero candidate per § 4 of the system doc).
5. Verify the photo on the live deployment before declaring shipped.

## What this is NOT

- Not a template gallery — actual deployed templates are `de-vito-plumbing_017` through `_020` in this repo.
- Not a brand-guidelines doc for Slatepress itself — that lives at slatepress.co.
- Not customer-specific — these rules apply to every plumbing site built, regardless of customer.

## Mirror locations

These same files are mirrored to:
- The work directory: `outputs/plumbing-site-generator/references/`
- The local backup: `~/Downloads/slatepress-skills-backup/plumbing-site-generator/references/`

If any of the three diverge, **the GitHub copy in this folder is the source of truth.**

## Versioning

System is **v1.0** as of 2026-04-27. Future rule additions become v1.1, v1.2, etc., with a changelog in plumbing-design-system-v1.0.md § 10. Breaking changes become v2.0 (discuss with Anthony first).
