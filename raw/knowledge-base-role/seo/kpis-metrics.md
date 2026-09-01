---
id: kpis-metrics-seo
title: "SEO KPIs — Healthy SEO & DR Performance"
category: "KPIs & Metrics"
domain: "SEO"
status: "Active"
last_updated: "2026-07-23"
tags: ["seo", "kpi", "dr", "metrics"]
summary: "The metrics that define healthy SEO and DR performance, with current baselines as of 2026-07-23."
data_source: "Ahrefs API, pulled live 2026-07-23"
---

# SEO KPIs — Healthy SEO & DR Performance

## Authority / backlink KPIs

- **Domain Rating (DR)** — 100-point authority scale. Baseline: InspectOS 6.0, HomeOS 2.8.
- **Referring domains (live)** — unique domains currently linking in. Baseline: InspectOS 11, HomeOS 474.
- **Referring domains (live vs. all-time) ratio** — a large gap signals link churn/loss, not just growth. Baseline: InspectOS 11/12 (stable), HomeOS 474/771 (61% retained — worth monitoring).
- **Backlinks (live)** — total link count. Baseline: InspectOS 131, HomeOS 1,205.
- **Spam-flagged referring domains** — count of domains in the profile marked `is_spam: true` by Ahrefs. Target: 0. Current: HomeOS has at least 1 (`za.com`, DR 90) in its top-10 by DR — needs a disavow review.

## Visibility / ranking KPIs

- **Organic keywords ranked (top 100)** — Baseline: InspectOS 11, HomeOS 0.
- **Keywords in top 3 / top 10** — tighter ranking bands that convert to real traffic. Baseline: InspectOS 0 keywords in top 3 (best position is 6, for "home inspection services").
- **Average position on priority terms** — track movement over time per target keyword (e.g. "adene," currently position 19 for InspectOS).

## Traffic KPIs

- **Estimated monthly organic traffic** — Baseline: InspectOS 48, HomeOS 0.
- **Estimated monthly organic traffic value** — Baseline: InspectOS $0.61, HomeOS $0.

## Technical health KPIs

- **Site Health Score** (Ahrefs Site Audit) — Baseline: InspectOS 66/100, HomeOS 85/100.
- **URL error count** — Baseline: InspectOS 190 of 553 crawled, HomeOS 41 of 275 crawled.
- **Crawl freshness** — date of last completed crawl; stale crawls mean stale health scores. Baseline: InspectOS 2026-07-20, HomeOS 2026-07-23.

## Content/page KPIs

- **Traffic concentration** — % of total organic traffic coming from a single page. Baseline: InspectOS is currently at ~100% concentration (`/en/home-inspections` carries all 48 visits) — a single-page dependency worth watching as more pages should start contributing.
- **Keywords per ranking page** — pages ranking for only 1 keyword vs. pages ranking for a cluster of related terms; more keywords per page generally signals stronger topical relevance.

## Guardrail KPI

- **% of referring domains flagged as manipulative/spam** — should stay at or near 0 regardless of DR. A high-DR spammy domain (like HomeOS's `za.com` link) is not a quality signal and shouldn't be treated as one.

## How to refresh this file

All baseline figures above were pulled live from Ahrefs on 2026-07-23 (InspectOS project ID `9596383`, HomeOS project ID `10072010`). These are point-in-time numbers, not static facts — re-pull before using them to justify a new decision, per the standing rule of verifying current data rather than working from memory of a prior check-in.
