---
title: "Source — Growth & Operations Role Knowledge Base"
type: source
tags: []
status: evergreen
created: 2026-07-23
updated: 2026-07-23
sources: []
brand: shared
verified: false
---

# Source — growth & operations role knowledge base

A 21-file internal "role KB" (`raw/knowledge-base-role/`) documenting a single Skaler-side role's ownership across three domains: SEO strategy/direction for InspectOS + HomeOS, Workspace Access & Credentials (1Password administration), and Tooling & Billing ownership. Structured domain-first, five category files per domain (Responsibilities, Skills & Expertise, Capabilities, Access & Permissions, Decision Authority & Guardrails), plus SEO adds Operations & Status, KPIs & Metrics, and four Platform Guides (Ahrefs, GA4, GTM, Campaign URL Builder).

No GDPR concern: the only named individuals are internal team members (Paul, Filipe, Petra, Juan) referenced by role-holding fact, not client/buyer data — consistent with how [[hiring-compensation]] and the rest of the hiring cluster already handle internal names.

## Extraction status

Fully ingested. Filed as:
- [[ops-role-hub]] — hub for this cluster.
- [[ops-seo-ownership]] — SEO domain: responsibilities, skills, capabilities, access, guardrails, live Ahrefs status and KPI baselines (pulled 2026-07-23).
- [[ops-workspace-access]] — 1Password/credentials domain: seat structure, access-granting authority, the unwritten-hygiene-policy gap.
- [[ops-tools-billing]] — Tooling & Billing domain: Coda.io confirmed as the wiki tool; several fields (spend threshold, payment methods, renewal dates) remain placeholders in the source.
- Platform/tool entities: [[ahrefs]], [[google-analytics]], [[google-tag-manager]], [[campaign-url-builder]].

## Notable data points

- **InspectOS SEO is technically weak**: Site Health 66/100, 190 of 553 crawled URLs have errors, DR 6.0, 48 est. monthly organic visitors, ~100% traffic concentration on one page (`/en/home-inspections`).
- **HomeOS has a large but stale backlink base with zero rankings**: 474 live referring domains, DR 2.8, 0 keywords ranked, 0 organic traffic — 88% of all-time backlinks (13,374 → 1,205 live) are gone. One flagged spam referring domain, `za.com` (DR 90), pending disavow review.
- A concrete, low-effort opportunity exists: InspectOS ranks position 19 (page 2) for "adene" (1,600 searches/mo), directly tied to its ADENE certificate service page.
- **1Password Families plan is at its 5-seat cap** (Paul, Filipe, Petra, Juan, `hello@inspectos.pt`) with no written 2FA / offboarding-SLA / access-log policy — flagged as an open gap, not yet a decision.
- **Tools & Billing domain is incomplete in the source itself**: spend-approval threshold, payment methods, and renewal dates are placeholders (`TBD` / `[fill in]`) across all three category files. This is a genuine gap in the source, not an ingest omission.

## Gaps carried forward

Added to the wiki's open-items tracking (see each ops page): tools-billing spend threshold undefined, workspace-access hygiene policy undefined, HomeOS backlink-loss cause unexplained. None resolved here — flagged for a decision, not guessed at.
