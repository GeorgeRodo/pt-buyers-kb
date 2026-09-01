---
title: InspectOS Inspector App — R&D Plan
type: concept
tags: [inspection]
status: draft
created: 2026-07-20
updated: 2026-07-20
sources: [src-inspectos-strategy-technical]
brand: inspectos
verified: false
---

# The inspector app — field operating system, not a report writer

Core thesis: the mobile app isn't a documentation tool bolted onto the inspection service, it's the data-collection engine for the entire [[inspectos-pca-pcs-strategy|PCS database]] — it enforces methodology consistency (which is what makes PCS scores comparable across inspectors) and captures structured data at the point of inspection rather than after the fact.

## Competitive landscape (June 2026)

No existing inspection-software competitor combines an open methodology, a proprietary scoring database, EU regulatory alignment, and AI-native field capture. Spectora dominates US mindshare but has no API and is English-only. Property Inspect is the closest European analog (200+ templates, offline mobile, "Inspect AI" launched 2026) but has a complex setup and no video AI. Inspecto (UK, 2024) is the most AI-native — it replaces manual photography with video walkthroughs that AI parses frame-by-frame — but is UK rental-only. WeProov is EU-based (France/Spain) but limited to damage documentation with no deep regulatory alignment. Across all evaluated "AI inspection" vendors, only 4 of 12 actually perform automated damage detection (baseline photo/video comparison flagging new damage) — the rest are documentation tools marketed as AI.

InspectOS's differentiation target: an open PCA methodology paired with proprietary PCS scoring (versus competitors' closed proprietary templates), Portugal-specific regulatory alignment (Simplex, EPC, seismic, BRP) that's EU-expandable, multi-modal AI (photo defect detection + voice-to-text + predictive risk scoring + baseline comparison, versus competitors' single-mode AI), and a platform built for ISO 17020:2026 Type A accreditation from the start rather than software-only.

## EU AI Act compliance architecture

High-risk requirements under the EU AI Act apply from August 2026, directly affecting how InspectOS can deploy AI in the app:

| AI use case | Risk class | Requirement |
|---|---|---|
| Photo defect detection / annotation | Limited | Transparency disclosure, human inspector reviews every finding |
| Automated condition scoring for buyer reports | Limited | Documented as a preparatory task to human assessment |
| Risk scoring for bank/insurer underwriting | **High** (Annex III) | Full conformity assessment, technical documentation, human oversight, post-market monitoring, EU database registration |
| Predictive maintenance from PCS trend data | Minimal | Existing legislation only |

The stated strategy is a "human-AI partnership" model — AI suggests, the inspector confirms, every AI-flagged finding requires human sign-off before entering a report — with the PCS analytics module sold to banks and insurers treated as full high-risk compliance scope, distinct from the lower-risk field-capture features.

## Regulatory grounding this app is built against

DL 10/2024's removal of the habitation license, [[dl-108-2026|DL 108/2026]]'s August 2026 activation of agent liability, and ISO/IEC 17020:2026's March 2026 publication (simplified to a Type A / Type non-A independence model, with explicit provisions for digital transformation and remote inspection) are treated as the three converging regulatory forces the app architecture is designed around — a QMS engine (competence tracking, calibration records, audit trails, complaints module) built into the software from day one, not bolted on before an IPAC assessment.

See [[inspectos-pca-pcs-strategy]] for the business strategy this product serves, [[inspectos-technical-scope-benchmarks]] for the international standards the app's checklist design draws on.
