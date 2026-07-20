---
name: wiki-query
description: >
  Answer a question from the pt-buyers-kb knowledge base with citations. Use
  when the user asks what the wiki says about a topic, requests a comparison
  or analysis grounded in the KB, or says query the wiki, check the kb, what
  do we know about. Executes the Query operation defined in AGENTS.md at the
  repo root.
---

# Wiki Query

Execute the **Query** operation exactly as specified in `AGENTS.md` at the
repository root. Read AGENTS.md first if it is not already in context.

1. Read `Home.md` and `index.md`, drill into only the relevant pages, and
   answer with wikilink citations.
2. Honest gaps: if the wiki does not contain the answer, say so and suggest
   what to ingest — never fill gaps from general knowledge without labeling
   it as outside the KB.
3. Respect `verified:` status — flag when an answer rests on unverified
   technical/legal claims.
4. If the answer is valuable (comparison, analysis, decision), file it in
   `06-syntheses/` with proper frontmatter and append to `log.md`.
   Explorations must compound.
