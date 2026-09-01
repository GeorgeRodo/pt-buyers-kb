---
title: Campaign URL Builder (UTM Links)
type: entity
tags: [agency, inspection]
status: draft
created: 2026-07-23
updated: 2026-07-23
sources: [src-role-knowledge-base]
brand: shared
verified: false
---

# Campaign URL Builder (UTM links)

Google's Campaign URL Builder appends tracking parameters to a URL so [[google-analytics|GA4]] can attribute traffic to the exact campaign/channel that sent it, instead of lumping it into generic "referral" or "direct." Five parameters exist (source, medium, campaign, term, content); this stack uses three by default. **UTM parameters are case-sensitive in GA4** — `utm_source=Facebook` and `utm_source=facebook` track as two different sources; always lowercase.

## Process already in use

A dedicated internal `utm-builder` skill is used instead of the public web tool for InspectOS social posts, since it already encodes these rules:

**Format:** `{base_url}?utm_source={platform}&utm_medium=social&utm_campaign={campaign_slug}`

| Parameter | Rule |
|---|---|
| `utm_source` | Always lowercase: `instagram`, `facebook`, `linkedin`, `tiktok`, `twitter`, `google` |
| `utm_medium` | Always `social` |
| `utm_campaign` | Lowercase, spaces → `+` (e.g. `apartment+inspection`) |
| `utm_content` | Only for special cases (FAQ posts, GBA posts) — not added by default |

Campaign slug convention: short, descriptive, lowercase, spaces → `+`, drop filler words (the/a/an/in/for). Established slugs: `bio`, `mold`, `structural`, `snagging`, `apartment+inspection`, `property+inspection+porto`, `epbd+compliance+2026`.

**Hard rule: never generate or append short links** — those are created separately by whoever posts, after the UTM URL is built; this tool's job stops at the full tagged URL.

Relevant to Exgest social-thread output (see [[social-media-playbook]]) — any Exgest-generated post that includes a link back to the wiki-derived content should use this convention. Every tagged link that gets clicked shows up in GA4's Acquisition reports under the matching source/medium/campaign — build here, confirm the traffic lands correctly in GA4.

See [[ops-role-hub]].
