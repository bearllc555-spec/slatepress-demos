# Website Design References

Working specs and design rules for every website Slatepress builds — plumbing demos, the
slatepress.co main site, the blog, and any future variants. Anthony states each rule
explicitly and we add it here so the rule survives across sessions.

## What's in here

| File | What it is | Stated |
|---|---|---|
| [text-motion-spec.md](./text-motion-spec.md) | Five non-negotiable text-animation rules: word fade-up on H1, letter reveal on H2, fx-row stagger on lists/cards/paragraphs, kicker-pulse on live-status dots, and a restrained-not-frenetic feel test. Includes the canonical CSS+JS implementation. | 2026-04-27 |
| [reference-handling-protocol.md](./reference-handling-protocol.md) | Rule for how to handle URLs given as design inspiration: ALWAYS screenshot the page AND view the source code before any creative work. No working from page text or archetype memory alone. | 2026-04-27 |

## How this gets used

Before any new design pass — a new plumber demo direction, a refresh of an existing version,
a redesign of the main site, anything visual — read every file in this folder first. The
rules compound: a design that has motion but ignores reference-handling will hit the right
animation but the wrong palette; a design that screenshots references but skips motion will
look right but feel static.

When Anthony states a new rule, add it here as a new file (one rule per file, named after
the concept), then update this index, then commit. Keeping rules in separate files makes
them easier to link to in conversation ("see [reference-handling-protocol.md](./reference-handling-protocol.md)")
than burying them in a single design.md.

## What this is NOT

- Not a template gallery — actual templates live in `outputs/plumbing-site-generator/assets/`
  in the work directory, not here.
- Not a brand-guidelines doc — Slatepress's own brand lives at slatepress.co.
- Not customer-specific — these rules apply to every site built, regardless of customer.

## Mirror locations

These same files are mirrored to:
- The work directory: `outputs/plumbing-site-generator/references/`
- The local backup: `~/Downloads/slatepress-skills-backup/plumbing-site-generator/references/`

If any of the three diverge, **the GitHub copy in this folder is the source of truth.**
