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

---

## Tiers of trust

Every claim in this wiki carries a reliability tier. This is the central discipline of the knowledge base and it overrides convenience: an unsourced claim is not a claim, and a confident sentence with no tier behind it is worse than an admitted gap, because the wiki feeds client-facing platforms where a wrong number is a liability.

Three fields do three different jobs. Do not collapse them into one:

- **Tier** — how strong the evidence is. A property of the source and how far the claim travels from it.
- **Review** — whether a human with domain standing has read the claim against its source. A property of process.
- **Recheck** — the date after which the claim is presumed wrong until re-verified. A property of time.

A claim can be Tier A and unreviewed. It can be reviewed and Tier D. It can be both and still be stale. All three gates must pass before a claim goes to a client.

### The tiers

**Tier A — primary official, quoted or directly cited.**
*Diário da República* text, the law itself, published Portuguese and European standards (NP, EN, Eurocode), INE and IMT official releases, court decisions, official cartography, the *Portal da Habitação*. Numbers and legal citations at this tier are reproduced exactly. If you are paraphrasing, you have left Tier A.

**Tier B — official or established source, interpreted.**
A law firm's published analysis of DL 67/2023, an IMT bracket table reproduced by a reputable practice, a trade body's technical note, LNEC guidance, an internal analysis that reasons transparently from a Tier A source. The step from A to B is the step from *what the document says* to *what it means*. That step is where most of this wiki's value is created and also where most of its risk lives.

**Tier C — derived, sample-limited, or practitioner consensus.**
Field-report frequency data, portal scrapes, listing-site comparables, "typical era" attributions from inspection experience, an estimate built from proxy indicators. Legitimate knowledge, insufficient authority. Tier C claims may inform judgement and must never be stated as fact to a client.

**Tier D — single weak source, inference, or unrefreshed.**
One undated blog, a single anecdote, an internal guess, a competitor's marketing copy, or — most commonly — a claim that was Tier A or B and has passed its recheck date. Tier D is a holding pen, not a wastebasket: it records what we suspect so someone can go and verify it. It never leaves the wiki.

### Tier ceiling inheritance

**A claim cannot be tiered above its source.** If `sources/inspectos-strategy-corpus.md` is Tier C, no claim derived from it is Tier B, however well-reasoned the derivation. Every `sources/` page therefore carries a `tier:` in frontmatter, assessed at ingest, and that tier caps everything downstream of it.

Corroboration raises the ceiling: the same claim independently supported by a Tier A source and a Tier C source is Tier A, and both go in `sources:`. Corroboration between two Tier C sources is still Tier C — agreement between weak sources is not strength, it is often a shared origin.

### Auto-demotion

A claim past its `recheck` date is **Tier D until re-verified**, automatically, with no human decision required. Do not wait for a lint pass to notice; if you read a page during any operation and its recheck date has passed, demote it and note it in the log.

Default recheck intervals, applied at ingest unless the source implies otherwise:

| Claim type | Interval |
|---|---|
| IMT brackets, tax rates, statutory fee tables | 12 months |
| AL containment zones, municipal regulations | 12 months |
| Price data, comparables, market volumes | 6 months |
| Legislation in force, standards | 36 months, or immediately on a known amendment |
| Construction pathology, defect mechanisms | none — physics does not expire |
| Competitor pricing, positioning, service lines | 6 months |

Legislation gets a long interval and an override: any ingest that touches a law resets the recheck on every page citing it. DL 108/2026 came into force 3 August 2026 and will generate exactly this cascade.

### Notation

Frontmatter carries the page's **floor** — the weakest tier present anywhere on it. Inline, mark only claims that fall *below* the page's dominant tier. On a page where everything is Tier A, nothing is annotated and `tier_floor: A` says so. This keeps prose readable and makes annotation meaningful: a marker means "this one is weaker than the rest of this page."

Inline marker, Obsidian inline-footnote syntax so it renders and greps cleanly:

> Rendering typical of the 1998–2006 boom stock, where sand-rich mixes were common in the Algarve ^[C · pattern across 7 field reports, no published survey].

Grep pattern for lint: `\^\[[ABCD] · `.

For a claim that is disputed between sources, use the existing warning callout and give both tiers:

> [!warning] Contradiction
> DL 108/2026 removes the deed-stage licence check ^[A · DR 1ª série, 3 Aug 2026] but the InspectOS strategy corpus describes a residual municipal verification ^[C · strategy deck, undated]. Unresolved — see Known gaps.

### What each tier is allowed to do

| | Internal syntheses | Wiki prose | Client-facing output (Exgest) |
|---|---|---|---|
| **A, reviewed** | yes | yes | yes, quoted |
| **B, reviewed** | yes | yes | yes, attributed |
| **C, reviewed** | yes | yes, hedged | hedged language only, never as a number or legal assertion |
| **D** | yes, flagged | yes, flagged | never |
| **any tier, unreviewed** | yes | yes | only with a `> [!warning]` callout in the draft |

"Hedged" means the register changes, not the number: *"in the roughly 400 inspections behind this pattern, around a third of that era's stock showed…"* rather than *"a third of that era's stock shows…"*. Never hedge away a quantitative threshold — 0.3mm stays 0.3mm whatever tier it carries.

---

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

tier_floor: A | B | C | D   # weakest tier present anywhere on the page. Claims at this
                             # tier must be marked inline. Recompute on every edit.
review: unreviewed | reviewed | disputed
                             # reviewed = a human with domain standing has read the page's
                             # claims against their sources and signed off. `disputed` means
                             # a reviewer rejected a claim and the page is held pending
                             # resolution — treat as unreviewed for all output purposes.
reviewed_by: ""              # name, empty until review
reviewed_on:                 # YYYY-MM-DD, empty until review
recheck:                     # YYYY-MM-DD. Past this date the page's dated claims are Tier D.
                             # Omit only for pages with no time-sensitive claims.
---
```

On `sources/` pages, add one more field:

```yaml
tier: A | B | C | D          # the source's inherent strength. Caps every claim derived from it.
```

**Migration from `verified:`.** The old boolean `verified: true` maps to `review: reviewed` and does *not* imply a tier — sign-off was never evidence strength. Any page still carrying `verified:` gets converted on next touch: `true` → `review: reviewed`, `false` → `review: unreviewed`, and `tier_floor` assessed fresh against the page's actual sources. Do not assume a previously-verified page is Tier A.

### Tag taxonomy (use these, don't invent parallel vocabularies)

- **Legal weaponry:** `dl-67-2023` (hidden defects, 30-day rule), `dl-10-2024` (Simplex, no state inspection), `dl-108-2026` (Simplex phase 2, no deed license, in force 3 Aug 2026), `dl-118-2013` (mediation regime), `cpcv`, `condominio`
- **Geography:** `lisbon`, `porto`, `algarve`, `silver-coast`, `alentejo`, `madeira`, `azores`
- **Phase:** `phase-1` … `phase-8`
- **Platform:** `agency`, `inspection`
- **Defect system:** `structural`, `acoustic`, `seismic`, `fire-scie`, `moisture`, `mep`, `thermal`, `geotechnical`
- **Persona:** `persona/d7-expat`, `persona/golden-visa`, `persona/us-remote`, `persona/uk-lifestyle`, `persona/hnw-investor`, `persona/local-pt`
- **Competitive landscape:** `competitor` — tag on `04-entities/` pages for competing inspection firms, mediators, and buyer's agents.

Tiers are not tags. They live in frontmatter and inline markers so they can be computed on; a `tier/a` tag would drift out of sync with `tier_floor` within a week.

### Symptom-first rule for construction pages

Defect pages lead with what the client sees, not the science. Template header block:

> **Client sees:** … | **Actual issue:** … | **Typical era:** … | **Tool needed:** … | **Legal weapon:** …

The legal weapon field must be Tier A or B — a defect page whose legal hook rests on a Tier C source is not usable by either platform and should be marked as such at the top of the page rather than quietly shipped. The typical-era field is very often Tier C (practitioner attribution) and should carry an inline marker; this is the most common tier mistake on construction pages, because era attribution *reads* as established fact.

Science and regulation follow below. This rule exists because the knowledge base feeds client-facing platforms; a page organized by chemistry is useless to an inspector in the field or a content writer.

### Linking

- Obsidian wikilinks: `[[phase-4-due-diligence|Phase 4 — Due Diligence]]`. Filenames are kebab-case; always give a readable alias.
- Every page links back to at least one hub (its parent). No orphans.
- Every defect page links to: its phase, the platform(s) it serves, its legal weapon, and affected regions.
- Don't over-link: first mention per page only.

### Atomicity

One concept per page. Never let a page grow into a catch-all ("construction defects" as a single 5,000-word page is the failure mode; separate pages per defect system is the pattern). Two triggers govern page lifecycle:

- **Promote:** a concept mentioned on 3+ pages without its own page gets one (backlog lives in the relevant hub).
- **Split:** a page that has accumulated a second distinct concept gets split, with links repaired in the same pass. A split that produces one Tier A page and one Tier C page is a good split — a mixed `tier_floor` is often the signal that a page is holding two concepts.

### Writing style

Prose over bullets except for genuinely discrete items (checklists, red-flag lists). Sentence case headings. Pages are living documents: a topic shaped by several sources is desirable, so on ingest rewrite and improve existing pages rather than appending — repeated editing converges to quality. Keep Portuguese technical/legal terms in italics with English gloss on first use: *vícios ocultos* (hidden defects). Quantitative thresholds are sacred — never paraphrase away a number (0.3mm crack width stays 0.3mm).

---

## Operations

### Ingest (new source arrives in raw/)

1. Read the source in full. **GDPR precondition:** if the file contains client-identifying data (names, addresses, contact details, specific negotiation outcomes), it must be anonymized *before* it enters `raw/` — `raw/` is immutable, so sanitization after the fact is impossible. If handed an unsanitized file, refuse the ingest and say why.
2. **Tier the source before reading it for content.** Decide `tier:` from what the document *is*, not from how convincing it sounds — a well-written strategy deck is Tier C, a badly-scanned page of *Diário da República* is Tier A. State the assessment and your reasoning before proceeding. If the source is undated, it cannot exceed Tier C.
3. Discuss key takeaways before filing (unless batch mode).
4. Write/update a summary page in `sources/`. **Field reports** — anonymized real-world inspection findings — are a valid source type and are filed here like any other source, at Tier C. **Promotion trigger:** the same defect pattern (era + system + symptom) appearing in 3+ field reports updates the matching `03-domains/construction/` page with a field-confirmed note and typical-frequency data, at Tier C with an inline marker — mirroring the general atomicity "promote at 3+ mentions" rule. Field data never reaches Tier B without corroboration from a published source. A pattern seen fewer than 3 times stays noted only on the individual source's summary page, not promoted into domain claims.
5. Integrate: update every phase, platform, domain, and entity page the source touches. A good source touches 5–15 pages. On each touched page, recompute `tier_floor`, set `recheck` from the table above, and reset `review` to `unreviewed` if any claim materially changed — **an edit invalidates prior sign-off.** A reviewed page silently edited back to unreviewed status without the field flipping is the single most dangerous failure mode in this schema, because Exgest trusts that field.
6. **Contradiction triage.** Flag contradictions with a `> [!warning]` callout and never silently overwrite. Resolve by tier where tier permits:
   - Higher tier beats lower: the higher-tier claim stands in the page's prose, the lower-tier claim is preserved in the callout with its tier marked. No human needed. Log it.
   - Equal tier, both A: escalate to Paul. Both claims stay in the callout, neither in prose.
   - Equal tier, B or below: escalate only if the contradiction blocks a platform decision. Otherwise record both and mark the page `tier_floor: D` for that claim.
   - Newer beats older *only* at equal tier. A recent Tier C blog does not override a 2023 Tier A statute.
7. Update `index.md`.
8. Append to `log.md`: `## [YYYY-MM-DD] ingest | Source Title | tier: X` + 2–3 lines on what changed, including any tier movements and contradictions resolved by triage.

### Query

1. Read `Home.md` and `index.md`, drill into relevant pages, answer with wikilink citations.
2. **Cite the tier alongside the link.** An answer that reads as uniformly confident when it rests on a Tier C inference is a failure of the query operation, not a stylistic preference. Where the answer's weakest link is Tier C or D, say so in the answer itself.
3. If any page consulted has passed its recheck date, demote it, say so in the answer, and log the demotion.
4. If the answer is valuable (comparison, analysis, decision), file it in `06-syntheses/` and log it. A synthesis inherits the **lowest** tier of the pages it draws on — that is its `tier_floor`. Explorations must compound.

### Lint (periodic health check)

Structural checks: contradictions between pages, claims superseded by newer sources, orphan pages, a non-empty `07-inbox/`, concepts mentioned ≥3 times without their own page, pages that have accumulated a second concept and need splitting, stubs older than 30 days, missing legal-weapon tags on defect pages. `09-output/` is excluded from orphan checks — it is not part of the wiki graph.

Tier checks, run in the same pass:

- **Expired rechecks.** Any page past `recheck` — demote to Tier D, list them. This replaces the old manual "regulatory citations that need re-verification" check.
- **Ceiling violations.** Any page whose `tier_floor` is higher than the `tier:` of a source in its `sources:` list. This is the most common silent error and it always inflates confidence.
- **Floor drift.** Any page whose `tier_floor` does not match its weakest inline marker, or which carries no markers but a floor below A.
- **Unsourced claims.** Any quantitative threshold, legal citation, or date with no source page behind it. These are not Tier D, they are not claims — remove or source them.
- **Stale sign-off.** Any page with `review: reviewed` whose `updated` is later than `reviewed_on`. The edit invalidated the review.
- **Downstream exposure.** Any `09-output/` draft citing a page that has since been demoted or edited. List the affected drafts; they need regenerating before publication.
- **D-tier backlog.** Tier D claims older than 60 days that nobody has tried to verify. These are the wiki's honest to-do list and they should be shrinking.

Log the pass with counts per check, so tier health is trackable over time rather than assessed by vibe.

### Exgest (repurpose compiled wiki content into platform-facing drafts)

1. Input: target platform (`inspectos` | `homeos`) + format (pSEO page | lead-magnet PDF draft | social thread | email sequence).
2. Walk `Home.md` → relevant pages, filtering by `brand:` matching the target or `shared`.
3. **Apply the output gate before writing a word.** Per the permissions table above: Tier A and B reviewed claims go out plainly; Tier C goes out hedged and never as a bare number or legal assertion; Tier D never leaves the wiki; anything unreviewed carries a `> [!warning]` callout in the draft naming the specific claim and its tier. Do not average a page's claims — gate each claim on its own tier, which is why inline markers exist.
4. If a draft's central hook depends on a Tier C or D claim, **stop and say so** rather than writing around it. A lead magnet built on an unverified frequency statistic is a liability with a design brief attached.
5. **Repurposing rule:** a `shared`-brand page (or a page with claims useful to both platforms) may spawn two outputs from the same underlying facts, not one shared draft — voice and angle change per brand, the claims don't:
   - `inspectos` output: technical authority register, mechanism-first, field-tool and standard-citation heavy (matches the symptom-first convention).
   - `homeos` output: exposure/leverage register — what asymmetry the buyer didn't know they had, framed as risk-to-money translation, not mechanism.
   Both outputs cite the same source page(s) and carry the same tier markers and `> [!warning]` flags; only framing and vocabulary differ, never the underlying number, tier, or legal citation. **Register does not launder tier** — a Tier C claim written in the inspectos authority voice is still Tier C and still hedged.
6. Emit drafts to `09-output/{platform}/{format}/`. Each draft carries a frontmatter block listing every source page it drew on with that page's tier and `updated` date, so a later lint pass can detect when a draft has gone stale underneath. Never write to `raw/`, wiki pages, or `index.md` during Exgest.
7. Human reviews before anything is published.
8. Append to `log.md`: `## [YYYY-MM-DD] exgest | {platform} | {format} | {topic}` + the lowest tier the draft relies on.

---

## Known gaps (maintain this list)

- A third platform may be added to the venture later. Nothing exists for it now — do not create pages, tags, or speculation until human user defines it; when he does, add a platform page, extend the tag taxonomy, and update Home.md and platforms-overview.md.
- Prompt-chain source modules 1–6, 9, 11–12 are referenced but their full outputs are not yet in `raw/` — only the chain design and modules 7, 8, 10 excerpts.
- ~~No pricing/fee data for the inspection platform yet.~~ — superseded 2026-07-20: pricing data now exists but across four non-matching schemes (see the `> [!warning]` on `inspectos-pca-pcs-strategy.md`). **Try tier triage before escalating:** the four schemes almost certainly do not sit at the same tier, and under the contradiction rule a higher-tier scheme resolves against lower-tier ones without Paul's involvement. Tier the four sources first, then escalate only what survives as an equal-tier conflict.
- ~~Appendix C CPCV clause library~~ — done: ingested into `cpcv.md` on 2026-07-14.
- ~~Appendix A onboarding questionnaire / BRA template~~ — done: ingested into `client-onboarding-toolkit.md` on 2026-07-16.
- `PCA_Framework.md` and `PCS_Standard_Setting_Strategy_v2.md` — referenced extensively by `INTEGRATION_ANALYSIS.md` as the two most technically important documents in the InspectOS strategy corpus, but never supplied in `raw/`. If they arrive, they should substantially deepen `inspectos-pca-pcs-strategy.md` and `inspectos-iso17020-accreditation.md`. Until then, every claim in those pages sourced only to `INTEGRATION_ANALYSIS.md`'s *description* of the missing documents is Tier D by the ceiling rule — a summary of a document nobody has read is not evidence.
- Three unresolved contradictions from the 2026-07-20 InspectOS ingest, each flagged with `> [!warning]` on the relevant pages, none silently resolved. Re-run each through the tier triage in Ingest step 6 before treating it as blocked on Paul:
  1. DL 108/2026's specific mechanics differ between the legal impact-assessment source and the InspectOS strategy source. **Likely resolvable by tier** — the *Diário da República* text is Tier A and the strategy source is not.
  2. Employed vs. contractor inspector model conflicts between `hiring-compensation.md` and `inspectos-pca-pcs-strategy.md`. **Not resolvable by tier** — this is a business decision, not an evidence dispute. Genuinely needs Paul.
  3. At least four non-matching InspectOS pricing schemes across three source clusters. See the pricing gap above.
- **Tier backfill.** Every page predating this schema carries the old boolean `verified:` and no tier. They are not Tier A by default and must not be treated as such. Backfill on touch rather than in one sweep, prioritising: pages cited by existing `09-output/` drafts, then legal pages, then construction pages carrying quantitative thresholds. Track the remaining count in each lint log so the backlog is visible.
- Deliberately deferred (not gaps to close opportunistically — wait for explicit direction): regional dossiers for Silver Coast and Comporta/Alentejo; pSEO template mapping for Exgest (revisit once ~20 compiled pages exist); persona pages beyond the initial `d7-expat` seed.