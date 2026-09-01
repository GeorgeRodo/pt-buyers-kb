---
title: SEO Ownership — Strategy, Status, and KPIs
type: concept
tags: [agency, inspection]
status: draft
created: 2026-07-23
updated: 2026-07-23
sources: [src-role-knowledge-base]
brand: shared
verified: false
---

# SEO ownership — strategy, status, and KPIs

This role sets SEO strategy and direction for both **InspectOS** and **HomeOS** and evaluates the SEO team's output; it doesn't execute tactically. Before any recommendation, current [[ahrefs]] (and [[google-analytics]]) data gets pulled and verified — never worked from memory of a prior check-in, since the numbers below are point-in-time and go stale within weeks.

## Two properties, two SEO logics

**InspectOS** (inspectos.pt) is a physical inspection service targeting foreign buyers who often don't yet know inspection is something they need — SEO here is an education/awareness problem, not just visibility. A backlink or content source is valuable if it puts InspectOS in front of that uninformed foreign audience, even without strong PT-specific traffic. **HomeOS** (homeos.pt) is a digital property-intelligence platform with no physical service; SEO content routes to free tools and a report waitlist rather than a booking. Both sit on the same underlying mechanics — technical health, on-page relevance, off-site authority — but the audience-fit judgment differs per brand.

## Responsibilities and delegation

Core duties: evaluate the SEO team's strategy and output before it ships; pull and verify current Ahrefs data before proposing or approving any action; verify the live site before treating a URL or content gap as missing (plans get built ahead of ship dates); track foundation-stage vs. scaling-stage vs. compounding-stage work and sequence accordingly; surface technical debt proactively even when not asked; produce specs/briefs/audits for the SEO team; judge whether a backlink/content prospect fits the actual goal (domestic PT visibility vs. foreign-buyer awareness vs. direct referral) rather than applying a generic traffic filter.

Tactical execution — outreach emails, link building, end-to-end keyword-research spreadsheets — belongs to the SEO team unless explicitly requested as a one-off.

**Execute directly:** pull/verify Ahrefs+GSC data; write specs/briefs/audits; evaluate team output; flag technical debt and spam-tactic risk.
**Delegate:** backlink outreach execution; on-page/technical implementation; day-to-day keyword tracking and reporting.
**Escalate:** which audience to prioritize when unclear; phase sequencing/parallelization calls; whether a tactic fits current team capacity — these get asked directly rather than guessed, since a wrong assumption here wastes real outreach effort.

## Hard guardrails

No PBNs, bulk paid-link packages, link farms, or any manipulative-reading tactic — even if a competitor is visibly outranking with them; flag it instead of matching it. No treating suspicious prospects (identical domain clusters, zero real traffic, throwaway names) as legitimate outreach targets. No filtering prospects by PT-only organic traffic when the actual goal is foreign-buyer awareness. No recommending later-phase tactics (large-scale digital PR, sustained journalist relationships) before earlier-phase gaps (broken links, thin backlink base, unfinished technical cleanup) are closed, unless explicitly parallelized.

## Access

Full query access to [[ahrefs]] (Site Explorer, Site Audit, Rank Tracker, Keywords Explorer) across two live projects — InspectOS (project ID `9596383`) and HomeOS (project ID `10072010`), both owned by `hello@inspectos.pt`, access type "shared." Also: Google Search Console, direct access to both live sites for crawl/QA checks, [[google-analytics|GA4]], [[google-tag-manager|GTM]], and the [[campaign-url-builder]].

## Current status (Ahrefs, pulled live 2026-07-23)

> [!warning] Point-in-time figures. Re-pull before using any of this to justify a new decision.

| Metric | InspectOS | HomeOS |
|---|---|---|
| Domain Rating | 6.0 | 2.8 |
| Live backlinks (all-time) | 131 (148) | 1,205 (13,374) |
| Live referring domains (all-time) | 11 (12) | 474 (771) |
| Organic keywords ranked (top 100) | 11 | 0 |
| Est. monthly organic traffic | 48 | 0 |
| Est. monthly organic traffic value | $0.61 | $0 |
| Site Health Score | 66/100 | 85/100 |
| Crawled URLs / errors | 553 / 190 | 275 / 41 |
| Last crawl | 2026-07-20 | 2026-07-23 |

**InspectOS:** top referring domains are niche-relevant to foreign buyers/expats regardless of raw PT traffic — provenexpert.com (DR 91), expat.com (DR 72), erasmusintern.org (DR 66), askmap.net (DR 74) — plus `realestate-lisbon.com`, `fairbank.pt` (Skaler), and cross-links from homeos.pt. Top keyword: "home inspection" (vol 1,700/mo, position 12). Concrete opportunity: **"adene"** (vol 1,600/mo) ranks position 19 (page 2, zero traffic) — a live optimization target, not a content gap, directly tied to the ADENE certificate service page. `/en/home-inspections` carries effectively 100% of current traffic (48/48, 9 keywords); the Portuguese-language equivalents each rank for exactly one keyword and drive zero traffic.

**HomeOS:** top referring domains are high-DR but include one Ahrefs-flagged spam domain — `za.com` (DR 90, `is_spam: true`) — worth a manual disavow review rather than treating its DR as a quality signal. The core anomaly: 474 live referring domains and 0 ranked keywords is an unusual combination; the authority signal exists but isn't translating into visibility, consistent with HomeOS still being pre-content/keyword-research phase rather than having a backlink problem. Also flagged: 88% of all-time backlinks (13,374 → 1,205) are no longer live — worth understanding why before treating the historical number as representative.

## KPI set

Authority/backlink: DR, live referring domains, live-vs-all-time retention ratio (HomeOS retains 61%, InspectOS ~92% — a large gap signals link churn), backlink count, spam-flagged referring domains (target 0). Visibility: keywords ranked top 100 / top 3 / top 10, average position on priority terms. Traffic: est. monthly organic traffic and its estimated value. Technical: Site Health Score (industry benchmark 90+ strong, below 70 signals structural issues — InspectOS's 66 sits below that line), URL error count, crawl freshness. Content: traffic concentration (InspectOS ~100% on one page — a single-page dependency worth watching), keywords per ranking page.

## Open item

HomeOS's 88% backlink die-off (13,374 → 1,205 live) is unexplained in the source — worth investigating before the next SEO strategy call.

Parent: [[ops-role-hub]].
