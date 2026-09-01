---
title: Ahrefs
type: entity
tags: [agency, inspection]
status: draft
created: 2026-07-23
updated: 2026-07-23
sources: [src-role-knowledge-base]
brand: shared
verified: false
---

# Ahrefs

SEO data platform used to evaluate authority and technical health for both InspectOS and HomeOS — see [[ops-seo-ownership]] for current live status pulled from it.

## Four tools in use

**Site Explorer** — entry point; enter a domain (own or a competitor's) for full organic search performance and backlink profile: Domain Rating, referring domains, top pages, organic keywords. **Site Audit** — crawls a site for technical/on-page issues (100+ checks: broken links, missing meta, crawl errors, Core Web Vitals); produces the Site Health Score. **Rank Tracker** — tracks keyword position over time by device/location; used to watch a specific target keyword move over weeks, not check it once. **Keywords Explorer** — search volume, difficulty, related-term research for planning new content, used when scoping content rather than for daily monitoring.

## Reading the Site Health Score

Industry benchmark: 90+ is strong, below 70 typically signals structural issues suppressing rankings. InspectOS's last pulled score (66/100) sits below that threshold. HomeOS (85/100) is closer to healthy but not yet strong.

## Workflow

Site Explorer first for the current authority/traffic snapshot → Site Audit to check what's technically broken underneath it → Rank Tracker to monitor movement on priority keywords after a change → Keywords Explorer only when scoping new content.

## Data discipline

Ahrefs numbers move — a score pulled today is stale within a month. Re-pull before using any figure to justify a recommendation.

InspectOS project ID `9596383`, HomeOS project ID `10072010`, both owned by `hello@inspectos.pt`, access type "shared."

See [[ops-role-hub]].
