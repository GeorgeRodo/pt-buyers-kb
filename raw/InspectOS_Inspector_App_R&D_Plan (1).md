# InspectOS Inspector App — Research & Development Plan
## June 2026 | Strategic Product & Engineering Roadmap

---

## 1. Executive Summary

This document is the **Research & Development Plan** for the InspectOS Inspector App — the mobile-first, field-native software platform that enables inspectors, engineers, and certified professionals to conduct Property Condition Assessments (PCA) in Portugal and, eventually, across Europe.

**Strategic Context:** InspectOS operates at the intersection of three converging forces:
1. **Regulatory tailwind:** Portugal's Simplex Urbanístico (DL 10/2024) eliminated mandatory municipal verification at sale, shifting 100% liability for hidden defects, illegal construction, and missing certificates to the buyer. From August 2026, real estate agents become liable for advising buyers — creating mandatory demand for independent, documented property condition verification.
2. **Standards opportunity:** ISO/IEC 17020:2026 was published in March 2026, simplifying the independence model (Type A / Type non-A) and embedding risk-based thinking. InspectOS can architect its platform and accreditation path directly against this new standard, avoiding legacy baggage.
3. **Competitive gap:** Existing tools (Spectora, Property Inspect, Inspecto, WeProov) are either US-centric, UK-rental-focused, or generic documentation platforms. None combine: (a) open PCA methodology, (b) proprietary PCS data moat, (c) EU regulatory compliance, and (d) AI-native field inspection.

**Core Thesis:** Build the inspector app as the **field operating system for property condition** — not just a report writer, but the tool that enforces methodology consistency, captures structured data for the PCS database, and makes every inspector more competent, faster, and defensible.

---

## 2. Competitive Intelligence (June 2026)

### 2.1 Direct Competitors — Feature & Pricing Matrix

| Platform | Market | Pricing | Mobile | AI | Offline | API | EU Focus | Key Weakness |
|---|---|---|---|---|---|---|---|---|
| **Spectora** | US home inspection | $109/mo | iOS/Android | Comment Assist | Yes | **No** | No (English only) | No API, US-only templates, high price |
| **Property Inspect** | UK/EU multi-sector | £45–£595/mo | iOS/Android | Inspect AI (£75/mo) | Yes | Enterprise only | Partial | Complex setup, no video AI, steep learning curve |
| **Inspecto** | UK lettings | Freemium | iOS/Android | **Video AI** (frame-by-frame) | Limited | No | UK only | Newer (2024), small marketplace, no EU expansion |
| **WeProov** | EU rental/insurance | Per-inspection | iOS/Android | Photo + notes | Yes | Limited | Yes (FR/ES) | Limited customization, basic reporting |
| **HomeGauge** | US | $89/mo | iOS/Android | Limited | Yes | No | No | Dated interface, US-centric |
| **InspectorData** | US | $69.99/mo | iOS/Android | Photo analysis, comment gen | Yes | No | No | 90-day trial, US-only |
| **RapidEye** | STR damage detection | Contact | Web | **Baseline comparison AI** | N/A | Yes (Breezeway) | No | STR-only, no field inspection workflow |
| **Snap Inspect** | Multi-sector | Varies | iOS/Android | Admin/reporting AI only | Yes | Limited | No | AI is not image-analysis; just voice-to-text + auto-assign |

### 2.2 Competitive Insights

**Spectora** dominates US home inspection mindshare with 917+ verified reviews. Users praise on-site report completion, photo editing, and mobile sync. Pain points: high cost ($109/mo), no API, English-only, per-user fees escalate quickly, occasional bugs and slow performance. Tech stack: Ruby on Rails backend, React frontend, Cloudflare, Google Analytics. No public ISO or SOC 2 certifications.

**Property Inspect** is the closest European analog. It serves residential, commercial, student, and facilities management. Offers 200+ templates, offline mobile, branded reports, and "Inspect AI" (launched 2026) for assisted reporting. Pricing starts at £45/mo (Solo, 100 properties) up to £595/mo (Enterprise, 1000+ properties). Weaknesses: complex setup, no video AI, primarily manual process, higher price point for multi-user teams.

**Inspecto** (UK, launched 2024) is the most AI-native competitor. It replaces manual photography with video walkthroughs; AI analyzes footage frame-by-frame, identifies rooms, catalogs fixtures, and generates ARLA-compliant PDF reports in under 10 minutes. Free plan for 3 properties. This is the benchmark for AI inspection speed — but it is UK-only and rental-focused.

**WeProov** focuses on damage/condition documentation for insurance and rental. Mobile photo capture, notes, professional reports. EU-based but limited customization and no deep regulatory alignment.

**RapidEye / Paraspot / ItemWise / Inspect360** represent the "true AI damage detection" category — these use baseline photo/video comparison to automatically flag new damage, stains, missing items. Only 4 out of 12 evaluated "inspection" vendors actually perform automated damage detection; the rest are documentation tools. This is a critical distinction: most "AI inspection" marketing is hype.

### 2.3 InspectOS Differentiation Opportunity

| Dimension | Competitors | InspectOS Target |
|---|---|---|
| **Methodology** | Proprietary templates, closed standards | Open PCA standard (vendor-neutral) + proprietary PCS scoring |
| **Regulatory** | Generic compliance, state/US/UK templates | Portugal-specific (Simplex, EPC, seismic, BRP), EU-expandable |
| **AI Depth** | Comment assist, basic photo analysis, or video AI only | Multi-modal: photo defect detection + voice-to-text + predictive risk scoring + baseline comparison |
| **Data Moat** | Siloed per-inspector reports | Centralized PCS database with historical + outcome-linked claims data |
| **Accreditation** | Software only; no inspection body accreditation | Platform built for ISO 17020:2026 Type A path + IPAC accreditation |
| **Pricing** | $49–$109/mo + per-inspection fees | €49–€79/mo unlimited, transparent, no per-report fees |
| **Offline** | Partial or limited | Full offline with secure local storage, GDPR-compliant deletion |

---

## 3. Regulatory & Standards Environment

### 3.1 Portugal — Simplex Urbanístico & Agent Liability (August 2026)

**Decreto-Lei 10/2024 (in force 1 Jan 2024)** eliminated the mandatory *licença de utilização* for property sales. The municipality no longer verifies urban planning compliance before sale. The buyer inherits all liability for illegal construction, hidden defects, and missing certificates post-*escritura*.

**Critical August 2026 Development:** Real estate agents become liable for advising buyers. Agents must now recommend independent inspections to reduce their own liability exposure. This creates **mandatory, inelastic demand** for property condition assessment services — exactly what InspectOS provides.

**InspectOS Positioning:**
- The "Simplex Safe" inspection (47 checkpoints, bilingual report, 48-hour delivery, cost estimates per anomaly) is the market-validated product.
- The inspector app must encode these 47 checkpoints into guided, mandatory workflows that ensure every inspection is complete and defensible.
- Integration with ADENE (energy certificate registry), municipal project archives, and notary systems is a competitive moat.

### 3.2 EU AI Act — Compliance Architecture (August 2026 Deadline)

The EU AI Act's **high-risk requirements apply from August 2026**. Property inspection AI must be classified carefully:

| AI Use Case | Likely Risk Class | Rationale | Compliance Required |
|---|---|---|---|
| Photo defect detection / annotation | **Limited Risk** | Transparency obligations only; human inspector reviews all findings | AI disclosure labels, human oversight UI |
| Automated condition scoring for buyer reports | **Limited Risk** | Preparatory task to human assessment (Art. 6(3)(d)) | Documentation of non-high-risk assessment |
| Risk scoring for bank loan/insurance underwriting | **High Risk** (Annex III) | Access to essential services / employment-like decisions | Conformity assessment, technical documentation, human oversight, post-market monitoring, registration in EU database |
| Predictive maintenance from PCS trends | **Minimal Risk** | No direct decision impact on individuals | Existing legislation only |

**InspectOS AI Strategy:**
- Build a **"human-AI partnership"** model: AI suggests, humans decide. Every AI-flagged finding requires inspector confirmation before entering the report.
- Document the non-high-risk assessment for photo/condition AI (Art. 6(3) derogation).
- If offering PCS analytics to banks/insurers, treat that module as high-risk and implement full conformity assessment (technical docs, risk management, data governance, human oversight, accuracy testing, cybersecurity).
- Use EU-friendly AI providers (Mistral, local models) where possible; for OpenAI/Anthropic, ensure strong Data Processing Agreements with EU data residency.

### 3.3 ISO/IEC 17020:2026 — Accreditation Path

**Published March 2026.** Key changes from 2012 edition:
- **Simplified independence model:** Type A / Type non-A (instead of A/B/C). Type A = fully independent; Type non-A = all others with documented impartiality risk management.
- **Risk-based thinking** embedded throughout management system requirements.
- **Enhanced impartiality and confidentiality** requirements with explicit documentation.
- **Digital transformation and remote inspection** provisions explicitly included.
- **Transition period:** 3 years (until March 2029) for existing accredited bodies; new applicants assessed against 2026 edition from 1 Jan 2027.

**InspectOS Implication:**
- The platform must be the **QMS (Quality Management System) engine** for the inspection body.
- Built-in features: inspector competence tracking, calibration records, audit trails, complaints/appeals module, impartiality declarations, witness audit evidence capture.
- Separate the SaaS platform entity from the accredited inspection body entity for Type A independence.
- Target IPAC (Portuguese accreditation body) assessment by Q2 2027.

### 3.4 EPBD & Energy Certificates (2026–2030)

The Energy Performance of Buildings Directive (EPBD) mandates EPCs across the EU. Portugal's ADENE registry is the national system. Key requirements:
- EPC integration in inspection workflows (mandatory data capture).
- Digital Building Logbooks (EU-promoted for lifecycle data sharing) — InspectOS can position as the field data capture layer.
- Renovation Passports (EPBD 2024 revision) — long-term planning module for property improvement.
- F-rated properties purchased after 29 May 2026 have specific EPBD compliance implications that buyers must review.

---

## 4. Product Architecture & Technical Stack

### 4.1 Design Principles

1. **Mobile-first, offline-native:** Inspectors work in basements, attics, rural areas with no signal. The app must function fully offline and sync intelligently.
2. **Methodology-enforced:** The app guides the inspector through the PCA checklist; skipping steps is not allowed (configurable enforcement per accreditation level).
3. **AI-suggested, human-confirmed:** Every AI finding is a draft until the inspector taps "confirm." This satisfies EU AI Act human oversight requirements.
4. **Data moat by default:** Every inspection feeds structured data into the PCS database. The app is the data capture device.
5. **Privacy by design:** GDPR-compliant from day one — data minimization, consent management, DSAR automation, EU data residency.

### 4.2 Recommended Tech Stack (EU-Optimized)

| Layer | Technology | Rationale |
|---|---|---|
| **Mobile App** | Flutter (primary) or React Native | Cross-platform, offline-capable, excellent camera/photo handling, fast native performance. Flutter preferred for consistent UI across iOS/Android and superior offline sync architecture. |
| **Web Dashboard** | Next.js 14 (App Router) + Tailwind CSS + shadcn/ui | SEO-friendly, PWA-capable, fast rendering, excellent developer experience. |
| **Backend API** | NestJS (TypeScript) or Laravel | Structured, enterprise-grade, excellent for compliance features (audit logging, role-based access, QMS workflows). NestJS preferred for TypeScript consistency with frontend. |
| **Database** | PostgreSQL (primary) + PostGIS (geospatial) + Redis (caching/sessions) | Robust, ACID-compliant, excellent geospatial support for property location data. Row-Level Security for multi-tenant isolation. |
| **File Storage** | Scaleway Object Storage or Hetzner S3-compatible | EU-sovereign, GDPR-friendly, cost-effective. CloudFront/Cloudflare CDN for report delivery. |
| **AI/ML Pipeline** | Hugging Face (local/on-prem models for photo analysis) + OpenAI/Anthropic API (with EU DPA) for narrative generation | Local models for sensitive photo analysis (defect detection) to minimize data transfer; LLMs for report text with strict data processing agreements. |
| **Search & Analytics** | Elasticsearch or Meilisearch | Fast property and inspection history search. |
| **Queue/Background Jobs** | BullMQ (Redis) or Laravel Horizon | Async photo processing, AI analysis, report generation, email delivery. |
| **Auth & Identity** | Clerk or Auth0 with EU data residency | Fast implementation, SSO-ready, GDPR-compliant. |
| **Payments** | Stripe (EU) | EUR support, SEPA, subscription management. |
| **Hosting** | Hetzner Cloud (Germany/Finland) or Scaleway (France) | EU data residency, cost-effective, excellent for GDPR compliance. Avoid default US-centric AWS unless using Frankfurt/Paris regions explicitly. |
| **Monitoring** | Grafana + Prometheus + Sentry | Observability, error tracking, performance monitoring. |

### 4.3 System Architecture Overview

```
┌─────────────────────────────────────────────────────────────┐
│                    INSPECTOS INSPECTOR APP                   │
│  ┌─────────────┐  ┌─────────────┐  ┌─────────────────────┐  │
│  │  Flutter    │  │  Offline    │  │  AI Edge Processing │  │
│  │  Mobile App │  │  SQLite DB  │  │  (Photo analysis,   │  │
│  │  (iOS/Android)│  │  + Sync     │  │   voice-to-text)    │  │
│  └─────────────┘  └─────────────┘  └─────────────────────┘  │
└─────────────────────────────────────────────────────────────┘
                              │
                              ▼ (sync when online)
┌─────────────────────────────────────────────────────────────┐
│                    INSPECTOS CLOUD PLATFORM                  │
│  ┌─────────────┐  ┌─────────────┐  ┌─────────────────────┐  │
│  │  Next.js    │  │  NestJS API │  │  PostgreSQL +       │  │
│  │  Dashboard  │  │  (GraphQL/  │  │  PostGIS + Redis    │  │
│  │  (Web)      │  │   REST)     │  │                     │  │
│  └─────────────┘  └─────────────┘  └─────────────────────┘  │
│  ┌─────────────┐  ┌─────────────┐  ┌─────────────────────┐  │
│  │  AI Pipeline│  │  Report     │  │  PCS Database       │  │
│  │  (Hugging   │  │  Generator  │  │  (Anonymized,       │  │
│  │   Face + LLM)│  │  (PDF/Web/  │  │   Historical,       │  │
│  │             │  │   JSON)     │  │   Outcome-linked)   │  │
│  └─────────────┘  └─────────────┘  └─────────────────────┘  │
│  ┌─────────────┐  ┌─────────────┐  ┌─────────────────────┐  │
│  │  QMS Module │  │  Integration│  │  Audit & Compliance │  │
│  │  (ISO 17020)│  │  (ADENE,    │  │  (GDPR, AI Act,     │  │
│  │             │  │   PEPU,     │  │   Audit Logs)       │  │
│  │             │  │   Municipal)│  │                     │  │
│  └─────────────┘  └─────────────┘  └─────────────────────┘  │
└─────────────────────────────────────────────────────────────┘
```

---

## 5. Feature Roadmap

### 5.1 MVP (Months 1–4) — "Field-Ready PCA"

**Goal:** Enable a certified engineer to complete a full Simplex Safe inspection on-site and generate a bilingual PDF report within 48 hours.

| Feature | Priority | Description |
|---|---|---|
| **Guided PCA Workflow** | P0 | 47-checkpoint Simplex Safe checklist with mandatory completion enforcement. Cannot skip steps. Progress bar. Time tracking per section. |
| **Offline-First Mobile** | P0 | Full offline operation. SQLite local DB. Photo/video capture with geotagging, timestamps, auto-backup. Sync queue with conflict resolution. |
| **Photo & Video Capture** | P0 | Multi-shot burst, annotations (arrows, boxes, text), auto-compression, EXIF preservation. Video clips up to 60 seconds per defect. |
| **Voice-to-Text Notes** | P0 | Real-time transcription in Portuguese and English. Noise filtering for construction environments. |
| **Basic AI Photo Assist** | P1 | Auto-categorization of photos by room/area. Blur detection. Duplicate detection. |
| **Report Generator** | P0 | Professional bilingual PDF (PT/EN) with executive summary, anomaly list with cost estimates, photo evidence, and negotiation recommendations. Web report shareable URL. |
| **Inspector Auth & Profiles** | P0 | Individual inspector accounts, Ordem dos Engenheiros / Ordem dos Arquitetos certification verification, competence tracking. |
| **Admin Dashboard** | P1 | Web dashboard for scheduling, report review, team management, basic analytics. |
| **GDPR Compliance** | P0 | Consent capture, data retention policies, DSAR request handling, EU data residency. |

### 5.2 Phase 2 (Months 5–8) — "AI-Native & QMS-Ready"

| Feature | Priority | Description |
|---|---|---|
| **AI Defect Detection** | P0 | Local/on-device photo analysis to detect cracks, water damage, mold, structural anomalies. Hugging Face models. Human confirmation required before report inclusion. |
| **AI Narrative Generation** | P1 | LLM-generated defect descriptions from inspector notes + photo context. Inspector edits/approves. |
| **Baseline Comparison** | P1 | Compare current inspection photos against previous inspection baseline (if available in PCS database). Auto-flag new damage. |
| **QMS Module** | P0 | Built-in ISO 17020:2026 compliance tools: impartiality declarations, competence tracking, calibration records, complaints/appeals logging, internal audit scheduling, witness audit evidence capture. |
| **EPC Integration** | P1 | Pull EPC data from ADENE registry via API. Auto-populate energy rating in report. Flag expired/missing certificates. |
| **Municipal Integration** | P1 | Query municipal project archives (Câmara Municipal) for approved architectural projects. Auto-compare as-built vs. approved. |
| **Multi-Property Portfolio** | P1 | Dashboard for property managers/landlords with portfolio-level condition summaries, maintenance scheduling, and trend analysis. |
| **Team & Multi-Inspector** | P1 | Team scheduling, payroll splits, quality review workflows, peer review requirements. |
| **White-Label Reports** | P2 | Custom branding for partner agencies (real estate, relocation, mortgage brokers). |

### 5.3 Phase 3 (Months 9–14) — "Institutional & European"

| Feature | Priority | Description |
|---|---|---|
| **PCS API** | P0 | Machine-readable JSON API for third-party PCA providers to feed anonymized data into the PCS database. Network effect creation. |
| **Bank/Insurer Dashboard** | P0 | B2B portal for banks (collateral risk) and insurers (underwriting risk) with portfolio-level analytics, capital surprise risk scoring, and historical claim correlation. |
| **Predictive Risk Scoring** | P1 | ML model trained on PCS database + outcome data (claims, legal disputes, renovation costs) to predict property risk scores. |
| **Digital Building Logbook** | P1 | EPBD-aligned digital logbook module capturing full property lifecycle data (inspections, renovations, EPCs, maintenance). |
| **Renovation Passport** | P1 | EPBD Renovation Passport planner — recommended improvement steps with cost estimates and EPC impact projections. |
| **Multi-Country Templates** | P1 | Spain, Italy, France template packs with local regulatory checkpoints. |
| **Notary Integration** | P2 | Direct report delivery to notary systems for *escritura* inclusion. Suspensive condition clause auto-generation. |
| **Tenant Self-Inspection** | P2 | WeProov-like mode for tenants/landlords to conduct basic condition reports (move-in/move-out) with guided photo capture. |

### 5.4 Phase 4 (Months 15–24) — "Platform & Standard Dominance"

| Feature | Priority | Description |
|---|---|---|
| **Open PCA Standard Governance** | P0 | Public documentation, schema definitions, validator tools, third-party certification for PCA compliance. |
| **IPAC Accreditation Evidence** | P0 | Platform auto-generates all documentation required for IPAC Type A accreditation audits. |
| **AI Act High-Risk Module** | P0 | Full conformity assessment tooling for bank/insurance-facing AI features: technical documentation, risk management, bias testing, human oversight logs. |
| **Satellite/Drone Integration** | P1 | Roof/facade inspection via drone imagery upload + AI analysis. Satellite imagery for property context and change detection. |
| **Market Intelligence Reports** | P1 | Automated market reports: neighborhood condition trends, price-per-defect benchmarking, seismic risk maps. |

---

## 6. AI Strategy & Implementation

### 6.1 AI Feature Map

| Capability | Model Approach | Data Source | Human Oversight | Risk Class |
|---|---|---|---|---|
| **Photo auto-categorization** (room/area detection) | Lightweight CNN (MobileNet/EfficientNet) | On-device, no cloud transfer | Inspector can re-categorize | Minimal |
| **Blur/poor quality detection** | Image quality classifier | On-device | Inspector retakes photo | Minimal |
| **Defect detection** (cracks, water, mold) | Fine-tuned Vision Transformer (Hugging Face) | Cloud pipeline with EU DPA | Inspector confirms/rejects each finding | Limited |
| **Damage severity scoring** | Multi-modal (image + text) classifier | Cloud pipeline | Inspector adjusts score | Limited |
| **Baseline comparison** (new vs. old damage) | Image embedding + similarity (Siamese network) | PCS database | Inspector reviews flagged changes | Limited |
| **Voice-to-text transcription** | Whisper (local or EU-hosted) | On-device or EU server | Inspector edits transcript | Minimal |
| **Narrative generation** | LLM (Mistral Large / GPT-4 with EU DPA) | Inspector notes + photo metadata | Inspector edits/approves entire text | Limited |
| **Risk prediction** (bank/insurance) | Gradient-boosted + neural on PCS data | Anonymized PCS database + claims | Human underwriter reviews score | High Risk |
| **Cost estimation** | Regression on historical repair data | PCS database + contractor quotes | Inspector adjusts estimate | Limited |

### 6.2 EU AI Act Compliance Checklist

- [ ] **Risk classification documentation** for every AI feature (Art. 6)
- [ ] **Transparency notices** in UI: "AI-assisted finding — awaiting your confirmation" (Art. 50)
- [ ] **Human oversight UI**: Inspector must actively confirm every AI suggestion before it enters the report
- [ ] **Technical documentation** for high-risk features (risk management system, data governance, accuracy testing)
- [ ] **Post-market monitoring** plan: track AI error rates, inspector override rates, dispute outcomes
- [ ] **Registration** in EU database for high-risk AI systems (Art. 49)
- [ ] **Bias testing** for risk scoring models across property types, neighborhoods, ages
- [ ] **Cybersecurity** for AI pipelines (ENISA guidelines)

---

## 7. Data Architecture & The PCS Moat

### 7.1 Data Model (Simplified)

```
Property (unique address, geohash, ADENE EPC ref, municipal project ref)
  └── Inspection (timestamp, inspector_id, methodology_version, weather)
        ├── Checkpoint (dimension, item, status: Compliant/Non-Compliant/Requires Attention)
        ├── Photo (url, geotag, timestamp, ai_tags, inspector_confirmed)
        ├── Video (url, duration, transcript)
        ├── Finding (description, severity, estimated_cost, ai_generated, human_confirmed)
        └── Report (pdf_url, web_url, json_url, recipient_list)
  └── PCS_Score (composite_score, dimension_scores, confidence_interval, data_completeness)
  └── Historical_Claim (outcome_data, legal_dispute, repair_cost, time_to_repair)
```

### 7.2 Data Governance Principles

1. **Inspectors own their inspection data** until they choose to contribute anonymized findings to PCS.
2. **PCS database is anonymized and aggregated** — no individual property identifiable without explicit consent.
3. **Outcome data is the moat:** Partner with insurers, banks, and contractors to collect post-inspection outcomes (claims filed, repairs done, legal disputes) and link them back to inspection findings.
4. **GDPR by design:** 30-day raw photo retention (with inspector override), 7-year report retention (legal requirement), permanent anonymized PCS data.
5. **Open standard, closed data:** The PCA methodology is open and publishable; the PCS database is proprietary and access-controlled.

---

## 8. Go-to-Market & Monetization

### 8.1 Pricing Strategy

| Tier | Price | Target | Features |
|---|---|---|---|
| **Starter** | €49/mo | Solo inspectors | Unlimited inspections, 100 properties, basic AI, branded PDF reports, email support |
| **Professional** | €79/mo | Small teams | Unlimited inspections, 250 properties, full AI suite, team scheduling, interactive web reports, phone support |
| **Enterprise** | €245/mo | Multi-inspector firms | 500+ properties, white-label, API access, CRM integrations, priority support |
| **Institutional** | Custom | Banks, insurers, PMs | PCS analytics, portfolio dashboards, custom ML models, SOC 2 + ISO 27001, dedicated CSM |

**Principles:** No per-inspection fees (encourages volume), transparent pricing, 30-day free trial (not 5 inspections — inspectors need real field testing), annual discount.

### 8.2 Go-to-Market Sequence

1. **Month 1–3:** Pilot with 10–20 Portuguese engineers (Ordem dos Engenheiros members). Shadow inspections, iterate mobile UX.
2. **Month 4–6:** Launch in Lisbon + Porto. Partner with 3–5 relocation agents and buyer agents as referral channels. Target Simplex-aware buyers.
3. **Month 7–9:** Expand to Algarve, Cascais, Sintra, Setúbal, Braga, Coimbra. Launch "InspectOS Certified" partner program for real estate agents.
4. **Month 10–14:** Enter Spain (Madrid, Barcelona, Valencia) with localized templates. Partner with Spanish engineering associations.
5. **Month 15–24:** EU-wide expansion (Italy, France, Netherlands, Germany) with country-specific regulatory packs.

### 8.3 Partnership Strategy

| Partner Type | Value Exchange | Integration |
|---|---|---|
| **Real Estate Agents** | Liability reduction, faster sales, buyer confidence | Embedded booking widget, co-branded reports, CPCV clause templates |
| **Mortgage Brokers** | Risk reduction for loan approvals | PCS score API, pre-approval condition reports |
| **Insurance Companies** | Better underwriting data, reduced claims | Outcome data exchange, risk scoring API |
| **Banks** | Collateral risk assessment | Portfolio monitoring, capital surprise alerts |
| **Relocation Agencies** | Expat buyer protection | Bilingual reports, Simplex education, bundled services |
| **ADENE / Municipalities** | Digital compliance, EPC enforcement | Direct registry integration, data quality feedback |
| **Universities / Research** | Academic validation, talent pipeline | Joint research on seismic risk, energy efficiency |

---

## 9. Risk Assessment & Mitigation

| Risk | Likelihood | Impact | Mitigation |
|---|---|---|---|
| **Competitor copies open PCA standard** | High | Medium | Speed to market + PCS data moat + accreditation credibility. Open standard wins when we are the default platform. |
| **EU AI Act reclassifies inspection AI as high-risk** | Medium | High | Build human-in-the-loop from day one. Document Art. 6(3) derogation. Maintain legal counsel specializing in AI regulation. |
| **ISO 17020:2026 accreditation delays** | Medium | High | Start QMS implementation in Month 1. Hire regulatory affairs lead by Month 3. Budget €20–40k for accreditation. |
| **Data quality in PCS database is poor** | Medium | High | Strict methodology enforcement in app. Inspector training program. Outcome data partnerships with insurers. |
| **Inspector adoption resistance** | Medium | High | Co-design with pilot inspectors. Superior mobile UX vs. competitors. Revenue sharing on institutional contracts. |
| **US competitor enters EU with bigger budget** | Low | High | GDPR-native positioning, local language support, regulatory integration, open standard network effects. |
| **Portugal market too small** | Low | High | Design for EU expansion from day one. Multi-language, multi-currency, multi-regulatory template system. |
| **Photo AI accuracy insufficient** | Medium | Medium | Start with narrow, high-confidence defects (cracks, water stains). Expand model scope iteratively. Always require human confirmation. |
| **Offline sync bugs cause data loss** | Medium | High | Extensive testing in low-connectivity scenarios. SQLite WAL mode, checksums, retry logic, conflict resolution UI. |

---

## 10. Timeline & Milestones

### 10.1 18-Month Development Roadmap

```
Month 1-2:   Team hiring (Flutter/NestJS devs, AI engineer, regulatory lead)
             Architecture design, data model finalization
             Pilot inspector recruitment (10 engineers)

Month 3-4:   MVP mobile app (guided PCA, offline, photo capture, voice-to-text)
             Basic PDF report generation
             Web admin dashboard v1
             GDPR compliance framework

Month 5:     MVP launch with pilot inspectors (Lisbon/Porto)
             Iterate based on field feedback

Month 6:     AI defect detection v1 (cracks, water damage)
             QMS module development begins
             EPC integration (ADENE API)

Month 7-8:   AI narrative generation
             Baseline comparison v1
             Team/multi-inspector features
             Municipal integration (Câmara Municipal APIs)

Month 9:     Phase 2 launch (AI-native, QMS-ready)
             White-label reports for partners
             Portfolio dashboard for landlords

Month 10-11: PCS API development
             Bank/insurer dashboard prototyping
             Spain template pack development

Month 12:    Institutional launch (B2B portal)
             PCS database reaches 1,000+ inspection records

Month 13-14: Multi-country expansion (Spain, Italy pilots)
             Digital Building Logbook module
             Renovation Passport planner

Month 15-16: Open PCA standard documentation release
             IPAC accreditation application submission

Month 17-18: ISO 17020:2026 Type A accreditation (target)
             EU-wide marketing campaign
             Series A fundraising (if traction validates)
```

### 10.2 Key Metrics (KPIs)

| Metric | Month 6 | Month 12 | Month 18 |
|---|---|---|---|
| Active inspectors | 50 | 200 | 500 |
| Inspections completed | 500 | 3,000 | 10,000 |
| PCS database records | 500 | 3,000 | 10,000 |
| AI suggestion accuracy | 70% | 85% | 90% |
| Inspector NPS | 50 | 60 | 70 |
| Report generation time | 2 hours | 30 min | 15 min |
| Revenue (MRR) | €2,450 | €15,800 | €49,500 |
| Partner agents | 10 | 50 | 150 |
| Countries live | 1 | 2 | 5 |

---

## 11. Team & Resource Requirements

### 11.1 Core Team (Months 1–12)

| Role | FTE | Timing | Key Responsibility |
|---|---|---|---|
| **CTO / Lead Engineer** | 1 | Month 1 | Architecture, Flutter/NestJS stack, technical decisions |
| **Mobile Developer (Flutter)** | 2 | Month 1 | iOS/Android app, offline sync, camera/photo pipeline |
| **Backend Engineer (NestJS)** | 2 | Month 1 | API, database, auth, QMS module, integrations |
| **AI/ML Engineer** | 1 | Month 2 | Photo defect detection, LLM integration, model training |
| **Product Designer (UX/UI)** | 1 | Month 1 | Mobile UX, inspector workflows, dashboard design |
| **Regulatory Affairs Lead** | 1 | Month 3 | ISO 17020 path, IPAC liaison, EU AI Act compliance, ADENE integration |
| **QA Engineer** | 1 | Month 3 | Mobile testing, offline scenarios, security testing |
| **DevOps / Infrastructure** | 1 | Month 2 | EU hosting, CI/CD, monitoring, GDPR infrastructure |
| **Customer Success / Ops** | 1 | Month 4 | Inspector onboarding, support, training material |

### 11.2 Budget Estimate (Months 1–18)

| Category | Amount |
|---|---|
| Engineering team (8 FTE × 18 months, avg €5k/mo) | €720,000 |
| Infrastructure (hosting, storage, CDN, AI APIs) | €48,000 |
| ISO 17020:2026 accreditation (consultant + fees) | €35,000 |
| Legal (GDPR, AI Act, terms, IP) | €25,000 |
| Marketing & GTM (Lisbon/Porto launch) | €60,000 |
| Tools & SaaS (design, monitoring, comms) | €18,000 |
| Buffer (15%) | €142,500 |
| **Total** | **€1,048,500** |

---

## 12. Conclusion & Next Steps

The InspectOS Inspector App is not merely a software tool — it is the **field operating system for a new standard of property transparency in Europe**. By combining:

- An **open PCA methodology** that earns institutional trust,
- A **proprietary PCS data moat** that improves with every inspection,
- **AI-native field workflows** that make inspectors faster and more consistent,
- **Regulatory-first architecture** aligned with Simplex, EU AI Act, and ISO 17020:2026,
- **European data sovereignty** and GDPR-by-design,

…InspectOS can establish itself as the default infrastructure layer for property condition assessment — starting in Portugal, expanding across Europe, and eventually becoming the standard against which all competitors are measured.

**Immediate Next Steps (Week 1–2):**
1. Finalize technical architecture document and Flutter/NestJS project scaffolding.
2. Recruit 3 pilot inspectors in Lisbon for co-design sessions.
3. Draft Product Requirements Document (PRD) mapping every PCA checklist item to a software feature.
4. Initiate IPAC pre-application consultation for ISO 17020:2026 Type A accreditation timeline.
5. Set up EU-hosted development environment (Hetzner/Scaleway) with GDPR-compliant data pipeline.
6. Begin Hugging Face model evaluation for Portuguese-specific defect detection (cracks, humidity, seismic damage).

---

*Document Version: 1.0*
*Date: June 2026*
*Classification: Internal Strategic — InspectOS Product & Engineering*
