---
id: platform-guide-google-analytics
title: "Platform Guide — Google Analytics (GA4)"
category: "Platform Guides"
domain: "SEO"
status: "Active"
last_updated: "2026-07-23"
tags: ["seo", "analytics", "ga4", "platform-guide"]
summary: "How to work with GA4: setup checklist, common misconfigurations, and how it complements Ahrefs data."
---

# Platform Guide — Google Analytics (GA4)

## What it is, and why it's in this stack

GA4 tracks actual visitor behavior on inspectos.pt and homeos.pt (pageviews, clicks, scrolls, conversions — modeled as events). It answers a different question than Ahrefs: Ahrefs estimates organic search performance from external data; GA4 reports what real visitors did once they landed on the site. Both are needed — Ahrefs for "are we visible," GA4 for "what happens once someone arrives."

## Setup checklist (verify these are correct, don't assume)

- **Property + web data stream** exist for each domain and are actively collecting data.
- **Enhanced Measurement** is switched on (auto-tracks scrolls, outbound clicks, file downloads without extra tagging).
- **Key events** (GA4's term for conversions) are marked for the actions that matter — e.g. inspection booking/inquiry for InspectOS, tool usage/report waitlist signup for HomeOS.
- **Data retention** — GA4 defaults to 2 months, which silently breaks historical analysis in Explore reports. Change this to 14 months (Admin → Data Settings → Data Retention).
- **Time zone** — GA4 defaults to US Pacific Time. Confirm it's set to the correct time zone for Portugal, or reporting dates will be off.
- **Installation method** — GA4 can be installed via a plugin, native gtag code, or Google Tag Manager. Since GTM is already part of this stack, route GA4 through GTM rather than hardcoding gtag — it keeps tag management centralized and auditable (see the Google Tag Manager platform guide).

## How to actually use it day to day

- **Realtime report** — confirm tracking is live after any site change.
- **Acquisition reports** — which channel/source traffic is coming from; cross-check against UTM-tagged campaign links (see Campaign URL Builder guide) to confirm campaign attribution is working.
- **Engagement reports** — which pages hold attention vs. bounce immediately; useful alongside Ahrefs' top-pages data to see whether a page that ranks is actually converting visitors once they land.
- **Explore** — for any custom breakdown not covered by standard reports (e.g. foreign-buyer segment behavior by country).
- **DebugView** — use this to verify a new event or tag is firing correctly before trusting it in reports.

## Where this fits in the role

Reading GA4 data falls under the same discipline as Ahrefs: pull current numbers before making a claim about what's working, don't work from a stale mental model of the site's traffic.

Sources:
- [Google Analytics 4 (GA4) Guide for Marketers 2026](https://www.mediasearchgroup.com/blog/mastering-google-analytics-4-a-step-by-step-guide-for-marketers/)
- [How to Install Google Analytics 4 in 2026 (3 Ways)](https://www.analyticsmania.com/post/how-to-install-google-analytics-4-with-google-tag-manager/)
- [GA4 Setup Guide Step by Step (2026)](https://www.nextalgoo.us/topic/ga4-setup-guide-step-by-step-with-code-examples)
