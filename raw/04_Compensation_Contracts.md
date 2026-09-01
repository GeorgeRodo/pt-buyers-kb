# InspectOS Compensation & Contracts Architecture

## TL;DR

This document architects the complete compensation framework for InspectOS's four inspector profiles: **full-time senior engineers** (€35,000–€50,000 gross annual, 14 payments), **contractors** (€250–€350/day or €200–€300 per inspection), **Brazilian transfers** (trainee at IEFP stipend rates during OEP processing, then converted to full pay), and **interns** (€1,057/month Master's IEFP stipend, 65–80% reimbursed by government). [^67^][^122^] The total employer cost for a full-time senior inspector at €45,000 gross is **€57,375** (including 23.75% employer social security + ~1.5% work accident insurance). [^128^][^131^] Contractor economics are highly favorable for both parties: under the simplified regime, a contractor invoicing €40,000/year pays effective tax of only **6.6%** in Year 1 (due to the 50% IRS coefficient reduction and 12-month social security exemption), yielding **€56,053 net** versus **€39,360** in Year 3+. [^123^] The **Contract Type Decision Matrix** guides when to use each arrangement: full-time employment for the anchor senior inspector role, recibo verde (green receipt) contracting for flexible capacity, interim trainee agreements for Brazilian candidates pending OEP admission, and IEFP internship agreements for university pipeline candidates. Every contract template includes OE compliance clauses, quality SLAs, and non-compete provisions adapted to Portuguese labor law.

---

## 1. Full-Time Senior Inspector Package

### 1.1 Base Salary Structure

The full-time senior inspector is InspectOS's **quality anchor** — an OE-registered civil engineer with signing authority who provides technical leadership, quality oversight, and court-admissible report validation. This role is essential for InspectOS's credibility and regulatory compliance. The compensation must be competitive with construction firms and utilities while remaining sustainable for a pre-seed proptech startup.

| **Component** | **Lisbon** | **Porto** | **Remote/Other** |
|---|---|---|---|
| **Base Salary (gross, 14 payments)** | €38,000 – €50,000 | €35,000 – €45,000 | €32,000 – €42,000 |
| **Meal Allowance** | €300 – €350/month (card) [^41^] | €280 – €320/month (card) | €280 – €320/month (card) |
| **Vehicle/Fuel Allowance** | €400 – €500/month OR company vehicle | €350 – €450/month OR company vehicle | €400 – €500/month (essential for field work) |
| **Phone/Internet** | €50 – €70/month | €50 – €70/month | €50 – €70/month |
| **Total Cash Compensation** | €46,600 – €60,200 | €43,160 – €54,840 | €40,160 – €51,840 |

The Lisbon premium of approximately **8–12%** over Porto reflects the higher cost of living and more competitive talent market in the capital. [^41^] The remote/other category applies to inspectors based in secondary cities (Coimbra, Braga, Aveiro) who cover their respective regions.

### 1.2 Performance Incentives

| **Incentive Type** | **Structure** | **Expected Annual Value** | **Rationale** |
|---|---|---|---|
| **Volume Bonus** | €25 per inspection above 15/month | €1,800 – €3,600 | Rewards productivity without compromising quality |
| **Quality Score Bonus** | €100–€200/month for audit scores ≥90% | €1,200 – €2,400 | Reinforces report quality and attention to detail |
| **Client Satisfaction Bonus** | €50 per inspection with 5-star client rating | €600 – €1,200 | Aligns inspector behavior with client experience |
| **Referral Bonus** | €500 per successfully hired referred inspector | Variable | Activates employee as talent scout |

The incentive structure is deliberately **hybrid** (volume + quality) to prevent the perverse incentive of rushing inspections to maximize volume. The quality score bonus (based on random audit results) should represent at least **40% of total incentive potential** to signal that InspectOS prioritizes accuracy over speed.

### 1.3 Benefits Stack

| **Benefit** | **Standard Offering** | **Cost to InspectOS** | **Notes** |
|---|---|---|---|
| **Health Insurance** | Subsídio de saúde: €50–€100/month toward private plan | €600 – €1,200/year | Complements public SNS; valued by employees |
| **Pension Contribution** | Employer contribution to complementar pension plan | 3–6% of salary | Optional but appreciated; tax-advantaged |
| **Professional Development** | OE continuing education credits, conference attendance | €1,000 – €1,500/year | Mandatory for OE title maintenance; also builds expertise |
| **Remote Work Flexibility** | 2–3 days/week office-optional after 6 months | €0 | Highly valued post-COVID; field work naturally hybrid |
| **Flexible Hours** | Core hours 10:00–16:00; inspection scheduling flexible | €0 | Essential for field-based role |
| **Holiday Allowance** | 14th month (subsídio de férias) — legally required [^41^] | Built into 14-payment structure | Portuguese standard; non-negotiable |
| **Christmas Allowance** | 13th month (subsídio de Natal) — legally required [^41^] | Built into 14-payment structure | Portuguese standard; non-negotiable |

### 1.4 Employer Cost Calculation

For a senior inspector hired at **€45,000 gross annual** (14 payments of €3,214) in Lisbon, the total employer cost is: [^128^][^131^]

| **Cost Component** | **Calculation** | **Annual Cost** |
|---|---|---|
| Gross Salary | €45,000 | €45,000 |
| Employer Social Security (23.75%) | €45,000 × 0.2375 | €10,688 |
| Work Accident Insurance (~1.5%) | €45,000 × 0.015 | €675 |
| Meal Allowance (€10.20/day × 22 days × 12 months) [^48^] | €10.20 × 264 | €2,693 |
| Vehicle Allowance | €450 × 12 | €5,400 |
| Phone/Internet | €60 × 12 | €720 |
| Health Subsidy | €75 × 12 | €900 |
| Professional Development Budget | | €1,200 |
| **Total Annual Employer Cost** | | **€67,276** |
| **Total with Volume/Quality Incentives (target)** | | **€70,000 – €72,000** |

### 1.5 What Makes This Competitive vs. Construction Firms

| **Factor** | **InspectOS Offer** | **Teixeira Duarte / Mota-Engil** | **Advantage** |
|---|---|---|---|
| Base Salary | €38k–€50k | €35k–€55k | Comparable |
| Schedule Flexibility | High (field-based, self-directed) | Low (site-based, rigid hours) | **Major advantage** |
| Travel Requirements | Local (Lisbon/Porto metro) | National/international ( Angola, Mozambique, Brazil) | **Major advantage** |
| Stress Level | Moderate (inspection vs. construction management) | High (deadlines, site pressure) | **Advantage** |
| Equity/Ownership | Possible (startup equity participation) | None | **Differentiator** |
| Technology Exposure | High (proptech platform, AI tools) | Low (traditional project management) | **Differentiator for tech-inclined engineers** |
| Career Path | Inspector → Senior → Team Lead → Regional Manager | Engineer → Project Manager → Director | Comparable |
| Autonomy | High (independent field work) | Moderate (hierarchical) | **Advantage** |

---

## 2. Contractor/Per-Inspection Model

### 2.1 Per-Inspection Rate Structure

The contractor model is InspectOS's **primary capacity-scaling mechanism**. With 5 contractors currently active, this model provides peak-load flexibility without the fixed cost burden of full-time employment. Contractors operate as **trabalhadores independentes** (self-employed), issuing **recibos verdes** (green receipts) through the Portuguese tax portal.

| **Property Type** | **Complexity** | **Per-Inspection Rate (to contractor)** | **InspectOS Revenue** | **Margin** |
|---|---|---|---|---|
| Apartment (T1–T2, <100m²) | Standard | €200 – €250 | €595 | 58–66% |
| Apartment (T3+, 100–150m²) | Standard | €250 – €300 | €595 | 50–58% |
| House/Villa (150–300m²) | Moderate | €300 – €350 | €750–€850 | 53–65% |
| Technical Diagnostic | Complex | €350 – €450 | €650+ | 31–46% |
| Pre-Listing Inspection | Standard | €200 – €250 | €450–€550 | 55–64% |
| Expert Witness / Court Report | Specialist | €400 – €600 | €1,000+ | 40–60% |

### 2.2 Retainer Options

For contractors who guarantee priority availability (e.g., 3+ inspections/week commitment):

| **Retainer Tier** | **Monthly Retainer** | **Commitment** | **Per-Inspection Rate** | **Best For** |
|---|---|---|---|---|
| **Standard** | €0 | Ad hoc | Full rate | Supplemental capacity |
| **Priority** | €500/month | Minimum 12 inspections/month | 10% discount on standard rate | Core capacity in high-demand region |
| **Exclusive** | €1,000/month | Minimum 20 inspections/month + right of first refusal | 15% discount + volume bonuses | Anchor contractor for a region |

### 2.3 Contractor Economics: Tax Optimization

The contractor model is financially advantageous for both parties due to Portugal's freelancer tax structure. [^122^][^123^][^125^] A contractor invoicing InspectOS **€40,000/year** (approximately 12–14 inspections/month at €250 average) faces the following tax treatment under the **Regime Simplificado**:

| **Year** | **Gross Income** | **IRS Coefficient** | **Taxable Base** | **IRS Owed** | **Social Security** | **Net Income** | **Effective Rate** |
|---|---|---|---|---|---|---|---|
| **Year 1** | €40,000 | 0.375 (50% reduction) | €15,000 | €1,499 | €0 (exempt) | **€38,501** | **3.7%** |
| **Year 2** | €40,000 | 0.5625 (25% reduction) | €22,500 | €3,946 | €4,494 | €31,560 | 21.1% |
| **Year 3+** | €40,000 | 0.75 (standard) | €30,000 | €6,541 | €4,494 | €28,965 | 27.6% |

The **Year 1 effective tax rate of 3.7%** is remarkably low due to two first-year benefits: (1) the **50% reduction on IRS taxable base** for new freelancers, and (2) the **12-month social security contribution exemption**. [^123^] This makes the contractor model especially attractive for InspectOS's first-year hires — they keep significantly more of their earnings than they would as employees.

For InspectOS, the contractor model eliminates **employer social security (23.75%)**, **work accident insurance**, **meal allowances**, and **vehicle provisions** (contractors use their own vehicles and claim expenses). The company pays only the invoice amount, with a **23% withholding tax** (retention at source) deducted and remitted to the tax authority on the contractor's behalf. [^122^][^126^]

### 2.4 Equipment and Software Provision

| **Item** | **Provision** | **Rationale** |
|---|---|---|
| **InspectOS Platform Access** | Provided by InspectOS | Core tool for report generation; no cost to contractor |
| **Smartphone/Tablet** | Contractor provides own | Standard equipment; most professionals already own |
| **Vehicle** | Contractor provides own; mileage reimbursed at €0.36/km [^41^] | Field work essential; mileage covers fuel and depreciation |
| **Measuring Tools** | Laser measure, moisture meter, thermal camera (if diagnostic) provided on loan | Specialized tools; InspectOS retains ownership |
| **OE Insurance** | Contractor maintains own OE professional liability insurance (€75,000 via Ageas) [^106^] | Mandatory; covered by OE membership |
| **Digital Camera** | Contractor provides own | Photo documentation essential; smartphone acceptable |

### 2.5 Tax/Invoice Requirements

Contractors must: [^122^][^125^]

1. **Register as trabalhador independente** on Portal das Finanças (free, under 30 minutes)
2. **Select CAE code** for engineering consultancy (CAE 71120 — Atividades de engenharia e técnicas afins)
3. **Issue recibo verde** for each inspection through Portal das Finanças within 5 days of service
4. **Apply 23% withholding tax** (retention at source) when invoicing InspectOS [^126^]
5. **File quarterly social security declarations** (even during exemption period)
6. **Submit annual IRS declaration** (Modelo 3, Anexo B) by June 30

InspectOS must:
1. Verify contractor's NIF and activity registration before first payment
2. Apply withholding tax (23%) on all payments to Portuguese-resident contractors
3. Issue withholding certificate (Modelo 10) annually by January 20
4. Report payments in quarterly VAT return (if InspectOS is VAT-registered)

---

## 3. Brazilian Relocation Package

### 3.1 Standard vs. Differentiator-Level Support

For Brazilian engineers recruited from Brazil (not already in Portugal), InspectOS should offer a **relocation package** that reduces the friction of international move while protecting both parties. The package is structured in **two tiers**: standard (what InspectOS commits to) and differentiator (what sets InspectOS apart from other Portuguese employers).

| **Component** | **Standard (Expected)** | **Differentiator (InspectOS Advantage)** | **Cost** |
|---|---|---|---|
| **OE Registration Fee Sponsorship** | Candidate pays R$ 59.42 CONFEA fee + OEP fees | **InspectOS advances all fees; deducted from first 3 months of pay** | €200–€500 |
| **CPLP Visa Processing** | Candidate handles independently | **InspectOS provides immigration lawyer referral + document checklist + employer letter** | €0 (referral only) |
| **Temporary Housing** | None | **First month housing stipend (€600–€800) or temporary accommodation arranged** | €600–€800 |
| **Flight Costs** | Candidate pays | **One-way flight São Paulo/Lisbon or Rio/Lisbon reimbursed after 6 months** | €500–€800 |
| **Local Orientation** | None | **Half-day orientation: bank account, NIF, NISS, health center registration, neighborhood tour** | €0 (internal time) |
| **Portuguese Language Support** | None | **Optional Portuguese classes if needed (rare for Brazilians)** | €0–€200 |
| **OE Registration Guidance** | None | **Step-by-step guide + direct OEP contact introduction + follow-up support** | €0 (internal time) |
| **First 90 Days Structure** | Standard employment | **Month 1: training + shadowing; Month 2: supervised solo; Month 3: independence assessment** | Built into onboarding |

### 3.2 Risk-Minimization Structure

The first 90 days should protect both parties:

| **Phase** | **Duration** | **Structure** | **InspectOS Commitment** | **Candidate Commitment** |
|---|---|---|---|---|
| **Phase 1: Trainee** | Days 1–30 | IEFP internship or private trainee contract; OEP registration processing | €1,057/month stipend + full training | Full-time attendance; OEP application submission |
| **Phase 2: Supervised Inspector** | Days 31–60 | Contractor agreement (recibo verde); inspections under senior supervision | €200/inspection minimum guarantee | Minimum 8 inspections/month |
| **Phase 3: Full Contractor/Employee** | Days 61–90 | Convert to standard contractor or full-time employment | Standard rates apply | Full performance expectations |

**Key protection clauses:**
- OEP registration must be submitted within **14 days** of arrival
- If OEP registration is denied, contract converts to **Angolan-style support role** (field work under senior supervision) or terminates with **2 weeks' notice**
- Relocation reimbursement (flight) is **clawed back** if candidate leaves within 6 months
- Housing stipend is **forgivable** (no repayment required)

---

## 4. Intern/Trainee Model

### 4.1 IEFP-Funded Internship

The **+Talento internship program** is the most cost-effective talent pipeline for InspectOS. The government reimburses **65–80% of the stipend cost**, reducing net expenditure to **€192–€370/month** for a Master's-level intern. [^67^][^90^][^93^]

| **Parameter** | **Specification** |
|---|---|
| **Duration** | 6 months (non-renewable) [^90^] |
| **Stipend (Master's)** | €1,056.95/month [^67^] |
| **IEFP Reimbursement** | 65–80% of stipend [^90^] |
| **Net Cost to InspectOS** | €211–€370/month |
| **Total 6-Month Net Cost** | €1,266–€2,220 |
| **Candidate Eligibility** | Age ≤35; registered as unemployed with IEFP; degree in relevant field [^93^] |
| **Application Window** | Opens periodically (next: February 10, 2026) [^90^] |

### 4.2 Value Proposition by Month

| **Month** | **Value Provided by Intern** | **InspectOS Investment** | **Net Value** |
|---|---|---|---|
| **Month 1** | Shadowing; administrative support; tool familiarization | €211–€370 + senior time (~20 hours) | Negative (investment phase) |
| **Month 2** | Assisted inspections; photo documentation; report drafting under supervision | Same | Slightly negative |
| **Month 3** | Supervised solo inspections (simple properties); report completion with review | Same | Breaking even |
| **Month 4** | Independent inspections (standard properties); quality improving | Same | Positive |
| **Month 5** | Full independent inspections; contributing to capacity | Same | Clearly positive |
| **Month 6** | Full capacity; conversion evaluation; referral source for university peers | Same | Maximum value |

### 4.3 Conversion Pathway

At Month 6, the intern is evaluated for conversion:

| **Evaluation Criteria** | **Pass Threshold** | **Conversion Offer** |
|---|---|---|
| Trial inspection score | ≥70% | Junior contractor or full-time junior role |
| OE registration (if eligible) | Active or in process | Accelerated to senior track |
| Client satisfaction (if client-facing) | ≥4.0/5.0 | Confirmed for client-facing role |
| Report quality audit | ≥75% | Approved for independent work |
| Attendance and professionalism | 100% attendance; no disciplinary issues | Cleared for conversion |

**Conversion options:**
- **Junior Contractor (recibo verde):** €150–€200 per inspection; flexible schedule
- **Full-Time Junior Employee:** €24,000–€28,000 gross annual; benefits included
- **Extended Trainee:** Additional 3-month IEFP extension (if available) or private trainee contract

---

## 5. Contract Templates & Legal Structures

### 5.1 Contract Type Decision Matrix

| **Scenario** | **Contract Type** | **Why** | **Key Clauses** |
|---|---|---|---|
| **Senior anchor inspector** | Full-time employment (CDI — Contrato a Termo Indeterminado) | Long-term commitment; quality anchor; regulatory compliance | OE verification, insurance, non-compete, IP, 90-day probation |
| **Flexible capacity inspector** | Recibo verde (self-employed contractor) | Cost efficiency; flexibility; no employer SS burden | Service agreement, quality SLA, per-inspection rate, equipment |
| **Brazilian candidate (OEP pending)** | Trainee agreement / IEFP internship | Regulatory compliance during OEP processing | Conversion trigger, clawback, supervision requirements |
| **Angolan support engineer** | Service agreement (support role) | No OE signing authority; supervised work | Supervision ratio, no independent signing, liability limitation |
| **University intern** | IEFP internship agreement | Government-subsidized; low cost | 6-month duration, conversion pathway, educational focus |
| **Vetted inspection firm** | Subcontractor agreement | White-label or overflow capacity | Quality standards, liability, exclusivity terms |

### 5.2 Key Contract Clauses

**Non-Compete Clause (Portuguese law-compliant):**
Portuguese labor law permits non-compete clauses but limits their scope. Under the **Código do Trabalho**, non-compete clauses must: (a) be in writing, (b) specify the restricted activity and geographic area, (c) be limited to **2 years** post-termination for employment contracts, and (d) provide **compensation** during the restriction period (typically 50–100% of base salary). For contractors, the restriction can be broader but must still be reasonable.

InspectOS non-compete:
- **Employment contracts:** 12-month restriction on working for competing inspection platforms in Portugal; compensation of 50% of last monthly salary × restriction months
- **Contractor agreements:** 6-month restriction on soliciting InspectOS clients directly; no compensation required (commercial agreement)

**Intellectual Property Clause:**
All inspection reports, photographs, methodologies, and client data generated during the engagement are the **exclusive property of InspectOS**. The inspector retains no rights to reuse, resell, or disclose client information or report content. This is standard for professional services and essential for maintaining InspectOS's brand integrity and client confidentiality.

**Quality SLA Clause:**
- Reports must be submitted within **48 hours** of site visit
- Report quality score (random audit) must maintain **≥80%** average
- Client complaints related to inspector error are tracked; **3 substantiated complaints** in a 6-month period trigger corrective action (retraining or termination)
- All reports must use InspectOS templates and follow standardized format

**Liability Clause:**
- Full-time employees: Covered by InspectOS corporate insurance + OE individual insurance
- Contractors: Must maintain active OE professional liability insurance (€75,000 minimum); InspectOS not liable for contractor negligence beyond corporate policy
- Trainees/interns: Covered by supervising OE-registered inspector's insurance

**Termination Clause:**
- **Employment contracts:** 30–60 days' notice (per Código do Trabalho); probation period 90 days (extendable to 180 days for graduates)
- **Contractor agreements:** 15 days' notice by either party; immediate termination for quality failures or OE membership lapse
- **Trainee agreements:** 7 days' notice; automatic termination if OEP registration denied

---

## 6. Total Reward Statement Template

The following template communicates the full value of the InspectOS compensation package to candidates:

---

### **InspectOS Total Reward Statement**

**Position:** Senior Property Inspector (Lisbon)

| **Component** | **Annual Value (€)** |
|---|---|
| **Base Salary** (14 payments) | €45,000 |
| **Meal Allowance** | €2,693 |
| **Vehicle Allowance** | €5,400 |
| **Phone/Internet** | €720 |
| **Health Subsidy** | €900 |
| **Professional Development** | €1,200 |
| **Performance Incentives** (target) | €2,500 |
| **Total Cash & Benefits** | **€58,413** |
| **Employer Social Security Contribution** (23.75%) | €10,688 |
| **Work Accident Insurance** | €675 |
| **Total Investment by InspectOS** | **€69,776** |

**Additional Benefits:**
- OE professional liability insurance (€75,000 coverage) — **provided free via OE/Ageas** [^106^]
- Flexible schedule and remote work options
- Professional development budget (OE credits, conferences)
- Career path: Inspector → Senior → Team Lead → Regional Manager
- Startup equity participation (eligible after 12 months)

**Net Monthly Income (Employee):**
- Gross monthly: €3,214 (14 payments)
- Employee SS (11%): -€354
- IRS withholding (~18%): -€578
- **Net monthly: ~€2,282**

---

## 7. Quick Reference: Portuguese Tax & Social Security 2026

| **Parameter** | **Value** | **Applies To** |
|---|---|---|
| Minimum wage | €920/month (14 payments = €12,880/year) [^48^] | All employees |
| Employee social security | 11% of gross salary [^128^] | Employees |
| Employer social security | 23.75% of gross salary [^128^] | Employers |
| Work accident insurance | 1–2% of gross salary [^131^] | Employers |
| Freelancer IRS coefficient (Year 1) | 37.5% of gross (50% reduction) [^123^] | New freelancers |
| Freelancer IRS coefficient (Year 2) | 56.25% of gross (25% reduction) [^123^] | Second-year freelancers |
| Freelancer IRS coefficient (Year 3+) | 75% of gross (standard) [^122^] | Established freelancers |
| Freelancer social security | 21.4% on 70% of income = ~15% effective [^125^] | Freelancers (Year 2+) |
| Freelancer SS exemption | 12 months [^123^] | First-time freelancers |
| Withholding tax (engineers) | 23% [^122^][^126^] | Contractors invoicing companies |
| VAT exemption threshold | €15,000/year [^122^] | Freelancers below threshold |
| Standard VAT rate | 23% [^122^] | Mainland Portugal |
| IRS filing deadline | April 1 – June 30 [^125^] | All taxpayers |
| Meal allowance (tax-free) | €10.20/day [^48^] | Employees |
| Mileage reimbursement | €0.36/km [^41^] | Employees using own vehicle |
