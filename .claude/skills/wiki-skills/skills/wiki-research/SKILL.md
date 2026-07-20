---
name: wiki-research
description: >
  Research a topic on the web to fill a gap in the pt-buyers-kb knowledge
  base. Use when the user says research, investigate, find sources on, fill
  the gap on, or asks for external information the wiki does not yet cover.
  Produces a source-candidate document for human curation — it does not
  write directly into raw/ or wiki pages.
---

# Wiki Research

Research feeds the KB's curation pipeline; it does not bypass it. The human
curates sources — research produces candidates, not ingested truth.

1. Check the wiki first (`Home.md`, `index.md`, relevant pages, the Known
   gaps list in `AGENTS.md`). State what the KB already covers so research
   targets the actual gap.
2. Run web research on the gap. Prefer primary sources: Diário da República
   for legislation, official portals (AT, IMPIC, câmaras municipais),
   standards bodies, peer-reviewed or industry-technical material. For
   Portuguese legal/regulatory topics, search in Portuguese as well as
   English.
3. Write a research report to `07-inbox/research-<slug>-YYYY-MM-DD.md`:
   - frontmatter per AGENTS.md schema (`type: source`, `status: draft`,
     `verified: false`)
   - findings with per-claim source URLs and access dates
   - preserve exact quantitative thresholds and legal citations — never
     paraphrase away a number
   - a `> [!warning]` callout on anything single-sourced or conflicting
   - a recommendation section: what should be ingested into `raw/`, what
     pages it would touch, what remains open
4. Do **not** write to `raw/` (immutable, human-curated), wiki pages, or
   `index.md`. The report waits in `07-inbox/` for human review; ingestion
   is a separate, explicit step.
5. Append to `log.md`: `## [YYYY-MM-DD] research | topic` + 2–3 lines.
