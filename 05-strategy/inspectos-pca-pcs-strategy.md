---
title: "InspectOS Strategy — PCG, PCA & PCS (the Three-Tier Architecture)"
type: concept
tags: [inspection, dl-10-2024, dl-108-2026]
status: draft
created: 2026-07-20
updated: 2026-07-20
sources: [src-inspectos-strategy-technical]
brand: inspectos
verified: false
---

# The three-tier architecture: PCG → PCA → PCS

InspectOS's canonical strategy (per `InspectOS_Business_Strategy_2026_2031.md`, explicitly the authoritative document over all prior strategy drafts) reframes the inspection platform as an infrastructure play, not a service business. Locked terminology — **never** substitute TCS, True Condition Score, RGS, or other deprecated terms:

- **Property Condition Gap (PCG)** — the market problem: the unmeasured distance between documented and physical property reality. A narrative/education campaign, not a product; InspectOS doesn't charge for it or own it.
- **Property Condition Assessment (PCA)** — the inspection methodology itself. Deliberately **open and vendor-neutral**, ISO/IEC 17020:2026-aligned, so professional bodies and regulators can endorse or mandate it without appearing to endorse a single company. Seven assessment dimensions: structural condition, MEP systems, building envelope, life safety, code compliance, maintenance status, environmental (moisture/mold/radon).
- **Property Condition Score (PCS)** — the proprietary output: a 0–100 numeric score (B2B-facing, feeds actuarial/underwriting models) plus a PCS-A to PCS-F letter grade (consumer-facing), six weighted dimensions (structural 25%, MEP 25%, envelope 20%, life safety 15%, deferred maintenance 10%, systems obsolescence 5%). Every PCA — whether InspectOS's own or an OE-PCA-certified competitor's — can feed the PCS database if submitted through InspectOS's platform. This is the actual moat: "open the railroad, own the tollbooth."

## Why now — the window

DL 10/2024 removed the pre-sale habitation license entirely; the strategy names **[[dl-108-2026|DL 108/2026]], effective 3 August 2026,** as the direct commercial launch catalyst — the point where agent liability for undocumented condition becomes acute and demand for third-party verification becomes urgent rather than optional. The strategic window is framed as roughly 24 months (August 2026 to Q4 2028–Q1 2029), between "agent fear" and the first wave of court precedent making verification effectively mandatory — after which competitors will have caught up and the standard-setting opportunity closes.

> [!warning] This source's account of DL 108/2026's specific mechanics (a flat €25,000 IMPIC fine threshold, uncapped 10-year seller liability, a €150,000 professional indemnity minimum for agents) does not fully match the figures in [[dl-108-2026]], sourced from two independent, more detailed impact-assessment documents (which describe fines up to €450,000 for solidary-liability infractions, a 1-year buyer annulment window rather than a flat 10-year liability figure, and an existing — not new — €150,000 agent insurance minimum that's been frozen since 2013). Both sources agree DL 108/2026 is the key catalyst; the specific numbers need reconciliation before either is used in a client-facing context.

## Standard-setting: five pathways, run in parallel

**Pathway A.0 — ISO 17020:2026 / IPAC accreditation** (prerequisite for all others; see [[inspectos-iso17020-accreditation]]). **Pathway A — OE endorsement**: InspectOS doesn't certify engineers, it certifies a three-tier PCA-I (trainee, supervised only) / PCA-II (authorized, independent) / PCA-III (senior, 5+ years) practitioner overlay on top of existing OE membership — positioned as complementary to OE authority, not competing with it. **Pathway B — regulatory reference**: getting IMPIC to cite PCA documentation as evidence of agent due diligence (a 12–18 month relationship-building process, not a legislative campaign) and Banco de Portugal to treat PCS as a macroprudential collateral-quality signal. **Pathway C — insurance underwriting integration**: judged "the deepest moat" — once an insurer's underwriting systems and claims workflows reference PCS data, switching cost becomes structural, not just competitive. **Pathway D — European harmonization** (2030+, contingent on the other four succeeding first): Portugal establishes a national IPQ standard, then pushes for CEN working-group adoption.

The standard is considered "won" when 3 of 5 conditions are met: 5,000+ verified PCS scores in the database, one regulatory body referencing PCA in supervisory guidance, one major insurer requiring PCA certification for liability pricing, OE recognizing PCA in its professional development curriculum, and 100+ notaries regularly attaching PCA reports to deeds.

## Employed-inspector model

The strategy states InspectOS employs inspectors rather than contracting them, calling this **"non-negotiable"** for two reasons: ISO 17020 Type A independence is harder to demonstrate for contractors who may have other financial relationships with property owners or developers, and data consistency for the PCS scoring model depends on inspectors trained on one calibrated protocol rather than mixed contractor methodology. Stated inspector economics: base salary €28,000–€32,000, per-inspection bonus €15–€25, equipment provided.

> [!warning] This directly conflicts with [[hiring-compensation]] and [[hiring-quality-gates]] (from the separately-ingested `src-inspectos-talent-master-plan`), which build the entire inspector-sourcing model around contractors (recibo verde) as "InspectOS's primary capacity-scaling mechanism," with only 1–2 full-time senior inspectors as an "anchor." The two source documents describe genuinely different operating models — not a minor terminology gap. Unresolved; flagging per the ingest convention rather than picking one silently. Whichever model is correct materially changes the entire hiring-cluster cost structure in [[hiring-90day-roadmap]].

## Pricing — internally unreconciled

Three non-matching pricing schemes appear across this source cluster: (1) a granular "Pricing Master v2" service-by-service table (Gas Inspection €75 up to Full Bundle €4,295, Pre-Purchase PCA €550); (2) Year 2 consumer tiers — Essential €495 (5 dimensions), Professional €695 (7 dimensions + bilingual report), Premium €995 (7 dimensions + environmental sampling + thermal imaging + video); (3) the B2B brochure pricing for mediators/mortgage brokers, structured by property size instead of tier — T1/T2 €195–295 up to Commercial €495–995. The financial model's unit economics (€225 gross profit at 37.8% margin) are calculated on a €595 bundled base case that doesn't cleanly map to any of the three schemes above. The source document itself flags this: "These need to be reconciled into a unified pricing document before commercial launch." Treat as unresolved — do not quote a single InspectOS price point without checking which scheme it came from.

## Financial shape (five-year projection, base case)

3,000 inspections in Year 1 rising to 40,000 by Year 5; total revenue €1.61M → €36.80M; blended gross margin 51.6% → 67.7% as B2B/API revenue (80–85% margin) and ESG/institutional revenue (85–90% margin) grow to dominate the mix over pure inspection revenue (~38% margin). Break-even projected Month 20. Capital plan: €500,000 pre-seed (June 2026) → €200K–400K bridge → €2M–4M Series A (Q3 2027–Q1 2028, funds Spain scouting) → €5M–10M Series B (2029+, European expansion).

## Competitive strategy

Threat arrives in three waves: domestic competitors (2027, easiest to defend against once IPAC accreditation is underway and 5,000+ scores exist), French/German diagnostic firms with existing European infrastructure (2028, the dangerous wave), and PE-backed consolidation plays (2029+, framed as acquisition targets rather than existential threats). Four preemptive moves: publish the PCA methodology openly before competitors arrive (any later entrant either adopts InspectOS's standard, enriching its database, or fights an open standard — commercially irrational); lock in the OE working-group relationship first; sign the first insurer pilot before claims data becomes public (a 2.5-year head start given insurance pilots need 12–18 months of loss-ratio data before rollout); and file trademarks immediately (InspectOS, PCA, PCS, Property Condition Gap — before any strategy document becomes public).

See [[inspectos-iso17020-accreditation]] for the accreditation mechanics this whole strategy depends on, [[platform-home-inspection]] for how this integrates with the buyer-journey framing, [[hiring-hub]] for the conflicting inspector-employment model.
