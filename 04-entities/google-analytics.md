---
title: Google Analytics (GA4)
type: entity
tags: [agency, inspection]
status: draft
created: 2026-07-23
updated: 2026-07-23
sources: [src-role-knowledge-base]
brand: shared
verified: false
---

# Google Analytics (GA4)

Tracks actual visitor behavior on inspectos.pt and homeos.pt (pageviews, clicks, scrolls, conversions modeled as events) — answers what [[ahrefs]] can't: Ahrefs estimates organic search performance from external data, GA4 reports what real visitors did once they landed.

## Setup checklist (verify, don't assume)

Property + web data stream exist and are actively collecting for each domain. Enhanced Measurement is on (auto-tracks scrolls, outbound clicks, downloads). Key events (GA4's term for conversions) are marked for what matters — inspection booking/inquiry for InspectOS, tool usage/report-waitlist signup for HomeOS. Data retention changed from the 2-month default to 14 months (Admin → Data Settings), or historical Explore-report analysis silently breaks. Time zone confirmed as Portugal, not GA4's US-Pacific default, or reporting dates are off. Installed via [[google-tag-manager|GTM]] rather than hardcoded gtag, to keep tracking centralized and auditable.

## Day-to-day use

Realtime report to confirm tracking is live after a site change. Acquisition reports cross-checked against [[campaign-url-builder|UTM-tagged links]] to confirm campaign attribution. Engagement reports (which pages hold attention vs. bounce) read alongside Ahrefs' top-pages data to see whether a ranking page actually converts. Explore for custom breakdowns not in standard reports (e.g. foreign-buyer segment behavior by country). DebugView to verify a new event/tag fires correctly before trusting it in reports.

Same discipline as Ahrefs: pull current numbers before claiming what's working.

See [[ops-role-hub]].
