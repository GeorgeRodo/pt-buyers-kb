---
id: platform-guide-ahrefs
title: "Platform Guide — Ahrefs"
category: "Platform Guides"
domain: "SEO"
status: "Active"
last_updated: "2026-07-23"
tags: ["seo", "ahrefs", "platform-guide"]
summary: "How to work with Ahrefs' core tools, and how to read the Site Health Score benchmark."
---

# Platform Guide — Ahrefs

Full current access details and live pulled data already live in `access-permissions/seo.md`, `operations-status/seo.md`, and `kpis-metrics/seo.md`. This file covers the tool itself — what each part does and how to read it.

## The four tools actually used here

- **Site Explorer** — the entry point. Enter a domain (or a competitor's) to see its full organic search performance and backlink profile: Domain Rating, referring domains, top pages, organic keywords. Used for both self-audits and competitor checks.
- **Site Audit** — crawls a site to find technical and on-page issues (100+ checks: broken links, missing meta, crawl errors, Core Web Vitals). Produces the Site Health Score.
- **Rank Tracker** — tracks keyword position over time, by device and location. Use this to watch a specific target keyword (e.g. "adene" for InspectOS) move over weeks, not just check it once.
- **Keywords Explorer** — search volume, difficulty, and related-term research for planning new content.

## How to read the Site Health Score

Industry benchmark: **90+ is strong**, **below 70 typically signals structural issues** that could be suppressing rankings. Read current scores against this: InspectOS's last pulled score (66/100) sits below that threshold — consistent with the technical debt already flagged in `operations-status/seo.md`. HomeOS (85/100) is closer to healthy but not yet in the strong range.

## Practical workflow

1. Site Explorer first, to get the current authority/traffic snapshot for a domain.
2. Site Audit to check what's technically broken underneath that snapshot.
3. Rank Tracker to monitor movement on priority keywords after any change.
4. Keywords Explorer when scoping new content, not for daily monitoring.

## Data discipline

Ahrefs numbers move — a score pulled today is stale in a month. Re-pull before using any figure to justify a recommendation, per the standing rule already documented in `responsibilities/seo.md`.

Sources:
- [All 35 Ahrefs Features Analyzed (2026)](https://searchatlas.com/blog/ahrefs-features/)
- [Ahrefs Site Audit Tool 2026: Full Review](https://www.allable.ai/blog/ahrefs-site-audit/)
- [Ahrefs Rank Tracker 2026: Full Review](https://www.allable.ai/blog/ahrefs-rank-tracker/)
