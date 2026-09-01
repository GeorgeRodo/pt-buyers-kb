# InspectOS Non-Inspector Hiring Plan
## Legal, Operations, Sales, Technology & Finance Roles

## TL;DR

This document complements the inspector-focused 7-prompt pipeline with hiring strategies for the **five additional capability layers** InspectOS needs to scale: **Legal & Compliance**, **Operations**, **Sales & Marketing**, **Technology**, and **Finance & Admin**. For a pre-seed/seed proptech startup, the recommended approach is **heavy outsourcing + strategic part-time hires**, not full-time payroll bloat. Priority sequencing: (1) **External legal counsel** (€2,000–€5,000/month) and **outsourced DPO** (€300–€800/month) are non-negotiable from Day 1 due to court-admissible reports and GDPR; (2) **Operations Manager** (€35,000–€45,000/year) is the first full-time non-inspector hire — this person orchestrates scheduling, quality, and inspector network management; (3) **Fractional CTO** (€150–€400/hour, ~€2,000–€4,000/month part-time) handles platform architecture and technical strategy without the cost of a full-time executive; (4) **Sales/BD** (€28,000–€40,000/year base + commission) and **outsourced bookkeeping** (€299–€600/month) follow once revenue justifies the headcount. The phased hiring roadmap staggers these roles across 12 months with a **total Year 1 non-inspector payroll budget of €85,000–€120,000** (excluding the already-budgeted inspector recruitment costs).

---

## 1. Legal & Compliance (High Priority — Risk Mitigation)

### 1.1 The Non-Negotiable Nature

Property inspections produce **court-admissible reports**, creating liability exposure on multiple fronts: professional negligence claims, regulatory non-compliance (OE, DGEG, ADENE), data privacy (GDPR), and contractual disputes. Unlike many startup functions where "we'll figure it out later" is acceptable, legal and compliance infrastructure must be in place **before** the first report is challenged, the first GDPR complaint is filed, or the first regulatory audit occurs. The CNPD (Comissão Nacional de Proteção de Dados) can impose fines of up to **€20 million or 4% of global turnover** for GDPR violations [^157^], and a single successful negligence claim against an inspection report could exceed InspectOS's annual revenue.

### 1.2 External Legal Counsel (Part-Time → Retained)

| **Profile** | **Real Estate/Construction Lawyer** |
|---|---|
| **Role** | Draft report disclaimers and liability waivers; review partnership agreements; advise on DL 10/2024 implications; handle client disputes; ensure OE compliance |
| **Engagement Model** | Monthly retainer (recommended) or hourly billing |
| **Cost** | **€150–€300/hour** for specialized real estate/construction counsel [^159^]; **€2,000–€5,000/month retainer** for ongoing advisory |
| **Sourcing** | Ordem dos Advogados (Portuguese Bar Association) directory; referrals from OE or real estate contacts; firms like Miranda, PLMJ, Vieira de Almeida (top tier, expensive) or mid-size Lisbon/Porto firms |
| **Key Tasks** | Report disclaimer language; contractor service agreements review; client T&Cs; partnership MOUs; regulatory change monitoring (DL 10/2024, RGEU replacement) |
| **When to Hire** | **Immediately** — before any new contract template is used |

Portuguese lawyer fees for property/construction matters typically follow two models: **hourly billing** at €150–€300/hour for specialized counsel, or **percentage-based fees** at 1–3% of transaction value for property transactions. [^159^][^161^] For InspectOS's needs (contracts, compliance advice, dispute resolution), a **monthly retainer of €2,000–€5,000** with a mid-size Lisbon firm is the most cost-effective model. This provides predictable budgeting and priority access to counsel when issues arise.

**Recommended Approach for InspectOS:**
- **Months 1–6:** External counsel on retainer (€2,000–€3,000/month) for contract drafting, template review, and ad-hoc advice
- **Months 6–12:** Increase retainer to €3,000–€5,000/month as operations scale and contractual volume grows
- **Month 12+:** Evaluate whether in-house legal (part-time or full-time) is justified based on transaction volume and dispute frequency

### 1.3 Compliance Officer / Quality Assurance Manager

| **Profile** | **Compliance/QA Manager (Part-Time Initially)** |
|---|---|
| **Role** | Oversee OE/DGEG/ADENE standards adherence; monitor report consistency; manage inspector insurance verification; conduct internal audits; maintain regulatory change log |
| **Engagement Model** | Part-time employee (50–75%) or contractor |
| **Cost** | **€18,000–€28,000/year** part-time (50%); **€25,000–€36,000/year** full-time [^178^] |
| **Sourcing** | OE member with regulatory background; former ADENE/DGEG employee; quality professional from construction/inspection sector |
| **Key Tasks** | Monthly insurance verification (all inspectors); random report audits; OE registration status tracking; ADENE certification compliance; corrective action oversight |
| **When to Hire** | **Month 2–3** — once 2+ full-time inspectors are onboarded |

The average Compliance Officer salary in Portugal is **€25,490/year**, with early-career professionals (1–4 years) earning around **€18,000** and mid-career (5–9 years) reaching **€36,475**. [^178^] For InspectOS, a **part-time compliance role at 50% FTE (€12,000–€18,000/year)** is sufficient initially, with the scope expanding to full-time as the inspector network grows beyond 15–20 active inspectors.

**Critical insight:** This role can be **combined with the Operations Manager** in the early stage (Months 3–9), with a dedicated compliance hire splitting off once the operational volume justifies it. The combined "Operations & Compliance Manager" profile is realistic for a startup and reduces early payroll costs.

### 1.4 Data Protection Officer (DPO) — Outsourced

| **Profile** | **External DPO (Mandatory for GDPR Compliance)** |
|---|---|
| **Role** | GDPR compliance oversight; data processing register (RoPA); Data Subject Access Request (DSAR) handling; DPIA (Data Protection Impact Assessment) for new processing; breach response; CNPD liaison |
| **Engagement Model** | Outsourced DPO service (mandatory independence requirement under GDPR Article 38) [^158^] |
| **Cost** | **€300–€800/month** (Shield/Co-Pilot packages); **€2,500+/month** for enterprise-grade governance [^156^] |
| **Providers** | Data Privacy Office (data-privacy-office.eu); DPO Centre (dpocentre.com); local Portuguese DPO firms; Bulletproof (bulletproof.co.uk) [^156^][^158^][^160^] |
| **Why Outsourced** | GDPR Article 38 requires DPO independence — an internal employee with other duties creates a conflict of interest [^158^]; external DPO costs up to 5× less than full-time hire (avg. €70,000/year Europe) [^156^] |
| **When to Engage** | **Immediately** — before processing any client personal data at scale |

For InspectOS, a **"Shield" or "Co-Pilot" package (€300–€800/month)** provides adequate coverage: named DPO appointment, supervisory authority registration, RoPA structure, DSAR workflow, vendor assessment process, and ongoing advisory via email/Slack. [^156^] The **€1,200 one-time implementation pack** establishes the foundational privacy infrastructure (RoPA, DSAR workflow, policy gap map) in the first 30 days. Given that InspectOS handles client names, property addresses, photos, and financial data, GDPR compliance is not optional — and an outsourced DPO is the most cost-effective path.

### 1.5 Legal & Compliance Budget Summary

| **Role** | **Model** | **Monthly Cost** | **Annual Cost** | **Priority** |
|---|---|---|---|---|
| External Legal Counsel | Monthly retainer | €2,000–€5,000 | €24,000–€60,000 | **Immediate** |
| Compliance/QA Manager | Part-time (50%) employee | €1,500–€2,500 | €18,000–€30,000 | **Month 2–3** |
| Outsourced DPO | Monthly service package | €300–€800 | €3,600–€9,600 | **Immediate** |
| **Total Legal/Compliance** | | **€3,800–€8,300** | **€45,600–€99,600** | |

---

## 2. Operations (Critical for Scaling)

### 2.1 Operations Manager / Head of Inspections

The Operations Manager is the **first non-inspector full-time hire** InspectOS should make. This person is the organizational backbone: they manage the inspector network (contractors, full-time, partners), coordinate scheduling, enforce quality standards, manage SLAs (e.g., 48-hour report delivery), and ensure regional coverage. Without this role, the founder/CEO becomes the bottleneck for every operational decision — a situation that becomes untenable once the inspector count exceeds 8–10.

| **Profile** | **Operations Manager / Head of Inspections** |
|---|---|
| **Role** | Inspector network management; scheduling and dispatch; quality audit oversight; training coordination; SLA enforcement; regional coverage planning; peak demand management |
| **Experience Required** | 3–7 years operations management; construction/property sector experience preferred; familiarity with contractor management; tech-savvy (platform tools) |
| **Cost** | **€35,000–€45,000/year gross** (Lisbon) [^164^][^165^][^166^]; **€32,000–€40,000/year** (Porto) |
| **Total Employer Cost** | €47,000–€61,000/year (including 23.75% SS, insurance, meal allowance) |
| **Sourcing** | LinkedIn; Net-Empregos; Michael Page/Hays (operations recruitment); referrals from construction/property contacts |
| **When to Hire** | **Month 2–4** — once inspector count reaches 7+ (5 existing + 2 new) |

Salary data for Operations Managers in Portugal shows a median of **$42,867/year (~€39,000)** [^164^], with Glassdoor reporting **€37,500 in Lisbon** [^166^] and ERI estimating **€49,781 nationally** [^165^]. For InspectOS, targeting the **€35,000–€45,000 range** (depending on experience level) is competitive while remaining appropriate for a startup budget.

**The "Operations + Compliance" Hybrid (Months 3–9):**

To optimize early payroll, InspectOS can hire an Operations Manager with **compliance responsibilities** built into the role:

| **Combined Responsibilities** | **Time Split** |
|---|---|
| Inspector scheduling & dispatch | 30% |
| Quality audit coordination | 20% |
| OE insurance/regulatory tracking | 15% |
| Training & onboarding management | 15% |
| Client communication & escalation | 10% |
| Reporting & metrics | 10% |

This combined role commands a **10–15% salary premium** over a pure operations role (€38,000–€50,000) but eliminates the need for a separate compliance hire until Month 9–12.

### 2.2 Scheduler / Dispatch Coordinator

| **Profile** | **Scheduler / Admin Support** |
|---|---|
| **Role** | Booking system management; client appointment scheduling; inspector route optimization; confirmation calls/emails; calendar management |
| **Engagement Model** | Full-time admin or virtual assistant |
| **Cost** | **€18,000–€24,000/year** (entry-level admin in Lisbon) [^173^] |
| **When to Hire** | **Month 6–9** — once daily inspection volume exceeds 8–10 inspections |

### 2.3 Field Operations / Training Lead

| **Profile** | **Field Operations & Training Lead** |
|---|---|
| **Role** | Onboard new inspectors; conduct trial inspections; perform quality audits; manage equipment inventory; standardize field processes; mentor junior inspectors |
| **Engagement Model** | Senior inspector promoted internally OR external hire |
| **Cost** | **€32,000–€42,000/year** (if external); **€3,000–€5,000/year stipend/bonus** (if promoted from senior inspector) |
| **When to Hire** | **Month 6–12** — once 3+ senior inspectors are in place; promote internally first |

### 2.4 Operations Budget Summary

| **Role** | **Model** | **Monthly Cost** | **Annual Cost** | **Target Hire** |
|---|---|---|---|---|
| Operations + Compliance Manager | Full-time employee | €2,900–€3,750 | €35,000–€45,000 | **Month 3** |
| Scheduler / Admin | Full-time employee | €1,500–€2,000 | €18,000–€24,000 | **Month 6** |
| Field Ops / Training Lead | Internal promotion + stipend | €250–€400 | €3,000–€5,000 | **Month 9** |
| **Total Operations (Year 1)** | | **€4,650–€6,150** | **€56,000–€74,000** | |

---

## 3. Sales & Marketing (Revenue Growth)

### 3.1 Sales / Business Development Manager

The Sales/BD Manager targets the **B2B partnerships** that drive scalable revenue: real estate agencies, lawyers, banks, investors, and developers who need bulk inspections or white-label services. This role is **revenue-generating** — a successful BD manager should pay for themselves within 3–6 months through new partnership deals.

| **Profile** | **Business Development Manager** |
|---|---|
| **Role** | B2B partnership development; real estate agency acquisition; bank/insurer white-label deals; investor/client relationship management; pipeline management; revenue forecasting |
| **Experience Required** | 3–5 years B2B sales; real estate or proptech sector experience; network in Lisbon/Porto property market; Portuguese + English fluent |
| **Cost** | **€28,000–€40,000/year base** + **10–20% commission** on new deals [^173^] |
| **On-Target Earnings (OTE)** | €35,000–€55,000/year |
| **Sourcing** | LinkedIn Sales Navigator; property industry referrals; recruitment agencies (Michael Page, Hays); real estate networking events |
| **When to Hire** | **Month 4–6** — once core operations are stable and there's capacity to handle B2B volume |

Salary benchmarks for sales roles in Portugal [^173^]:

| **Sales Role** | **Entry** | **Mid-Level** | **Senior** |
|---|---|---|---|
| Sales Representative | €1,100–€1,500/mo | €1,800–€2,500/mo | €3,000–€4,500/mo |
| Business Development Manager | — | €2,300–€3,300/mo | €3,300–€4,500/mo |
| Account Manager | — | €2,000–€2,800/mo | €3,000–€4,000/mo |

For InspectOS, a **mid-level BD Manager at €2,500–€3,000/month base (€30,000–€36,000/year)** with a **15% commission** on new B2B revenue is the right profile. The commission structure should target:

| **Deal Type** | **Commission** | **Example** |
|---|---|---|
| New real estate agency partnership | 15% of first 3 months' revenue | Agency refers 10 inspections/month @ €595 = €5,950/mo × 15% = €893 |
| Bank white-label contract | 10% of annual contract value | €50,000/year contract = €5,000 commission |
| Investor portfolio deal | 10% of deal value | 20 inspections @ €550 = €11,000 × 10% = €1,100 |

### 3.2 Marketing Specialist / Content Lead

| **Profile** | **Marketing Specialist (Part-Time → Full-Time)** |
|---|---|
| **Role** | SEO optimization ("home inspection Portugal", "vistoria técnica Lisboa"); Google Ads management; LinkedIn content and outreach; DL 10/2024 educational content; bilingual (PT/EN) materials; website management; review generation; lead nurturing |
| **Engagement Model** | Part-time contractor (50%) initially; full-time once revenue justifies |
| **Cost** | **€1,200–€2,000/month** part-time (recibo verde); **€2,000–€3,000/month** full-time [^173^] |
| **When to Hire** | **Month 3–6** — part-time contractor; **Month 9–12** — evaluate full-time conversion |

Marketing Manager salaries in Portugal range from **€2,000–€2,800/month mid-level** to **€3,200–€5,000/month senior**. [^173^] For InspectOS's needs (digital-first, content-heavy, SEO-focused), a **part-time marketing contractor at €1,200–€2,000/month** provides sufficient capacity for content creation, ad management, and social media — with the flexibility to scale up as lead volume grows.

### 3.3 Account Manager / Customer Success

| **Profile** | **Account Manager (Part-Time Initially)** |
|---|---|
| **Role** | Post-sale follow-up; upsell energy certificates, snagging inspections, diagnostic services; retention for repeat clients (investors, agencies); NPS tracking; churn prevention |
| **Engagement Model** | Part-time (combined with scheduler/admin initially) |
| **Cost** | **€1,500–€2,500/month** part-time |
| **When to Hire** | **Month 6–9** — once B2B client base reaches 10+ recurring partners |

### 3.4 Sales & Marketing Budget Summary

| **Role** | **Model** | **Monthly Cost** | **Annual Cost** | **Target Hire** |
|---|---|---|---|---|
| BD Manager | FT employee + commission | €2,500–€3,300 + commission | €30,000–€40,000 base | **Month 5** |
| Marketing Specialist | PT contractor (50%) | €1,200–€2,000 | €14,400–€24,000 | **Month 4** |
| Account Manager | PT employee | €1,500–€2,500 | €18,000–€30,000 | **Month 9** |
| **Total Sales/Mktg (Year 1)** | | **€5,200–€7,800** | **€62,400–€94,000** | |

---

## 4. Technology & Platform

### 4.1 Fractional CTO / Tech Lead

InspectOS's platform already supports online booking — the technology priority is **maintenance, incremental improvements, and scalability planning**, not ground-up development. A full-time CTO is massively overkill at this stage. A **fractional CTO** provides executive-level technical guidance on a part-time basis.

| **Profile** | **Fractional CTO** |
|---|---|
| **Role** | Platform architecture oversight; technical strategy; vendor management (hosting, SaaS tools); security assessment; mobile app roadmap; AI/automation integration planning; technical due diligence for investors |
| **Engagement Model** | Part-time retainer (1–2 days/week) or hourly |
| **Cost** | **€150–€400/hour** [^184^]; **€2,000–€4,000/month** retainer (20–40 hours/month); **€5,000–€10,000/project** for specific deliverables (MVP, audit, architecture review) [^180^] |
| **Sourcing** | Toptal (toptal.com); 10x Team (10x.team); Fractional Jobs (fractionaljobs.io); Portuguese tech community (Porto Tech Hub, Lisbon tech meetups); LinkedIn |
| **When to Engage** | **Month 1–2** — for platform audit and technical roadmap; ongoing retainer from Month 3 |

Fractional CTO rates vary by scope and expertise: [^180^][^184^]

| **Engagement Type** | **Rate** | **Best For** |
|---|---|---|
| Hourly advisory | €150–€250/hour | Ad-hoc technical decisions; vendor evaluation; architecture questions |
| Monthly retainer (20 hrs) | €2,000–€3,000/month | Ongoing guidance; roadmap execution; team mentoring |
| Monthly retainer (40 hrs) | €3,500–€5,000/month | Active development oversight; sprint planning; technical leadership |
| Project-based (MVP/audit) | €5,000–€15,000 | Specific deliverable with defined scope and timeline |

**Recommended for InspectOS:** Start with a **€2,000–€3,000/month retainer** (20 hours/month) for ongoing platform oversight, technical strategy, and vendor management. Scale to 40 hours/month only if significant development work is initiated (e.g., mobile app, AI features).

### 4.2 Software Developer (Freelance / Contractor)

| **Profile** | **Software Developer (Part-Time Contractor)** |
|---|---|
| **Role** | Platform maintenance; bug fixes; feature development (report templates, client portal, inspector mobile interface); integrations (calendar, payments, CRM) |
| **Engagement Model** | Freelance contractor (recibo verde) part-time |
| **Cost** | **€2,200–€3,500/month** part-time (60–80 hours/month) for mid-level developer [^173^]; **€3,500–€5,500/month** for senior |
| **Sourcing** | Toptal; Upwork (Portuguese developers); Landing.jobs (Portuguese tech jobs); LinkedIn; referrals from fractional CTO |
| **When to Hire** | **Month 3–6** — once technical roadmap from fractional CTO is defined |

Portuguese software engineer salaries [^173^]:

| **Level** | **Monthly Gross** | **Annual Gross** |
|---|---|---|
| Junior (0–2 yrs) | €1,400–€1,800 | €19,600–€25,200 |
| Mid-Level (2–5 yrs) | €2,200–€3,200 | €30,800–€44,800 |
| Senior (5+ yrs) | €3,500–€5,500 | €49,000–€77,000 |

For InspectOS, a **mid-level developer at €2,500–€3,000/month part-time** (recibo verde, so no employer SS) provides sufficient development capacity for incremental platform improvements without the commitment of a full-time hire.

### 4.3 Technology Budget Summary

| **Role** | **Model** | **Monthly Cost** | **Annual Cost** | **Target Hire** |
|---|---|---|---|---|
| Fractional CTO | Monthly retainer (20 hrs) | €2,000–€3,000 | €24,000–€36,000 | **Month 2** |
| Software Developer | PT contractor (recibo verde) | €2,500–€3,000 | €30,000–€36,000 | **Month 4** |
| **Total Technology (Year 1)** | | **€4,500–€6,000** | **€54,000–€72,000** | |

---

## 5. Finance & Admin

### 5.1 Bookkeeper / Accountant (Outsourced)

Finance is a **prime outsourcing candidate** for a startup at InspectOS's stage. Portuguese accounting firms specializing in freelancers and small businesses offer comprehensive packages at a fraction of in-house costs.

| **Profile** | **Outsourced Accountant / Bookkeeper** |
|---|---|
| **Role** | Monthly bookkeeping; invoicing and recibo verde processing for contractors; VAT (23%) filing; payroll processing; expense tracking; financial reporting; year-end tax preparation |
| **Engagement Model** | Monthly service package from Portuguese accounting firm |
| **Cost** | **€299–€600/month** for small business packages [^174^][^176^]; **€600–€1,200/month** for full-service (bookkeeping + payroll + tax) |
| **Providers** | Elevate Accounting (elevateaccounting.pt, from €299/mo) [^174^]; Atlantic Accounting (atlanticaccounting.pt) [^176^]; local TOC (Técnico Oficial de Contas) firms |
| **When to Engage** | **Immediately** — before first contractor payment or invoice |

Portuguese accounting packages for small businesses typically include [^174^][^176^]:

| **Tier** | **Monthly Cost** | **Includes** |
|---|---|---|
| **Starter** | €299–€400 | Monthly bookkeeping, bank reconciliation, VAT filing, basic reporting |
| **Core** | €400–€600 | Full bookkeeping + payroll (up to 5 employees) + quarterly IRS + financial statements |
| **Full-Service** | €600–€1,000 | All above + contractor invoicing support + year-end tax + advisory |

For InspectOS, the **Core package (€400–€600/month)** is appropriate given the mix of employees, contractors (recibos verdes), and VAT-liable services.

### 5.2 Financial Controller / CFO (Later Stage)

| **Profile** | **Financial Controller / Part-Time CFO** |
|---|---|
| **Role** | Budgeting and forecasting; pricing strategy; investor reporting; financial modeling; fundraising support; cash flow management |
| **Engagement Model** | Part-time consultant or fractional CFO |
| **Cost** | **€2,000–€4,000/month** part-time (1–2 days/week); **€60,000–€90,000/year** full-time |
| **When to Hire** | **Month 9–18** — when preparing for Seed/Series A fundraising or when revenue exceeds €500K/year |

### 5.3 Office / Admin Support

| **Profile** | **Virtual Assistant / Admin Support** |
|---|---|
| **Role** | General admin; data entry; report formatting support; CRM management; email handling; document organization |
| **Engagement Model** | Part-time VA (remote) |
| **Cost** | **€800–€1,200/month** part-time (Portugal-based); **€400–€800/month** (offshore VA) |
| **When to Hire** | **Month 6–9** — once operational volume justifies |

### 5.4 Finance & Admin Budget Summary

| **Role** | **Model** | **Monthly Cost** | **Annual Cost** | **Target Hire** |
|---|---|---|---|---|
| Outsourced Accountant | Monthly service package | €400–€600 | €4,800–€7,200 | **Immediate** |
| Virtual Assistant / Admin | PT remote | €800–€1,200 | €9,600–€14,400 | **Month 6** |
| Financial Controller | PT consultant | €2,000–€4,000 | €12,000–€24,000 | **Month 12** |
| **Total Finance/Admin (Year 1)** | | **€3,200–€5,800** | **€26,400–€45,600** | |

---

## 6. 12-Month Non-Inspector Hiring Roadmap

### 6.1 Phased Hiring Sequence

| **Month** | **Role** | **Model** | **Monthly Cost** | **Cumulative Monthly** |
|---|---|---|---|---|
| **Month 1** | External Legal Counsel (retainer) | External | €2,500 | €2,500 |
| | Outsourced DPO | External | €500 | €3,000 |
| | Outsourced Accountant | External | €500 | €3,500 |
| **Month 2** | Fractional CTO (retainer) | External | €2,500 | €6,000 |
| **Month 3** | Operations + Compliance Manager | FT employee | €3,200 | €9,200 |
| **Month 4** | Marketing Specialist (PT contractor) | Contractor | €1,500 | €10,700 |
| | Software Developer (PT contractor) | Contractor | €2,500 | €13,200 |
| **Month 5** | BD Manager (FT employee) | FT employee | €2,800 + commission | €16,000 |
| **Month 6** | Scheduler / Admin (FT employee) | FT employee | €1,800 | €17,800 |
| | Virtual Assistant (PT) | Contractor | €1,000 | €18,800 |
| **Month 9** | Account Manager (PT employee) | PT employee | €2,000 | €20,800 |
| **Month 12** | Financial Controller (PT consultant) | Consultant | €3,000 | €23,800 |

### 6.2 Budget Summary by Quarter

| **Quarter** | **Roles Active** | **Quarterly Cost** | **Cumulative Year 1** |
|---|---|---|---|
| **Q1 (M1–3)** | Legal counsel, DPO, Accountant, Fractional CTO, Ops Manager | ~€22,000 | €22,000 |
| **Q2 (M4–6)** | + Marketing, Developer, BD Manager, Scheduler/Admin, VA | ~€50,000 | €72,000 |
| **Q3 (M7–9)** | Stable team + Account Manager | ~€55,000 | €127,000 |
| **Q4 (M10–12)** | + Financial Controller | ~€65,000 | €192,000 |
| **TOTAL YEAR 1** | | | **€192,000** |

**Note:** This €192,000 represents the **ramp-up scenario** where all roles are hired on the aggressive timeline. A more conservative approach (delaying non-critical hires by 2–3 months) reduces Year 1 spend to approximately **€140,000–€160,000**.

### 6.3 Headcount Summary

| **Category** | **Month 1** | **Month 6** | **Month 12** |
|---|---|---|---|
| **Inspectors** | 5 contractors | 8–10 (5+ FT/contractor) | 12–15 |
| **Legal/Compliance** | 2 external | 2 external + 1 FT (Ops/Compliance) | 2 external + 1 FT |
| **Operations** | 0 | 2 FT (Ops Manager + Admin) | 3 FT (Ops, Admin, Training Lead) |
| **Sales/Marketing** | 0 | 2 (1 FT BD + 1 PT Marketing) | 3 (BD, Marketing, Account Mgr) |
| **Technology** | 0 | 2 external (CTO + Developer) | 2 external |
| **Finance/Admin** | 1 external (Accountant) | 2 external + 1 PT (Accountant, VA) | 3 (Accountant, VA, Controller) |
| **TOTAL HEADCOUNT** | **~8** | **~17–20** | **~25–30** |

---

## 7. Sourcing Channels for Non-Inspector Roles

### 7.1 Role-Specific Sourcing Strategies

| **Role** | **Best Channels** | **Expected Time-to-Hire** | **Cost-per-Hire** |
|---|---|---|---|
| **Operations Manager** | LinkedIn; Net-Empregos; Michael Page; referrals from construction/property network | 4–8 weeks | €1,500–€3,000 |
| **BD Manager** | LinkedIn Sales Navigator; property industry events; recruitment agencies | 4–8 weeks | €2,000–€4,000 |
| **Marketing Specialist** | LinkedIn; Landing.jobs; creative recruitment (Ponto.Gentil); freelancer platforms | 3–6 weeks | €500–€1,500 |
| **Fractional CTO** | Toptal; 10x Team; Fractional Jobs; Portuguese tech meetups | 2–4 weeks | €0 (platform fees) |
| **Software Developer** | Landing.jobs; Toptal; Upwork (Portuguese); GitHub; LinkedIn | 4–8 weeks | €1,000–€2,500 |
| **External Legal** | Ordem dos Advogados; referrals; industry events | 1–2 weeks | €0 |
| **Outsourced DPO** | Data Privacy Office; DPO Centre; CNPD registered providers | 1–2 weeks | €0 |
| **Outsourced Accountant** | Google; referrals; Ordem dos Técnicos Oficiais de Contas | 1–2 weeks | €0 |

### 7.2 Key Platforms for Portuguese Non-Engineering Talent

| **Platform** | **Best For** | **URL** |
|---|---|---|
| **Landing.jobs** | Tech, marketing, operations roles in Portugal | landing.jobs |
| **Michael Page Portugal** | Mid-to-senior professional roles (ops, sales, legal) | michaelpage.pt |
| **Hays Portugal** | Professional and technical roles | hays.pt |
| **Net-Empregos** | General professional roles | net-empregos.com |
| **Indeed.pt** | Broad reach across all categories | indeed.pt |
| **LinkedIn** | All professional roles; best for BD and ops | linkedin.com |
| **Toptal** | Elite fractional CTOs and developers | toptal.com |
| **10x Team** | Fractional executives (CTO, CMO, CFO) | 10x.team |
| **Upwork** | Freelance developers, marketers, VAs | upwork.com |

---

## 8. Risk Mitigation: Non-Inspector Hiring

| **Risk** | **Mitigation** |
|---|---|
| **Over-hiring before revenue justifies** | Use the phased roadmap; default to outsourcing/part-time; only convert to FT when revenue covers 1.5× the role cost |
| **BD Manager fails to generate ROI** | 3-month probation with clear KPIs (pipeline value, partnership meetings, closed deals); commission-heavy structure reduces fixed cost |
| **Operations Manager can't scale** | Hire someone with 3–7 years experience who has scaled teams before; avoid first-time managers for this critical role |
| **Fractional CTO not available enough** | Build in minimum availability (20 hrs/month) with response time SLAs; maintain relationship with backup CTO |
| **Legal costs balloon** | Cap monthly retainer; define scope clearly (excluded: litigation, which is hourly); review every 6 months |
| **Marketing spend without measurable ROI** | Track CAC (customer acquisition cost) and lead source; cut channels that don't convert within 90 days |

---

## 9. Integration with Inspector Recruitment

The non-inspector hiring plan and the inspector recruitment pipeline (from the 7-prompt Master Plan) are **interdependent**. Key integration points:

| **Integration Point** | **How They Connect** |
|---|---|
| **Operations Manager ↔ Inspector Onboarding** | The Ops Manager executes the 90-day onboarding journey from Prompt 5; they need to be hired before inspector volume exceeds 8–10 |
| **Legal Counsel ↔ Contract Templates** | External lawyer reviews all contract templates (employment, contractor, trainee) before they're used in the inspector vetting process |
| **DPO ↔ Inspector Data** | The DPO ensures GDPR compliance for inspector personal data, client data, and property photos processed through the platform |
| **BD Manager ↔ B2B Talent Licensing** | The BD Manager sells the B2B training/certification services outlined in Prompt 7, creating revenue from the training infrastructure built for inspectors |
| **Marketing ↔ Brazilian Pipeline** | The Marketing Specialist creates Portuguese-language content for the Brazilian Market Entry Program from Prompt 7 |
| **Fractional CTO ↔ AI Automation** | The fractional CTO evaluates and implements the AI-assisted inspection tools identified in Prompt 7's future-proofing section |
| **Accountant ↔ Contractor Payments** | The outsourced accountant processes all recibo verde payments to contractor inspectors, handles VAT, and ensures withholding compliance |
