---
id: operations-status-seo
title: "How SEO Works, How It's Executed, and Current Status"
category: "Operations & Status"
domain: "SEO"
status: "Active"
last_updated: "2026-07-23"
tags: ["seo", "process", "current-status", "ahrefs", "dr"]
summary: "SEO methodology, execution pipeline, and live current status for InspectOS and HomeOS as of 2026-07-23."
data_source: "Ahrefs API, pulled live 2026-07-23"
---

# How SEO Works, How It's Executed, and Current Status

## How SEO works here

Two live properties, two different SEO logics:

- **InspectOS (inspectos.pt)** — a physical inspection service targeting foreign property buyers in Portugal, many of whom don't yet know inspection is something they need to do. SEO here is an *education/awareness* problem as much as a visibility one. A backlink or content source is valuable if it puts InspectOS in front of that uninformed foreign audience — not just because it has strong PT-specific traffic.
- **HomeOS (homeos.pt)** — a digital property-intelligence platform. No physical service, so SEO content routes to free tools and a report waitlist rather than a booking.

Both sites sit on the same underlying SEO mechanics: technical health (crawlability, no broken links), on-page relevance (content matching real search intent), and off-site authority (backlinks from relevant, legitimate domains) — but the audience-fit judgment differs per brand.

## How it's executed

1. This position sets strategy and direction (see `responsibilities/seo.md`) — a function of the role, not a specific individual.
2. Before any recommendation, current Ahrefs data is pulled and verified — not worked from memory of a prior check-in.
3. Specs, briefs, and audits are produced and handed to the SEO team for execution.
4. Work comes back and gets evaluated against the original brief and current data.
5. Phase discipline applies: foundation-stage gaps (technical cleanup, thin backlink base) get closed before scaling-stage tactics (backlink acquisition, PR) are recommended, unless explicitly parallelized.

Both properties already have live, verified Ahrefs projects set up (InspectOS: project ID `9596383`; HomeOS: project ID `10072010`), both owned by `hello@inspectos.pt`, access type "shared" — meaning tracking infrastructure is already in place; the gap is in the underlying SEO fundamentals (see below).

## Current status (live data, pulled 2026-07-23)

### InspectOS (inspectos.pt)

| Metric | Value |
|---|---|
| Domain Rating (DR) | **6.0** (Ahrefs Rank ~25.6M) |
| Live backlinks | 131 (148 all-time) |
| Live referring domains | 11 (12 all-time) |
| Organic keywords ranked (top 100) | 11 |
| Est. monthly organic traffic | 48 visitors |
| Est. monthly organic traffic value | $0.61 |
| Site Health Score | 66 / 100 |
| Crawled URLs / errors / warnings / notices | 553 / 190 / 392 / 279 |
| Last crawl | 2026-07-20 |

**Top referring domains:** provenexpert.com (DR 91), expat.com (DR 72), erasmusintern.org (DR 66), askmap.net (DR 74) — all niche-relevant to foreign buyers/expats, good audience fit regardless of raw PT traffic. Also linked from `realestate-lisbon.com` and `fairbank.pt` (Skaler), and cross-linked from `homeos.pt`.

**Top ranking keywords:** "home inspection" (vol 1,700/mo, position 12, 30 est. visits/mo), "home inspection services" (vol 150, position 6), "property inspection" (vol 100, position 9). Notably, **"adene"** (vol 1,600/mo — the Portuguese energy-certificate authority, directly relevant to InspectOS's ADENE certificate service) ranks at **position 19** — page 2, zero traffic yet. This is a live optimization target, not a gap that needs new content.

**Top pages:** `/en/home-inspections` carries effectively all current traffic (48/48, 9 keywords). The Portuguese-language equivalents (`/inspecoes-residenciais`, `/adene-certificado-energetico`) each rank for exactly one keyword and drive zero traffic — the EN page is doing all the work right now.

### HomeOS (homeos.pt)

| Metric | Value |
|---|---|
| Domain Rating (DR) | **2.8** (Ahrefs Rank ~38.7M) |
| Live backlinks | 1,205 (**13,374 all-time**) |
| Live referring domains | 474 (**771 all-time**) |
| Organic keywords ranked (top 100) | **0** |
| Est. monthly organic traffic | **0** |
| Site Health Score | 85 / 100 |
| Crawled URLs / errors / warnings / notices | 275 / 41 / 191 / 101 |
| Last crawl | 2026-07-23 (today) |

**Top referring domains:** blogspot.com (DR 95), yahoo.com (DR 94), blogger.com (DR 94), sapo.pt (DR 87), iol.pt (DR 79) — high raw DR, but one flagged domain: **`za.com` (DR 90) is marked `is_spam: true`** in Ahrefs' own data. Worth a manual disavow review rather than treating it as a quality signal just because of its DR.

## Flags worth this position's attention

- **HomeOS: large backlinks/referring-domains base, zero rankings.** 474 live referring domains and literally 0 ranked keywords is an unusual combination — the authority signal exists but isn't translating into visibility yet. Consistent with HomeOS being in an earlier content/keyword-research phase (formal keyword research for the next content phase was still pending as of the last status check) — this isn't a backlink problem, it's a content/targeting gap.
- **HomeOS: 88% of all-time backlinks are no longer live** (13,374 → 1,205). Worth understanding why before treating the historical number as representative of current authority.
- **InspectOS: 190 of 553 crawled URLs have errors** (Site Health 66/100) — meaningful technical debt sitting underneath any content or backlink work.
- **InspectOS: "adene" keyword** is a concrete, low-effort opportunity — high volume, already ranking (page 2), directly tied to an existing service page.
