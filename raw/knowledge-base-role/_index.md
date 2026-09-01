---
id: index
title: "Role Knowledge Base: Manifest"
last_updated: "2026-07-23"
---

# Manifest

Role-scoped knowledge base covering three responsibility domains: SEO, Workspace Access & Credentials Management, and Tooling & Billing Ownership. Structure is domain-first: each domain has its own folder, containing the category files relevant to that domain. No single "owner" field or named-individual language is used anywhere in this KB.

## seo/ (11 categories: 5 core + Operations & Status + KPIs & Metrics + 4 Platform Guides)

| Category | File | Status | Summary |
|---|---|---|---|
| Responsibilities | `seo/responsibilities.md` | Active | Strategy direction and evaluation of SEO team output; not tactical execution. |
| Skills & Expertise | `seo/skills-expertise.md` | Active | Technical SEO evaluation, backlink/competitive analysis, phase sequencing. |
| Capabilities | `seo/capabilities.md` | Active | Execute vs. delegate vs. escalate breakdown for SEO work. |
| Access & Permissions | `seo/access-permissions.md` | Active | Ahrefs (2 live projects), GSC, live site access. |
| Decision Authority & Guardrails | `seo/decision-authority-guardrails.md` | Active | Unilateral authority + hard constraints (no manipulative link tactics, geo-targeting discipline, phase discipline). |
| Operations & Status | `seo/operations-status.md` | Active | How SEO works, how it's executed, and live current status (DR, backlinks, keywords, site health) for InspectOS + HomeOS, pulled 2026-07-23. |
| KPIs & Metrics | `seo/kpis-metrics.md` | Active | Full KPI set for healthy SEO/DR performance, with current baselines. |
| Platform Guides | `seo/platform-guides/google-analytics.md` | Active | How to work with GA4: setup checklist, common misconfigurations, complements Ahrefs data. |
| Platform Guides | `seo/platform-guides/ahrefs.md` | Active | How to use Site Explorer, Site Audit, Rank Tracker, Keywords Explorer; Health Score benchmark. |
| Platform Guides | `seo/platform-guides/campaign-url-builder.md` | Active | UTM link rules already in use for InspectOS social campaigns. |
| Platform Guides | `seo/platform-guides/google-tag-manager.md` | Active | Tags/triggers/variables; always use Preview mode before publishing. |

## workspace-access/ (5 categories)

| Category | File | Status | Summary |
|---|---|---|---|
| Responsibilities | `workspace-access/responsibilities.md` | Active | 1Password (`hello@inspectos.pt`, Families, 5 seats); access-granting authority with Paul and Filipe; billing routes through Petra. |
| Skills & Expertise | `workspace-access/skills-expertise.md` | Active | Vault administration, seat-cap management, least-privilege judgment. |
| Capabilities | `workspace-access/capabilities.md` | Active | Execute (Paul/Filipe) vs. escalate (Petra approves, Filipe executes). |
| Access & Permissions | `workspace-access/access-permissions.md` | Active | 1Password Families, 5/5 seats: Paul, Filipe, Petra (Financial Manager), Juan (HR), `hello@inspectos.pt`. |
| Decision Authority & Guardrails | `workspace-access/decision-authority-guardrails.md` | Active | Access grants unilateral (Paul/Filipe); billing/seats via Petra → Filipe. **Gap flagged** — no written 2FA/offboarding-SLA/access-log policy exists yet. |

## tools-billing/ (5 categories)

| Category | File | Status | Summary |
|---|---|---|---|
| Responsibilities | `tools-billing/responsibilities.md` | Active | Owned by **Paul and Filipe**. Coda.io confirmed as the wiki tool (not Notion). |
| Skills & Expertise | `tools-billing/skills-expertise.md` | Active | *(needs further specifics)* |
| Capabilities | `tools-billing/capabilities.md` | Active | Execute: Paul/Filipe. *(spend threshold still needed)* |
| Access & Permissions | `tools-billing/access-permissions.md` | Active | Coda.io, Ahrefs, hosting, domain registrar — billing owner Paul/Filipe. *(payment method + renewal dates still needed)* |
| Decision Authority & Guardrails | `tools-billing/decision-authority-guardrails.md` | Active | Owned by Paul/Filipe. *(spend threshold still needed)* |

## Open items to resolve

- **Workspace Access — no written access-hygiene rule.** No mandatory 2FA policy, no offboarding SLA, no shared access log. Flagged in `workspace-access/decision-authority-guardrails.md`.
- **Tooling & Billing — spend threshold and full tool roster still missing.** Domain is marked Active but several fields remain placeholders (payment method, renewal dates, sign-off threshold).
- **SEO — technical debt.** InspectOS Site Health 66/100 (190 URL errors of 553 crawled). HomeOS backlink profile includes at least one Ahrefs-flagged spam domain (`za.com`, DR 90) worth a disavow review. Both flagged in `seo/operations-status.md`.

## Notes for ingestion

- Every file has YAML frontmatter (`id`, `title`, `category`, `domain`, `status`, `last_updated`, `tags`, `summary`) for metadata filtering. No `owner` field, and no named-individual references, are used anywhere in this KB — ownership/responsibility is stated by role or by the specific people who actually hold it (Paul, Filipe, Petra, Juan), never by a generic "the position holder."
- Structure is domain-first as of this version: top-level folders are domains (`seo/`, `workspace-access/`, `tools-billing/`); each contains the category files relevant to that domain. SEO has 7 categories (the two extra: Operations & Status, KPIs & Metrics); the other two domains have the original 5.
- SEO, Workspace Access, and the Operations/KPI files are fully populated with real content, including live-pulled Ahrefs data (dated 2026-07-23, re-pull before relying on it for a new decision). Tooling & Billing has real ownership/tooling facts but several fields remain placeholders pending further input.
