# InspectOS Quality Gates Playbook

## TL;DR

This playbook establishes a **7-gate decision tree** from first candidate contact to approved inspector status, with an estimated **total timeline of 15–45 days** depending on candidate type. Every inspector producing court-admissible reports for InspectOS must be either **(a) an OE-registered engineer with active professional liability insurance** (€75,000 coverage provided free through Ageas Portugal, policy 8410226152) [^106^][^109^], or **(b) working under the direct supervision of such an engineer** with the registered engineer signing all reports. The **Compliance Risk Matrix** identifies **three highest-risk failure points**: (1) hiring an engineer whose OE membership has lapsed or who lacks signing authority, (2) allowing a Brazilian candidate to inspect before CONFEA-to-OEP transfer is complete, and (3) failing to verify that the OE professional liability insurance declaration has been issued. This document provides step-by-step verification protocols for each gate, specific regulatory references (OE bylaws, DL 10/2024, Lei 25/2018, DGES Decreto-Lei 66/2018), and a standardized trial inspection scenario with evaluation rubric.

---

## 1. Gate 1: OE Verification Workflow

### 1.1 Why This Gate Is Non-Negotiable

Under Portuguese law, **only OE-registered engineers** (or architects registered with the Ordem dos Arquitetos) can issue **court-admissible technical inspection reports**. [^27^] The OE's professional regulatory framework, established by **Decreto-Lei n.º 27.288/1936** and governed by the **Estatuto de 1992** [^24^], creates a clear legal hierarchy: an inspection report signed by a non-OE-registered individual lacks the professional certification required for judicial proceedings and may expose both the individual and InspectOS to liability under the **Código da Responsabilidade Civil Profissional**.

InspectOS's market positioning explicitly depends on this credential: the company's website states inspectors are "**OE, DGEG and ADENE verifiable**" and contrasts this with "market typical" where credentials "vary; no standardised credential." [^121^] Maintaining this competitive differentiation requires rigorous OE verification at the very first gate.

### 1.2 Step-by-Step OE Verification Process

**Step 1: Initial Self-Declaration**
The candidate provides:
- Full name (as registered with OE)
- OE membership number (número de cédula profissional)
- OE registration specialty (Civil, Electrotechnical, Mechanical, etc.)
- OE professional title (Engenheiro Nível 1, Nível 2, Sénior, or Especialista)
- Date of OE admission

**Step 2: Official Verification via OE Records**
The IMPIC (Instituto dos Mercados Públicos, do Imobiliário e da Construção) maintains a **public registry of civil engineers** authorized under **Lei nº 25/2018, de 14 de junho** — the law governing technical roles in construction. [^22^] This registry can be accessed at [impic.pt](https://www.impic.pt/impic/pt-pt/consultar/listagem-eng-civis-lei252018_2) and provides:
- Engineer name
- IMPIC registration number
- Geographic region (Norte, Centro, Sul, Açores, Madeira)

While this registry does not cover all OE members (only those registered for specific construction roles under Lei 25/2018), it provides a **first-pass verification** for civil engineers claiming signing authority.

For comprehensive verification, InspectOS should:

| **Verification Action** | **Method** | **Expected Outcome** | **Timeline** |
|---|---|---|---|
| Request OE membership card scan | Candidate submits Cédula Profissional | Visual confirmation of membership number, specialty, and validity date | Same day |
| Verify via OE regional office | Phone/email to OE North/South regional office | Direct confirmation of active status | 1–2 business days |
| Request OE professional liability declaration | Candidate requests from Ageas via engenheiros@ageas.pt [^106^] | Confirms insurance coverage active (€75,000) | 2–3 business days |
| Check IMPIC registry (civil engineers) | Search [impic.pt](https://www.impic.pt/impic/pt-pt/consultar/listagem-eng-civis-lei252018_2) [^22^] | Confirms Lei 25/2018 registration for construction roles | Immediate |

**Step 3: Verify Signing Authority**
Not all OE members have equal signing authority. The OE classifies members by professional title: [^23^]

| **Title** | **Signing Authority Level** | **Relevance for Inspection** |
|---|---|---|
| Conselheiro (239 members) | Full | Highest authority; can sign all report types |
| Engenheiro Nível 1 (4,711 members) | Full | 5-year degree equivalent; full signing authority |
| Engenheiro Nível 2 (45,921 members) | Full | Post-Bologna integrated Master's; full signing authority |
| Sénior (10,465 members) | Full + enhanced credibility | 10+ years experience; preferred for court testimony |
| Especialista (1,391 members) | Full + specialization | Specialist title in specific engineering domain |
| Membro Efetivo (general) | Varies | Must hold one of above titles for full signing authority |

For InspectOS's purposes, **Engenheiro Nível 1, Nível 2, Sénior, and Especialista** all possess sufficient signing authority for inspection reports. The **Sénior** and **Especialista** titles add credibility weight in court proceedings but are not legally required for report validity.

**Step 4: Confirm Professional Liability Insurance**
The OE provides **free professional liability insurance** to all effective members through **Ageas Portugal**, policy number **8410226152**. [^105^][^106^] However, the coverage level depends on whether the member has requested the **professional exercise declaration** (declaração para exercício profissional):

| **Insurance Status** | **Coverage** | **Sufficient for InspectOS?** |
|---|---|---|
| With professional exercise declaration | €75,000 per incident/year [^106^] | **Yes** — standard coverage |
| Without declaration | €1,000 per incident/year [^106^] | **No** — insufficient for inspection liability |
| Enhanced coverage (optional) | €75,000–€1,000,000 [^106^] | **Yes** — recommended for senior inspectors |

The candidate must request their **declaração de seguro** from Ageas by emailing **engenheiros@ageas.pt** or calling **21 794 30 20 / 22 608 11 20** (weekdays, 8:30–19:00). [^109^] InspectOS should retain a copy of this declaration in the inspector's personnel file.

### 1.3 Red Flags — Automatic Disqualification

| **Red Flag** | **Why It Matters** | **Action** |
|---|---|---|
| Cannot provide OE membership number | Unverifiable credentials; report may lack legal validity | **Disqualify immediately** |
| OE membership suspended or expired | Cannot legally sign inspection reports | **Disqualify; candidate must reactivate first** |
| Specialty is not Civil Engineering | May lack building inspection competence | **Conditional: assess case-by-case; electrotechnical acceptable for systems-only inspections** |
| No professional exercise declaration | Insurance coverage only €1,000 — insufficient | **Require candidate to request declaration before proceeding** |
| Ethical sanctions in past 5 years | Compromised professional standing | **Disqualify** |
| OE membership obtained via non-standard route | Credential may be challenged | **Enhanced verification via OE regional office** |

---

## 2. Gate 2: Brazilian Reciprocity Protocol

### 2.1 The CREA-to-OE Transfer Process

The **Termo de Reciprocidade CONFEA-OEP** (signed September 29, 2015, with Termo Complementar 3 added February 2025) [^15^][^17^] creates a streamlined pathway for Brazilian engineers to obtain OE registration without diploma revalidation. InspectOS can leverage this pathway both for candidates already in Portugal and for candidates InspectOS recruits from Brazil.

### 2.2 Document Checklist and Timeline

| **Phase** | **Required Documents** | **Responsible Party** | **Timeline** |
|---|---|---|---|
| **Phase 1: Pre-Qualification** (InspectOS internal) | CREA registration proof, academic transcript (3,600+ hours), passport copy, ethical standing certidão | InspectOS HR | 1–3 days |
| **Phase 2: CONFEA Application** | Formulário de Registro no Sistema OEP, authenticated passport copy, authenticated professional card copy, photograph | Candidate (via CREA state chapter) | CONFEA analysis: up to 90 days [^16^] |
| **Phase 3: CONFEA to OEP** | CONFEA issues certidão específica (R$ 59.42 fee) [^16^]; dossier forwarded to OEP | CONFEA | 2–5 days after approval |
| **Phase 4: OEP Analysis** | OEP reviews dossier for compatibility with Portuguese engineering standards | OEP | 30–60 days |
| **Phase 5: OEP Admission** | Candidate pays OEP fees and anuidade; receives cédula profissional | Candidate + OEP | 7–14 days |
| **TOTAL** | | | **90–180 days end-to-end** |

### 2.3 Common Rejection Reasons and Mitigation

| **Rejection Reason** | **Frequency** | **Mitigation Strategy** |
|---|---|---|
| Coursework hours below 3,600 | Common for older or non-standard degrees | Request candidate obtain supplementary coursework documentation from university |
| CREA registration not active or in arrears | Common | Require candidate to regularize CREA status before application |
| Ethical sanctions within 5 years | Uncommon | Automatic disqualification; no mitigation |
| Degree not recognized as engineering equivalent | Occasional for technology degrees | Pre-screen: technology degrees (tecnólogo) are **excluded** from reciprocity [^16^] |
| Missing or improperly authenticated documents | Common | Provide candidate with document checklist; recommend consular authentication |

### 2.4 Interim Status: Can They Inspect While Pending?

**No.** Under Portuguese law, an engineer **cannot exercise the profession** (including signing inspection reports) until OE registration is complete. [^18^] The interim period between CREA application and OEP admission leaves the candidate in a regulatory gap: they are a qualified engineer under Brazilian law but cannot practice in Portugal.

InspectOS has **two options** for Brazilian candidates in this interim period:

| **Option** | **Structure** | **Compensation** | **Timeline to Full Inspection Authority** |
|---|---|---|---|
| **A: Paid internship / trainee** | Work under direct supervision of OE-registered senior inspector; assist with field work, photography, documentation; do NOT sign reports | IEFP stipend (€1,057/month for Master's) [^67^] or private trainee salary | 90–180 days (pending OEP admission) |
| **B: Contractor support role** | Same as Option A but on per-diem basis; candidate performs field support only | €100–€150/day field support rate | 90–180 days |

Both options allow InspectOS to **retain and train** the candidate while their OEP registration processes, converting them to full inspector status upon OEP admission. This "train while you wait" approach is a significant competitive advantage over employers who reject candidates pending registration.

---

## 3. Gate 3: Angolan Support Role Framework

### 3.1 Legal Structure

Angolan engineers **do not** have a reciprocity pathway equivalent to the CONFEA-OEP agreement. [^59^] They must follow the standard **DGES degree recognition process** under **Decreto-Lei nº 66/2018** [^19^], which involves individual curricular analysis by a Portuguese university and can require supplementary coursework or examinations — a **6–12+ month process** costing **€2,000–€5,000**. [^18^]

For InspectOS, the practical solution is the **contractor support role**: experienced Angolan site engineers contribute field inspection capacity under the direct supervision and signing authority of an OE-registered senior inspector. This structure is legally valid because:

- The OE-registered engineer retains **full legal responsibility** for the report
- The Angolan support engineer contributes **field observation and documentation** only
- The supervision ratio complies with OE professional liability requirements

### 3.2 Supervision Requirements

| **Parameter** | **Requirement** | **Rationale** |
|---|---|---|
| Signing authority | Only OE-registered senior inspector signs reports | Legal requirement for court admissibility |
| Supervision ratio | Maximum 3 support engineers per senior inspector | Ensures adequate oversight; adjusts based on experience |
| Field presence | Senior inspector must visit property for complex cases; may delegate routine cases to support with remote review | Balances quality and efficiency |
| Report review | Senior inspector must review and approve all report content before signature | Quality gate; prevents errors |
| Professional liability | Senior inspector's OE insurance (€75,000) covers reports they sign [^106^] | Insurance follows the signature |

### 3.3 Angolan Contractor Profile

The ideal Angolan support engineer profile for InspectOS:
- **5+ years** of site engineering experience on Angolan construction projects
- **Portuguese language fluency** (Angola's official language)
- **Practical knowledge** of concrete pathology, structural assessment, building defects
- **Smartphone/tablet competency** for digital documentation
- **Valid Portuguese work authorization** (via CPLP visa or other pathway)

---

## 4. Gate 4: Trial Inspection Standard

### 4.1 Standardized Trial Inspection Scenario

Every candidate who passes Gates 1–3 must complete a **standardized trial inspection** before receiving approval to conduct independent inspections. The trial is designed to evaluate **technical competence, report quality, and attention to detail** under realistic conditions.

**Trial Inspection Parameters:**

| **Parameter** | **Specification** |
|---|---|
| **Property type** | Urban residential apartment or townhouse (80–150 m²) |
| **Property age** | 15–40 years (typical of InspectOS client properties) |
| **Location** | Within 30 minutes of InspectOS office (Lisbon or Porto) |
| **Duration** | 2–3 hours on-site + 4–6 hours for report writing |
| **Report deadline** | 48 hours from site visit |
| **Deliverable** | Full inspection report using InspectOS template format |
| **Evaluation panel** | 2 senior InspectOS inspectors + 1 operations manager |

### 4.2 Embedded Defects Checklist

The trial property must contain **at least 8 pre-planned defects** across six categories, which the candidate is expected to identify, classify, and document:

| **Category** | **Defect Type** | **Severity** | **What Candidate Must Do** |
|---|---|---|---|
| Structural | Visible crack in load-bearing wall | Functional/Significant | Identify, measure, photograph, classify severity, assess structural significance |
| Humidity | Stain/mold in bathroom or exterior wall | Functional | Identify source, assess extent, recommend further investigation |
| Electrical | Non-compliant electrical panel (no differential) | Critical | Identify non-compliance with RTIEBT, flag as safety issue |
| Gas | Missing or expired gas inspection certificate | Critical | Identify, reference DL 97/2017 requirement |
| Covering/Envelope | Damaged roof membrane or flashing | Functional | Identify, assess water ingress risk, photograph |
| Urbanism/Compliance | Unregistered extension or modification | Significant | Compare physical structure to registered description, identify discrepancy |
| Systems (HVAC) | Non-functional or improperly installed heating | Functional | Identify, assess impact, recommend repair/replacement |
| Finishes | Significant degradation of flooring or plaster | Cosmetic/Functional | Document, assess extent |

### 4.3 Evaluation Rubric

The candidate is scored on a **100-point scale** across five dimensions:

| **Dimension** | **Weight** | **Excellent (90–100)** | **Satisfactory (70–89)** | **Conditional Pass (50–69)** | **Fail (<50)** |
|---|---|---|---|---|---|
| **Defect Detection Rate** | 30% | Identifies 7+ of 8 embedded defects | Identifies 5–6 defects | Identifies 3–4 defects | Identifies <3 defects |
| **Severity Classification** | 20% | All severity classifications correct | 80%+ correct | 60–79% correct | <60% correct |
| **Report Quality** | 25% | Professional, complete, well-structured; photos clear and well-labeled | Minor gaps; generally professional | Significant gaps; needs revision | Incomplete or unprofessional |
| **Regulatory Knowledge** | 15% | Correctly references relevant Portuguese regulations (DL 10/2024, RTIEBT, DL 97/2017) | References most relevant regulations | Limited regulatory references | No regulatory references |
| **Communication** | 10% | Clear, precise language; actionable recommendations | Generally clear; minor ambiguities | Some unclear sections; vague recommendations | Unclear, confusing, or incomplete |

### 4.4 Pass/Conditional/Fail Determination

| **Score** | **Decision** | **Next Step** |
|---|---|---|
| **80–100** | **Pass** | Approve for independent inspections with standard QA oversight |
| **65–79** | **Conditional Pass** | Require 2–4 additional supervised inspections; re-evaluate |
| **50–64** | **Conditional Fail** | Require structured retraining; re-trial in 30 days |
| **Below 50** | **Fail** | Disqualify from inspector role; may offer trainee position if potential evident |

---

## 5. Gate 5: Insurance & Liability Framework

### 5.1 OE Group Insurance (Primary Coverage)

The OE's group professional liability insurance through **Ageas Portugal** (policy 8410226152) provides the **foundation of InspectOS's insurance architecture**. [^105^][^106^] Key parameters:

| **Parameter** | **Value** | **Notes** |
|---|---|---|
| Insurer | Ageas Portugal, S.A. [^105^] | Major Portuguese insurance group |
| Policy number | 8410226152 [^105^] | Annual renewal (July–June cycle) |
| Coverage per member | €75,000/incident/year [^106^] | With professional exercise declaration |
| Base coverage (no declaration) | €1,000/incident/year [^106^] | Insufficient for inspection work |
| Maximum enhanced coverage | €1,000,000 [^106^] | Optional individual upgrade |
| Coverage scope | Portugal + Autonomous Regions; worldwide except USA/Canada [^106^] | |
| Covered activities | Peritagens e diagnósticos (inspections and diagnostics) explicitly listed [^108^] | |
| Deductible | 10% of claim, max €1,000 [^108^] | Applies to OET policy; OE policy terms may vary |

**Critical action:** Every inspector must request their **declaração de seguro** from Ageas before conducting their first inspection. InspectOS must retain a copy and verify annual renewal.

### 5.2 InspectOS Corporate Insurance Layer

Beyond individual OE insurance, InspectOS should maintain:

| **Insurance Type** | **Purpose** | **Recommended Coverage** |
|---|---|---|
| Corporate Professional Liability | Covers claims against InspectOS as an entity | €500,000–€1,000,000 |
| General Liability | Covers property damage or bodily injury during inspections | €250,000–€500,000 |
| Cyber Liability | Covers data breaches of client property information | €100,000–€250,000 |
| Director & Officer | Covers management liability | €250,000–€500,000 |

### 5.3 Employee vs Contractor Insurance Implications

| **Inspector Type** | **Insurance Structure** | **Key Consideration** |
|---|---|---|
| **Full-time employee** | OE individual insurance (primary) + InspectOS corporate (secondary) | Employer may need additional coverage for acts within scope of employment |
| **Contractor (recibo verde)** | OE individual insurance (primary) + own professional insurance if enhanced | Contractor must maintain active OE membership and insurance; InspectOS verifies annually |
| **Intern/Trainee** | Covered under supervising inspector's insurance while in training | No independent signing authority; supervisor assumes liability |
| **Angolan support** | Covered under supervising OE-registered inspector's insurance | Support role only; no independent liability |

---

## 6. Gate 6: Background & Reference Protocol

### 6.1 Minimum Viable Reference Check

The reference check process for InspectOS inspectors should focus on **technical competence and inspection quality** rather than generic personality fit. The following questions are designed to reveal inspection-specific capabilities:

**Questions for Previous Employers/Clients:**

| **Question** | **What It Reveals** | **Red Flag Response** |
|---|---|---|
| "Describe the most complex building defect this engineer identified that others missed." | Attention to detail; diagnostic skill | "Nothing comes to mind" or generic answer |
| "How would you rate the quality of their technical reports on a 1–10 scale? What would have made them a 10?" | Report writing competence; self-awareness of quality gaps | Score below 6; complaints about clarity or completeness |
| "Have any of their reports been challenged legally or technically? How did they respond?" | Resilience under scrutiny; professional integrity | Reports frequently challenged; defensive response to criticism |
| "Did they consistently meet deadlines for report delivery?" | Reliability; time management | Pattern of missed deadlines |
| "Would you hire them again for inspection work?" | Overall assessment | Hesitation or qualified "no" |

**Questions for Academic References (for juniors/interns):**

| **Question** | **What It Reveals** |
|---|---|
| "How did this student perform in structural analysis coursework?" | Foundation knowledge for building inspection |
| "Did they demonstrate attention to detail in laboratory or project work?" | Precision — critical for inspection |
| "How did they handle constructive criticism of their work?" | Growth mindset; coachability |

### 6.2 Background Check Requirements

| **Check Type** | **Required For** | **Method** | **Timeline** |
|---|---|---|---|
| Criminal record (certidão de registo criminal) | All inspectors with signing authority | Request from candidate; verify via Portuguese Justice system | 5–10 days |
| OE ethical standing | All OE-registered candidates | Verify via OE regional office | 1–2 days |
| Previous employment verification | All full-time and senior contractors | Contact previous employers directly | 3–7 days |
| Academic credential verification | All candidates (especially Brazilian/Angolan) | Verify with issuing institution | 7–14 days |
| Driving record | All field inspectors (vehicle use) | Request from candidate | 2–3 days |

---

## 7. Gate 7: Technical Proficiency Assessment

### 7.1 Digital Tool Stack Competency

InspectOS inspectors use a **digital platform** for scheduling, report generation, photo documentation, and GPS logging. [^121^] Minimum technical literacy thresholds:

| **Tool Category** | **Specific Tools** | **Minimum Competency** | **Assessment Method** |
|---|---|---|---|
| **InspectOS Platform** | Web-based inspection app | Navigate interface, complete digital checklist, upload photos | Live demonstration during onboarding |
| **Photo Documentation** | Smartphone camera + cloud upload | Take clear, well-composed photos; geotag; upload to platform | Trial inspection photo review |
| **GPS/Location** | Google Maps, platform GPS logging | Navigate to properties; log inspection location | Live demonstration |
| **Report Writing** | InspectOS template (digital) | Complete all fields; write clear, factual descriptions | Trial inspection report evaluation |
| **PDF/Document Handling** | Adobe Reader, digital signature | Open, review, and digitally sign reports | Live demonstration |
| **Communication** | Email, WhatsApp, platform messaging | Respond to client and office communications within 24 hours | Observation during trial period |

### 7.2 Portuguese Building Code Knowledge

Inspectors must demonstrate working knowledge of the regulatory framework governing Portuguese construction and inspection:

| **Regulation** | **Relevance** | **Knowledge Level Required** |
|---|---|---|
| **DL 10/2024 (Simplex Urbanístico)** [^114^][^118^] | Defines urban planning liability shift to buyers; creates inspection demand | Understand key provisions; explain to clients |
| **Lei 31/2009** [^116^] | Qualification requirements for technical construction roles | Know engineer's role and limitations |
| **RTIEBT** (Portaria 949-A/2006) | Electrical installation regulations | Identify non-compliance in electrical systems |
| **DL 97/2017** | Gas installation safety regulations | Verify gas inspection certificates; identify safety issues |
| **DL 101-D/2020** | Energy certification system | Understand energy certificate requirements |
| **RGEU** (until June 2026) / New regime | General urban building regulations | Reference for construction compliance assessment |

---

## 8. Quality Gates Decision Tree

```
CANDIDATE FIRST CONTACT
         |
    [GATE 1: OE Verification]
    - OE membership confirmed? 
    - Signing authority verified?
    - Insurance declaration obtained?
         |
    YES / NO
    |       \
    |    [Disqualify or redirect to trainee]
    |
[GATE 2: Profile-Specific Check]
    |
    ├── Portuguese candidate → Proceed to Gate 3
    ├── Brazilian candidate → Verify CREA status → If eligible, proceed;
    │   if pending OEP admission → Interim trainee role → Proceed to Gate 3
    └── Angolan candidate → No OE pathway → Support role only →
        Supervised by OE-registered senior → Proceed to Gate 3 (modified)
    |
[GATE 3: Background & Reference Check]
    - Criminal record clear?
    - OE ethical standing clean?
    - References satisfactory?
    |
    YES / NO
    |       \
    |    [Disqualify]
    |
[GATE 4: Technical Proficiency Assessment]
    - Digital tools competency?
    - Building code knowledge?
    |
    PASS / FAIL
    |       \
    |    [Retrain and reassess or disqualify]
    |
[GATE 5: Trial Inspection]
    - Score 80+ → FULL APPROVAL
    - Score 65–79 → CONDITIONAL (2–4 supervised inspections)
    - Score 50–64 → RETRAIN + RE-TRIAL
    - Score <50 → DISQUALIFY
    |
[APPROVED INSPECTOR STATUS]
    - OE insurance verified
    - Trial inspection passed
    - Report template trained
    - QA audit schedule assigned
```

---

## 9. Compliance Risk Matrix

| **Risk** | **Likelihood** | **Impact** | **Mitigation Action** | **Owner** |
|---|---|---|---|---|
| Inspector's OE membership lapses during employment | Medium | **Critical** — reports lose legal validity | Monthly OE status verification; automated renewal reminders | Operations Manager |
| Brazilian candidate inspects before OEP admission complete | Low | **Critical** — illegal practice; liability exposure | Explicit contract clause prohibiting inspection before OEP admission; supervisor oversight | Compliance Lead |
| Insurance declaration not obtained (€1,000 coverage only) | Medium | **High** — insufficient coverage for claims | Mandatory insurance verification before first inspection; annual renewal check | HR/Operations |
| Angolan support engineer signs report without OE supervision | Low | **Critical** — report inadmissible; fraud risk | System-enforced: only OE-registered profiles can digitally sign reports | Tech/Platform |
| Trial inspection property defects too obvious/hard | Low | **Medium** — unfair evaluation | Standardized trial properties with calibrated defect difficulty | Quality Manager |
| Reference check reveals undisclosed ethical issue | Low | **High** — reputational damage | Multi-reference protocol; direct OE ethical standing verification | HR |
| Report template not followed; inconsistent quality | Medium | **Medium** — brand damage; client complaints | Mandatory template training; random audit program | Quality Manager |

---

## 10. Implementation Checklist

### Pre-First-Hire Actions (Week 1)

- [ ] Create OE verification SOP document
- [ ] Register for access to IMPIC registry search
- [ ] Establish contact with OE North and South regional offices
- [ ] Create document template for insurance declaration request (to Ageas)
- [ ] Identify 2–3 trial inspection properties (with embedded defects)
- [ ] Build digital trial inspection evaluation form (100-point rubric)
- [ ] Create reference check question template
- [ ] Establish relationship with Ageas for bulk insurance queries
- [ ] Draft contract clauses for Brazilian interim trainees
- [ ] Draft contract clauses for Angolan support roles

### Per-Candidate Actions

- [ ] Gate 1: Verify OE membership and signing authority
- [ ] Gate 1: Obtain and file insurance declaration
- [ ] Gate 2: Profile-specific verification (CREA for Brazilians, DGES for Angolans)
- [ ] Gate 3: Conduct background and reference checks
- [ ] Gate 4: Assess digital tool competency
- [ ] Gate 5: Schedule and conduct trial inspection
- [ ] Gate 5: Evaluate trial using 100-point rubric
- [ ] Gate 5: Document decision (Pass/Conditional/Fail)
- [ ] Post-Approval: Add to QA audit schedule
- [ ] Post-Approval: Issue inspector credentials and platform access
