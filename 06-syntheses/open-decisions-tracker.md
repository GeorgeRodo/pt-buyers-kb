---
title: Open Decisions Tracker — Unresolved Contradictions & Calls Needed
type: synthesis
tags: [dl-108-2026, dl-10-2024, inspection]
status: draft
created: 2026-07-20
updated: 2026-07-23
sources: [src-dl-108-2026-impact-assessment, src-inspectos-strategy-technical, src-inspectos-talent-master-plan, src-buyers-agent-playbook-2026, src-construction-defects-prompt-chain]
brand: shared
verified: false
---

# Open decisions tracker

**The question:** across lint passes and ingests, several genuine contradictions and unresolved calls have accumulated in the source material — each individually flagged with a `> [!warning]` on its own page, but nowhere collected in one place. This page is that place: a living list, updated as items close, so open decisions persist across sessions instead of living only in chat history and scattered log entries.

**Rule for maintainers:** when an item below is resolved, don't delete it — mark it resolved (strikethrough the summary, keep the entry, note the resolution and date), the way `AGENTS.md`'s own known-gaps list handles closed items. This page should always show its own history.

## Open

### 1. InspectOS pricing — four non-matching schemes
No single InspectOS price for a given service can be trusted without checking which scheme it came from: the granular "Pricing Master v2" per-service table, the Year 2 Essential €495/Professional €695/Premium €995 consumer tiers, the B2B brochure pricing by property size (T1/T2 €195–295 up to Commercial €495–995), and a separately-cited "starting at €980" snagging price. The source material itself acknowledges this is unreconciled. **Blocks:** any client-facing pricing content for the inspection platform. Detail: [[inspectos-pca-pcs-strategy]].

### 2. Inspector employment model — employed vs. contractor
The InspectOS strategy corpus states the employed-inspector model is "non-negotiable" (for ISO 17020 Type A independence and PCS data-consistency reasons). The entire hiring/ops corpus — sourcing, compensation, quality gates, onboarding — is built around contractors (recibo verde) as the primary capacity mechanism, with only 1–2 full-time seniors as an "anchor." These are two different operating models with different cost structures, not a terminology gap. **Blocks:** the hiring-cluster cost projections in [[hiring-90day-roadmap]] and [[hiring-non-inspector-roles]], which assume the contractor model. Detail: [[inspectos-pca-pcs-strategy]] vs. [[hiring-compensation]].

### 3. DL 108/2026 — mechanics discrepancy between sources
The two-document legal impact assessment ([[dl-108-2026]]) and the InspectOS strategy corpus give different specific figures for the same law: the strategy corpus cites a flat €25,000 IMPIC fine threshold and uncapped 10-year seller liability; the legal-impact-assessment sources describe solidary-liability fines up to €450,000, a 1-year buyer annulment window, and an existing (not new) €150,000 agent insurance minimum frozen since 2013. **Blocks:** any client-facing summary of what DL 108/2026 actually does. Detail: [[dl-108-2026]].

### 4. Area-discrepancy threshold — 2% vs. 5%
The prompt-chain source's registry cross-check flags area discrepancies at >2%; the playbook source's Appendix C.4 CPCV-stage red flag uses >5% for what appears to be the same unpermitted-alteration check. Open since 2026-07-14, untouched since. **Blocks:** a precise, citable number for the [[phase-4-due-diligence|Phase 4 desktop audit]] and [[cpcv|CPCV red-flag]] checklists. Detail: [[cpcv]], [[registo-predial]].

### 5. RCAAP mislabeling
`entities-hub.md` defines RCAAP as Portugal's academic open-access research repository; [[phase-4-due-diligence]] and [[sops]] both cite "RCAAP/licensing checks" as a per-property desktop-audit step. These can't both be the same RCAAP — likely a mislabeled registry in the original source material. Open since 2026-07-14, untouched since. **Blocks:** correcting whichever page has the wrong registry name.

### 6. Strategic framing — is PCG/PCA/PCS the story we're telling?
The InspectOS strategy corpus reframes the inspection platform from "forensic due-diligence add-on to the buyer journey" to a three-tier Property Condition Gap → Property Condition Assessment → Property Condition Score infrastructure/standard-setting play, aimed at eventually selling proprietary risk data to banks and insurers across Southern Europe. This is a real strategic choice arriving via source material, not a decision made deliberately in this KB. Needs a call on whether [[platform-home-inspection]]'s core positioning should adopt this framing, stay with the narrower due-diligence framing, or hold both (aspirational infrastructure play vs. near-term product) explicitly labeled as such. Detail: [[inspectos-pca-pcs-strategy]].

## Process note (not a content decision)

All 92 pages in this KB carry `verified: false` — no human domain expert has signed off on any page's technical or legal claims. Per `AGENTS.md`, pages with `verified: false` must never be used verbatim in a client-facing inspection report. This isn't a contradiction to resolve, just the standing gate between "internally coherent wiki" and "usable client-facing content" — worth keeping in view as items above get closed, since resolving a contradiction doesn't itself constitute verification.

Up: [[syntheses-hub]] · Related: [[dl-108-2026]], [[inspectos-pca-pcs-strategy]], [[hiring-compensation]], [[cpcv]]
