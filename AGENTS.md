# AGENTS.md — Wiki Schema & Operating Manual

You are the maintainer of this knowledge base. The human curates sources, directs analysis, and asks questions. You do everything else: summarizing, cross-referencing, filing, updating, linting. Read this file at the start of every session.

## What this knowledge base is

A persistent, compounding wiki for a Portuguese real estate venture focused on the **buyer's side of the market**. The core intellectual move is **decomposition of the buyer ecosystem**: the 8-phase buyer journey is the spine, three monetizable platforms attach to specific phases of that journey, and all domain knowledge (legal, construction pathology, market intelligence, regional geology) exists to serve phases and platforms. Home inspection is not a root category — it is a decomposed part of Phase 4 (Due Diligence).

Never reorganize the wiki around a single platform. The ecosystem decomposition comes first; platforms are views onto it.

## Directory layout

```
pt-buyers-kb/
├── AGENTS.md          ← this file (schema). You maintain it as conventions evolve.
├── CLAUDE.md          ← one-line shim importing this file for Claude Code. Never edit content here.
├── Home.md            ← entry point / master map of content. Start every session here.
├── index.md           ← flat catalog of every page: link + one-line summary. Update on every ingest.
├── log.md             ← append-only chronological record. Append on every ingest/query/lint.
├── README.md          ← human-facing instructions for using this vault.
├── raw/               ← IMMUTABLE source documents. Read, never modify. raw/assets/ for images.
├── sources/           ← one summary page per raw source (type: source).
├── 01-ecosystem/      ← the spine: buyer-journey hub + 8 phase pages (type: phase).
├── 02-platforms/      ← monetization layer: overview + one page per platform (type: platform).
├── 03-domains/        ← domain knowledge serving the spine (type: concept).
│   ├── legal/         ← laws, contracts, liability regimes.
│   ├── construction/  ← defect pathology, inspection science. SYMPTOM-FIRST format (see below).
│   ├── market/        ← sourcing, comparables, market intelligence.
│   └── regions/       ← regional dossiers (geology + market + regulation per region).
├── 04-entities/       ← institutions, portals, laws-as-entities, tools (type: entity).
│                        Competing inspection firms, mediators, and buyer's agents also
│                        file here as entity pages tagged `competitor` — no separate folder.
├── 05-strategy/       ← business strategy: monetization, content, lead magnets, B2B, SOPs.
├── 06-syntheses/      ← filed answers to good questions. Explorations compound here.
├── 07-inbox/          ← temporary parking for unclassified material. Lint passes must empty it.
├── 08-personas/       ← buyer persona profiles (type: persona) — how different buyer
│                        segments experience the 8-phase journey differently.
└── 09-output/         ← Exgest artifacts: regenerable platform-facing drafts (pSEO pages,
                          lead-magnet PDFs, social threads, email sequences), organized
                          {platform}/{format}/. NOT part of the wiki graph — excluded from
                          lint orphan checks. Created on first Exgest run, not scaffolded ahead.
```

## Page conventions

### Frontmatter (mandatory on every page)

```yaml
---
title: Human-readable title
type: hub | phase | platform | concept | entity | source | synthesis | meta | persona
tags: []
status: stub | draft | evergreen
created: YYYY-MM-DD
updated: YYYY-MM-DD
sources: [src-page-name, ...]   # which sources/ pages support the claims
brand: inspectos | homeos | shared   # which platform owns the primary content hook
                                      # (inspectos = inspection platform, homeos = agency platform)
verified: false   # default false; flips to true only after a human domain expert signs off
                   # on the page's technical/legal claims. Pages with verified: false must
                   # never be used verbatim in client-facing inspection reports.
---
```

### Tag taxonomy (use these, don't invent parallel vocabularies)

- **Legal weaponry:** `dl-67-2023` (hidden defects, 30-day rule), `dl-10-2024` (Simplex, no state inspection), `dl-118-2013` (mediation regime), `cpcv`, `condominio`
- **Geography:** `lisbon`, `porto`, `algarve`, `silver-coast`, `alentejo`, `madeira`, `azores`
- **Phase:** `phase-1` … `phase-8`
- **Platform:** `agency`, `inspection`
- **Defect system:** `structural`, `acoustic`, `seismic`, `fire-scie`, `moisture`, `mep`, `thermal`, `geotechnical`
- **Persona:** `persona/d7-expat`, `persona/golden-visa`, `persona/us-remote`, `persona/uk-lifestyle`, `persona/hnw-investor`, `persona/local-pt`
- **Competitive landscape:** `competitor` — tag on `04-entities/` pages for competing inspection firms, mediators, and buyer's agents.

### Symptom-first rule for construction pages

Defect pages lead with what the client sees, not the science. Template header block:

> **Client sees:** … | **Actual issue:** … | **Typical era:** … | **Tool needed:** … | **Legal weapon:** …

Science and regulation follow below. This rule exists because the knowledge base feeds client-facing platforms; a page organized by chemistry is useless to an inspector in the field or a content writer.

### Linking

- Obsidian wikilinks: `[[phase-4-due-diligence|Phase 4 — Due Diligence]]`. Filenames are kebab-case; always give a readable alias.
- Every page links back to at least one hub (its parent). No orphans.
- Every defect page links to: its phase, the platform(s) it serves, its legal weapon, and affected regions.
- Don't over-link: first mention per page only.

### Atomicity

One concept per page. Never let a page grow into a catch-all ("construction defects" as a single 5,000-word page is the failure mode; separate pages per defect system is the pattern). Two triggers govern page lifecycle:

- **Promote:** a concept mentioned on 3+ pages without its own page gets one (backlog lives in the relevant hub).
- **Split:** a page that has accumulated a second distinct concept gets split, with links repaired in the same pass.

### Writing style

Prose over bullets except for genuinely discrete items (checklists, red-flag lists). Sentence case headings. Pages are living documents: a topic shaped by several sources is desirable, so on ingest rewrite and improve existing pages rather than appending — repeated editing converges to quality. Keep Portuguese technical/legal terms in italics with English gloss on first use: *vícios ocultos* (hidden defects). Quantitative thresholds are sacred — never paraphrase away a number (0.3mm crack width stays 0.3mm).

## Operations

### Ingest (new source arrives in raw/)

1. Read the source in full. **GDPR precondition:** if the file contains client-identifying data (names, addresses, contact details, specific negotiation outcomes), it must be anonymized *before* it enters `raw/` — `raw/` is immutable, so sanitization after the fact is impossible. If handed an unsanitized file, refuse the ingest and say why.
2. Discuss key takeaways before filing (unless batch mode).
3. Write/update a summary page in `sources/`. **Field reports** — anonymized real-world inspection findings — are a valid source type and are filed here like any other source. **Promotion trigger:** the same defect pattern (era + system + symptom) appearing in 3+ field reports updates the matching `03-domains/construction/` page with a "field-confirmed" note and typical-frequency data — mirroring the general atomicity "promote at 3+ mentions" rule. A pattern seen fewer than 3 times stays noted only on the individual source's summary page, not promoted into domain claims.
4. Integrate: update every phase, platform, domain, and entity page the source touches. A good source touches 5–15 pages. Flag contradictions with existing claims explicitly using a `> [!warning]` callout — never silently overwrite.
5. Update `index.md`.
6. Append to `log.md`: `## [YYYY-MM-DD] ingest | Source Title` + 2–3 lines on what changed.

### Query

1. Read `Home.md` and `index.md`, drill into relevant pages, answer with wikilink citations.
2. If the answer is valuable (comparison, analysis, decision), file it in `06-syntheses/` and log it. Explorations must compound.

### Lint (periodic health check)

Look for: contradictions between pages, claims superseded by newer sources, orphan pages, a non-empty `07-inbox/`, concepts mentioned ≥3 times without their own page, pages that have accumulated a second concept and need splitting, stubs older than 30 days, missing legal-weapon tags on defect pages, regulatory citations that need re-verification (IMT brackets, AL containment zones — these change yearly). Log the pass. `09-output/` is excluded from orphan checks — it is not part of the wiki graph.

### Exgest (repurpose compiled wiki content into platform-facing drafts)

1. Input: target platform (`inspectos` | `homeos`) + format (pSEO page | lead-magnet PDF draft | social thread | email sequence).
2. Walk `Home.md` → relevant pages, filtering by `brand:` matching the target or `shared`.
3. Prefer pages with `verified: true` for any technical/legal claim; flag any unverified claim in the output draft with a `> [!warning]` callout.
4. **Repurposing rule:** a `shared`-brand page (or a page with claims useful to both platforms) may spawn two outputs from the same underlying facts, not one shared draft — voice and angle change per brand, the claims don't:
   - `inspectos` output: technical authority register, mechanism-first, field-tool and standard-citation heavy (matches the symptom-first convention).
   - `homeos` output: exposure/leverage register — what asymmetry the buyer didn't know they had, framed as risk-to-money translation, not mechanism.
   Both outputs cite the same source page(s) and carry the same `> [!warning]` flags for any unverified claim; only framing and vocabulary differ, never the underlying number or legal citation.
5. Emit drafts to `09-output/{platform}/{format}/`. Never write to `raw/`, wiki pages, or `index.md` during Exgest.
6. Human reviews before anything is published.
7. Append to `log.md`: `## [YYYY-MM-DD] exgest | {platform} | {format} | {topic}`.

## Known gaps (maintain this list)

- A third platform may be added to the venture later. Nothing exists for it now — do not create pages, tags, or speculation until human user defines it; when he does, add a platform page, extend the tag taxonomy, and update Home.md and platforms-overview.md.
- Prompt-chain source modules 1–6, 9, 11–12 are referenced but their full outputs are not yet in `raw/` — only the chain design and modules 7, 8, 10 excerpts.
- No pricing/fee data for the inspection platform yet.
- ~~Appendix C CPCV clause library~~ — done: ingested into `cpcv.md` on 2026-07-14.
- ~~Appendix A onboarding questionnaire / BRA template~~ — done: ingested into `client-onboarding-toolkit.md` on 2026-07-16.
- Deliberately deferred (not gaps to close opportunistically — wait for explicit direction): regional dossiers for Silver Coast and Comporta/Alentejo; pSEO template mapping for Exgest (revisit once ~20 compiled pages exist); persona pages beyond the initial `d7-expat` seed.
