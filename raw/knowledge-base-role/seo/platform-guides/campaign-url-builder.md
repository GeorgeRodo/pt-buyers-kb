---
id: platform-guide-campaign-url-builder
title: "Platform Guide — Campaign URL Builder (UTM Links)"
category: "Platform Guides"
domain: "SEO"
status: "Active"
last_updated: "2026-07-23"
tags: ["seo", "utm", "campaign-tracking", "platform-guide"]
summary: "How UTM links are built for InspectOS/HomeOS campaigns, including the exact parameter rules already in use."
---

# Platform Guide — Campaign URL Builder (UTM Links)

## What it does

Google's Campaign URL Builder (ga-dev-tools.google/campaign-url-builder) appends tracking parameters to a URL so GA4 can attribute traffic to the exact campaign/channel that sent it, rather than lumping it into generic "referral" or "direct" traffic. Five parameters exist (source, medium, campaign, term, content); this stack uses three of them by default.

**UTM parameters are case-sensitive in GA4** — `utm_source=Facebook` and `utm_source=facebook` are tracked as two different sources. Always lowercase.

## The exact process already in use here

There's a dedicated internal tool for this (`utm-builder` skill) — use it rather than the public web tool when generating links for InspectOS social posts, since it already encodes the rules below:

**Format:**
```
{base_url}?utm_source={platform}&utm_medium=social&utm_campaign={campaign_slug}
```

**Parameter rules:**

| Parameter | Rule |
|---|---|
| `utm_source` | Always lowercase: `instagram`, `facebook`, `linkedin`, `tiktok`, `twitter`, `google` |
| `utm_medium` | Always `social` |
| `utm_campaign` | Lowercase, spaces replaced with `+` (e.g. `apartment+inspection`) |
| `utm_content` | Only for special cases (FAQ posts, GBA posts) — not added by default |

**Campaign slug convention:** short, descriptive, lowercase, spaces → `+`, drop filler words (the/a/an/in/for). Established slugs already in use: `bio`, `mold`, `structural`, `snagging`, `apartment+inspection`, `property+inspection+porto`, `epbd+compliance+2026`.

**Hard rule: never generate or append short links.** Short links are created separately by whoever is posting, after the UTM URL is built — this tool's job stops at the full tagged URL.

## Where this connects

Every UTM-tagged link that gets clicked shows up in GA4's Acquisition reports under the matching source/medium/campaign — that's the verification loop: build the link here, confirm the traffic lands correctly in GA4.

Sources:
- [URL builders: Collect campaign data with custom URLs — Google Analytics Help](https://support.google.com/analytics/answer/10917952?hl=en)
- [A Guide to UTM Parameters in Google Analytics 4](https://www.analyticsmania.com/post/utm-parameters-in-google-analytics-4/)
