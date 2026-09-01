---
title: InspectOS Compensation & Contracts Architecture
type: concept
tags: [inspection]
status: draft
created: 2026-07-20
updated: 2026-07-20
sources: [src-inspectos-talent-master-plan]
brand: inspectos
verified: false
---

# Compensation & contracts architecture

Four inspector profiles, each with a distinct contract logic: full-time senior engineers (the quality anchor), contractors (the capacity-scaling mechanism), Brazilian transfers (trainee-then-convert, gated by OEP registration timing), and interns (government-subsidized pipeline).

## Full-time senior inspector

Base salary €35,000–€50,000 gross (14 payments), with meal, vehicle/fuel, and phone allowances bringing total cash compensation to roughly €40,000–€60,000 depending on city. Total employer cost at a €45,000 gross base is **€67,000–€72,000/year** once employer social security (23.75%), work-accident insurance (~1.5%), and the allowance stack are added — the gap between gross salary and true cost is the number to plan around, not the headline figure. Incentives are deliberately hybrid (volume + quality, with quality weighted ≥40% of incentive potential) to avoid rewarding rushed inspections.

## Contractor (recibo verde)

Per-inspection rate €200–€450 depending on property complexity, against InspectOS's own €595–€850+ pricing — a 50–66% margin on standard jobs. The Portuguese freelancer tax regime makes this unusually favorable in Year 1: a contractor invoicing €40,000/year pays an effective tax rate of just **3.7% in Year 1** (50% IRS coefficient reduction + 12-month social-security exemption for new freelancers), rising to ~21% in Year 2 and ~28% in Year 3+ as the exemptions expire. InspectOS's own cost is simpler: no employer social security, no allowances, just the invoice amount minus 23% withholding tax remitted to the tax authority.

## Brazilian relocation package

Structured as a 90-day risk-minimization ramp: Days 1–30 trainee (IEFP stipend or private trainee pay, OEP registration submitted within 14 days of arrival), Days 31–60 supervised contractor work, Days 61–90 full contractor/employee conversion. Relocation costs (flight reimbursement, temporary housing stipend, OE fee sponsorship) are clawed back if the candidate leaves within 6 months — except the housing stipend, which is forgivable.

## Intern (IEFP +Talento)

€1,057/month gross stipend for a Master's-level intern, 65–80% reimbursed by IEFP — net cost to InspectOS is €211–€370/month for a 6-month, non-renewable placement. The value curve is explicitly front-loaded negative (Months 1–2: shadowing, net cost) and back-loaded positive (Months 4–6: independent inspections, net contribution).

## Contract type decision matrix

| Scenario | Contract type | Key clauses |
|---|---|---|
| Senior anchor inspector | Full-time (CDI) | OE verification, insurance, non-compete, IP, 90-day probation |
| Flexible capacity inspector | Recibo verde | Service agreement, quality SLA, per-inspection rate |
| Brazilian, OEP pending | Trainee/IEFP internship | Conversion trigger, clawback, supervision requirements |
| Angolan support engineer | Service agreement | Supervision ratio, no independent signing authority |
| University intern | IEFP internship agreement | 6-month duration, conversion pathway |

Non-compete clauses on employment contracts are capped at 12 months under Portuguese labor law with compensation required during the restriction; contractor agreements carry a lighter 6-month client-non-solicitation term with no compensation owed. Quality SLA: 48-hour report delivery, ≥80% average audit score, three substantiated client complaints in six months triggers corrective action.

See [[hiring-talent-market]] for the market rates this is benchmarked against, [[hiring-onboarding-retention]] for the career ladder these figures feed into, [[hiring-quality-gates]] for the insurance/liability structure each contract type inherits.

> [!warning] This contractor-centric model conflicts with [[inspectos-pca-pcs-strategy]] (from the separately-ingested `src-inspectos-strategy-technical`), which states InspectOS employs inspectors and calls the employed model "non-negotiable" for ISO 17020 Type A independence and PCS data-consistency reasons. Unresolved — see that page's warning for detail.
