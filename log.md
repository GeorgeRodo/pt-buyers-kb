---
title: Log
type: meta
tags: []
status: evergreen
created: 2026-07-13
updated: 2026-07-14
sources: []
brand: shared
verified: false
---

# Log

Append-only. Entry format: `## [YYYY-MM-DD] <ingest|query|lint|meta> | Title` — parseable via `grep "^## \[" log.md`.

## [2026-07-13] meta | Vault instantiated
Schema (CLAUDE.md), directory layout, tag taxonomy, and symptom-first convention established. Decomposition decision recorded in the synthesis "inspection-in-the-buyer-journey": buyer journey is the spine; platforms are views; home inspection files under Phase 4.

## [2026-07-13] ingest | Buyer's Agent Playbook Portugal 2026
Full structural extraction: 8 phase pages, agency platform page, market pages (intelligence, sourcing, comparables), CPCV, regional market sections, retention economics. Not yet extracted: Ch. 10 property-type deep dives, Ch. 11.8 fee models, Appendices B/C — logged in source page.

## [2026-07-13] ingest | 12-Module Construction Defects Prompt Chain
Extracted modules 7, 8, 10 and the strategy memo: 4 defect exemplar pages, condomínio law, DL 67/2023, DL 10/2024, regional geology, all 5 strategy pages, inspection platform page. Gap: full outputs of modules 1–6, 9, 11–12 not in raw/ — top expansion priority.

## [2026-07-13] lint | Initial pass
Known issues accepted at seed time: platform-3-tbd is a deliberate stub; porto dossier thin; defect backlog (carbonation, damp/thermal bridges, PB, aluminum wiring, ETICS, radon) listed in construction-defects-hub; IMT/tax figures carry annual re-verification warnings.

## [2026-07-13] meta | Platform 3 removed; article ingested
Platform 3 shelved per Paul ("not considering it right now"): stub page deleted, all references, tags, and diagram entries removed; CLAUDE.md notes only that a third platform may be defined later. Ingested "How to Create Your Own Knowledge Base with Obsidian" (S. Magdy, Medium 2025): adopted atomicity rule and inbox convention into CLAUDE.md; source summary filed; raw copy saved.

## [2026-07-13] lint | Second pass
Structure, frontmatter, links, and tags checked across all 39 pages. Fixed: instagram-renovation-detection.md was missing its dl-67-2023 legal-weapon tag despite naming it as the weapon in the header block. Flagged for Paul: RCAAP is defined in entities-hub.md as an academic open-access repository, but phase-4-due-diligence.md and sops.md both cite "RCAAP/licensing checks" as a per-property desktop-audit step — these can't both be right, likely a mislabeled source registry. Promotion candidates: AL/Alojamento Local licensing (RNAAL, containment zones) is cited across 8+ pages with no dedicated page; Registo Predial cited 3x with only a one-liner in entities-hub. No orphans, no broken links, no stale stubs (all pages dated today), inbox empty of unfiled material.

## [2026-07-14] ingest | Buyer's Agent Playbook Portugal 2026 (second pass — gap closure)
Closed the three gaps flagged at first ingest. New pages: property-types-hub.md + six type pages (historical, new-build/off-plan, land/development, luxury, resale/traditional, rural/quinta) under 03-domains/market/; agency-checklists.md under 05-strategy/ (Appendix B viewing/DD/pre-closing/handover/snagging/off-plan checklists). Updated: cpcv.md (Appendix C.3 ten-clause library), platform-buyers-agency.md (§11.8 fee-setting/collection discipline; corrected a stale "seven type playbooks incl. high-yield" claim to the actual six), phase-2/3/4/7/8 pages (links to new property-type and checklist pages). Flagged, not resolved: playbook Appendix C.4 gives a >5% area-discrepancy threshold where phase-4-due-diligence.md (fed by the construction-defects-prompt-chain source) gives >2% for the same check — warning callouts added to both cpcv.md and phase-4-due-diligence.md pending Paul's call on which applies where. Not filed: Appendix C.1/C.2/C.5 sample scripts (illustrative, lower priority) and Appendix A field-by-field structure (still only referenced, not transcribed).

## [2026-07-14] schema-review | Paul feedback round 1
CLAUDE.md updated: added mandatory `brand:`/`verified:` frontmatter fields, a Persona tag tier and `competitor` tag, `08-personas/` (type: persona) and `09-output/` (Exgest artifacts, excluded from lint) to the directory layout, a new Exgest operation, and a GDPR-anonymization precondition plus field-report source type on Ingest. Known gaps list refreshed: CPCV clause library marked done, Silver Coast/Comporta dossiers and pSEO template mapping and extra personas moved to deliberately-deferred. Propagated: added `brand`/`verified: false` to all 53 existing wiki pages (conservative inspectos/homeos/shared split, no content changes); created 08-personas/personas-hub.md and the d7-expat seed persona; updated Home.md and index.md for the new folders/pages.

## [2026-07-14] schema-review | Paul feedback round 2
Second Paul review confirmed round 1's brand/persona/competitor/verification/GDPR/Exgest additions already covered most of his asks — no rework needed there. Three genuinely new items added to CLAUDE.md: (1) Ingest field-report step now has an explicit promotion trigger — a defect pattern recurring in 3+ anonymized field reports updates the matching 03-domains/construction/ page, mirroring the existing atomicity "promote at 3+" rule. (2) Exgest gained a content-repurposing rule: a shared-brand or dual-relevant page can spawn separate inspectos (technical-authority) and homeos (asymmetry/leverage) outputs from the same underlying claims — voice differs, the cited numbers and legal citations never do. (3) Filed 06-syntheses/municipal-variance-and-the-thesis.md answering Paul's Câmara-variance question: the thesis rests on information asymmetry, not on the three founding decrees being an exhaustive account of the market — municipal variance is regional-dossier operational detail, not a caveat on Home.md's framing. pSEO template mapping deliberately left deferred per existing known-gaps note.

## [2026-07-14] lint | Cleanup pass (task-list items 3–5)
Three items closed from the standing task list. (1) property-types-hub.md: removed the stale `> [!warning]` about platform-buyers-agency.md's "seven types incl. high-yield" claim, since that page was already corrected 2026-07-14 — replaced with a plain changelog note. (2) porto.md: expanded using previously-unmined regional data already sitting in raw/buyers-agent-playbook-portugal-2026.md §3.1.2 and §11.2 (city vs. metro demand/supply/price split, gaioleiro structural type, domestic/foreign demand balance) — no new source needed, this was ingest debt from the first pass. Removed the "thinnest dossier" status line; updated index.md's Porto entry to match. (3) Promoted two concepts past the atomicity 3+ threshold to full pages under 04-entities/: alojamento-local.md (AL/RNAAL licensing, containment zones, post-Mais Habitação regime, the licence-non-transfer warning) and registo-predial.md (certidão predial vs. caderneta predial distinction, title-defect DD role, houses the area-discrepancy 2%/5% conflict detail). entities-hub.md and index.md updated to link both; cpcv.md's existing warning callout now points to registo-predial.md for the fuller reconciliation note. RCAAP mislabeling (item 2 on the standing list) and the 2%/5% threshold conflict itself (item 1) remain open, both still awaiting Paul's call.
