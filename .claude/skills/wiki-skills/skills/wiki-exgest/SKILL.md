---
name: wiki-exgest
description: >
  Repurpose compiled pt-buyers-kb wiki content into platform-facing drafts.
  Use when the user says exgest, generate output, draft a pSEO page, lead
  magnet, social thread, or email sequence for inspectos or homeos. Executes
  the Exgest operation defined in AGENTS.md at the repo root.
---

# Wiki Exgest

Execute the **Exgest** operation exactly as specified in `AGENTS.md` at the
repository root. Read AGENTS.md first if it is not already in context.

1. Required inputs: target platform (`inspectos` | `homeos`) and format
   (pSEO page | lead-magnet PDF draft | social thread | email sequence).
   Ask if either is missing.
2. Walk `Home.md` → relevant pages, filtering by `brand:` matching the target
   or `shared`.
3. Prefer `verified: true` pages for technical/legal claims; flag any
   unverified claim in the draft with a `> [!warning]` callout.
4. Repurposing rule: a `shared` page may spawn two outputs — same facts,
   different register. `inspectos` = technical authority, mechanism-first,
   tool/standard-citation heavy. `homeos` = exposure/leverage,
   risk-to-money translation. Numbers and legal citations never change
   between the two.
5. Emit drafts to `09-output/{platform}/{format}/`. **Never** write to
   `raw/`, wiki pages, or `index.md` during Exgest.
6. Remind the user: human review before anything is published.
7. Append to `log.md`:
   `## [YYYY-MM-DD] exgest | {platform} | {format} | {topic}`.
