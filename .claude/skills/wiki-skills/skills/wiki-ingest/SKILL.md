---
name: wiki-ingest
description: >
  Ingest a new source document into the pt-buyers-kb knowledge base. Use when
  the user says ingest, add source, file this document, process raw file, new
  source arrived, or drops a document intended for the wiki. Executes the
  Ingest operation defined in AGENTS.md at the repo root.
---

# Wiki Ingest

Execute the **Ingest** operation exactly as specified in `AGENTS.md` at the
repository root. Read AGENTS.md first if it is not already in context.

Summary of the contract (AGENTS.md is authoritative if they ever diverge):

1. **GDPR precondition first.** Before anything else, check the file for
   client-identifying data (names, addresses, contacts, specific negotiation
   outcomes). `raw/` is immutable, so an unsanitized file must be refused —
   explain why and stop.
2. Read the source in full.
3. Discuss key takeaways with the user before filing, unless they asked for
   batch mode.
4. Write/update a summary page in `sources/` (frontmatter per AGENTS.md;
   field reports are valid sources; apply the 3+ field-report promotion rule).
5. Integrate across every phase, platform, domain, and entity page the source
   touches (typically 5–15 pages). Flag contradictions with a `> [!warning]`
   callout — never silently overwrite. Rewrite and improve existing pages
   rather than appending.
6. Update `index.md`.
7. Append to `log.md`: `## [YYYY-MM-DD] ingest | Source Title` + 2–3 lines.

Arguments: if the user names a specific file, ingest that file. If they say
"ingest" with no target, list unprocessed files in `raw/` (files with no
matching `sources/` page) and ask which to process.
