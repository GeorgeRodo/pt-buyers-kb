---
name: wiki-lint
description: >
  Run a health check on the pt-buyers-kb knowledge base. Use when the user
  says lint, health check, check the wiki, find orphans, find contradictions,
  audit structure, or clean up the inbox. Executes the Lint operation defined
  in AGENTS.md at the repo root.
---

# Wiki Lint

Execute the **Lint** operation exactly as specified in `AGENTS.md` at the
repository root. Read AGENTS.md first if it is not already in context.

Checks to run (AGENTS.md is authoritative if they ever diverge):

- Contradictions between pages; claims superseded by newer sources
- Orphan pages (no wikilink from any hub) — `09-output/` is **excluded**
  from orphan checks, it is not part of the wiki graph
- Non-empty `07-inbox/` — lint passes must empty it
- Concepts mentioned on 3+ pages without their own page (promote trigger)
- Pages that have accumulated a second distinct concept (split trigger)
- Stubs older than 30 days
- Defect pages missing legal-weapon tags
- Regulatory citations needing re-verification (IMT brackets, AL containment
  zones — these change yearly)
- Frontmatter completeness per the mandatory schema in AGENTS.md

Report findings grouped by severity before fixing anything. Mechanical fixes
(index rows, missing links, frontmatter fields) may proceed after the user
confirms; content-level fixes (contradictions, splits) need per-item
discussion. Append the pass to `log.md`.

Useful mechanics: extract wikilinks with grep/sed across `*.md`, compare
against `index.md` rows, and cross-check frontmatter `updated:` dates.
