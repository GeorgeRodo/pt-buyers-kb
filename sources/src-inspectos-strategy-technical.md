---
title: "Source: InspectOS Strategy & Technical Corpus (FAIRBANK Group)"
type: source
tags: [inspection, dl-10-2024, dl-108-2026]
status: evergreen
created: 2026-07-20
updated: 2026-07-20
sources: []
brand: inspectos
verified: false
---

# Source — InspectOS strategy & technical corpus

**Raw files:** `InspectOS_Business_Strategy_2026_2031.md` (canonical — see below) · `InspectOS_ISO_17020_Alignment.md` · `InspectOS_Inspector_App_R&D_Plan (1).md` · `inspectos_technical_scope_technology_report (1).md` · `InspectOS_Brochure_Mediators.md` · `InspectOS_Brochure_MortgageBrokers.md` · `INTEGRATION_ANALYSIS.md` · `InspectOS_Post_August_3_Strategy_Report_REVISED.md` · **Ingested:** 2026-07-20.

## What it is

A founder-level strategy and technical-planning corpus for InspectOS, prepared by "FAIRBANK Group" (named as InspectOS's parent/consulting entity throughout — first appearance in this KB). These documents reveal a substantially more ambitious and differently-branded venture than the earlier `src-construction-defects-prompt-chain` and `src-buyers-agent-playbook-2026` sources described: not "home inspection" but a three-tier **Property Condition Gap (PCG) → Property Condition Assessment (PCA) → Property Condition Score (PCS)** infrastructure play, with PCA as an open, ISO/IEC 17020:2026-aligned standard and PCS as a proprietary B2B risk-scoring database sold to banks and insurers.

**Canonicity note:** `InspectOS_Business_Strategy_2026_2031.md` explicitly states it is "the single authoritative source of InspectOS strategy" and "supersedes prior strategy documents, including TCS_Standard_Setting_Strategy.md (deprecated), the Post-August 3 Strategy Report, and the original First Mover Defense." This KB treats it accordingly: `InspectOS_Post_August_3_Strategy_Report_REVISED.md` was scanned for consistency but not separately extracted, since the Business Strategy document supersedes it. `INTEGRATION_ANALYSIS.md` is a meta-document mapping a 24-document portfolio, most of which (documents #1–21, including `PCA_Framework.md` and `PCS_Standard_Setting_Strategy_v2.md`, the two documents it discusses most) is **not present in `raw/`** — only the integration-analysis document itself was ingested, as a map of what's missing, not as primary content.

## Core claims

- **Three-tier architecture:** PCG (narrative/market-education, not a product) → PCA (open, vendor-neutral, ISO 17020:2026-aligned inspection methodology, seven dimensions) → PCS (proprietary 0–100 + letter-grade score, six weighted dimensions, InspectOS's actual moat). See [[inspectos-pca-pcs-strategy]].
- **DL 108/2026 (3 August 2026) is named as the direct commercial launch catalyst** — independently corroborating this KB's own [[dl-108-2026]] research, though this source's account of the decree's specifics (€25,000 IMPIC fine threshold, 10-year uncapped seller liability, €150,000 professional indemnity minimum) does not fully match the numbers in [[src-dl-108-2026-impact-assessment]] — see the warning on [[inspectos-pca-pcs-strategy]].
- **ISO/IEC 17020:2026 Type A accreditation via IPAC** is treated as the structural prerequisite for everything else — a 15-month, non-shortcuttable process that becomes the primary competitive moat against later entrants. See [[inspectos-iso17020-accreditation]].
- **Employed-inspector model, stated as "non-negotiable"** — directly conflicting with the contractor-centric model in [[hiring-compensation]] and [[hiring-quality-gates]] from the separately-ingested `src-inspectos-talent-master-plan`. Flagged, not resolved — see the warning on [[inspectos-pca-pcs-strategy]].
- **Two-entity legal structure** (locked decision): `InspectOS Avaliações, Lda.` (the accredited inspection body) and `InspectOS Tecnologia, Lda.` (the PCS data platform), both under FAIRBANK Group, separated specifically to satisfy ISO 17020 Type A independence.
- **Pricing is internally unreconciled across sources** — three different, non-matching pricing schemes appear across this cluster (the "Pricing Master v2" service-by-service table, the Year 2 Essential/Professional/Premium tiers, and the B2B brochure pricing for mediators/mortgage brokers). The Business Strategy document itself flags this as unresolved. See [[inspectos-pca-pcs-strategy]].
- **Inspector App R&D plan**: competitive analysis against Spectora, Property Inspect, Inspecto, WeProov and others; EU AI Act risk-classification of inspection AI features (photo defect detection = limited risk, bank/insurer risk-scoring = high risk under Annex III). See [[inspectos-inspector-app]].
- **International technical-scope benchmarking**: UK RICS three-level survey standard, France's mandatory seller-funded DDT, Spain's building-only ITE, Netherlands' lender-driven inspection, Germany's engineer-led Baugutachten — used to argue Portugal has no equivalent unit-level mandatory inspection and to design InspectOS's own service tiers. See [[inspectos-technical-scope-benchmarks]].

## Why this matters

This is a significant scope expansion for the inspection platform's ambition — from "forensic due-diligence add-on to the buyer journey" to "the infrastructure standard for property condition data in Southern Europe, selling into banks and insurers." It doesn't replace the buyer-journey framing this KB is built around, but it substantially deepens [[platform-home-inspection]] and introduces real internal contradictions (pricing, employment model) against material already in the wiki that need a human call, not a wiki-maintainer guess.

## Integrated into

[[platform-home-inspection]] (updated with warnings) · [[inspectos-pca-pcs-strategy]] (new) · [[inspectos-iso17020-accreditation]] (new) · [[inspectos-inspector-app]] (new) · [[inspectos-technical-scope-benchmarks]] (new) · [[hiring-compensation]] and [[hiring-quality-gates]] (cross-referenced for the employment-model conflict)

## Not yet extracted

`PCA_Framework.md` and `PCS_Standard_Setting_Strategy_v2.md` — the two source documents `INTEGRATION_ANALYSIS.md` treats as the most technically important in the whole portfolio — are referenced extensively but were never supplied in `raw/`. If they arrive, they should substantially deepen [[inspectos-pca-pcs-strategy]] and [[inspectos-iso17020-accreditation]]. `InspectOS_Post_August_3_Strategy_Report_REVISED.md` was not separately extracted (superseded per the canonicity note above) — if Paul wants its specific "Post-August-3 activation sprint" tactical detail preserved despite the supersession, flag it for a follow-up pass.
