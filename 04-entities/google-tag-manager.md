---
title: Google Tag Manager (GTM)
type: entity
tags: [agency, inspection]
status: draft
created: 2026-07-23
updated: 2026-07-23
sources: [src-role-knowledge-base]
brand: shared
verified: false
---

# Google Tag Manager (GTM)

Delivery mechanism for tracking code on inspectos.pt and homeos.pt — tags are configured in GTM's interface and pushed live through one container snippet, instead of editing site code every time a new tracking pixel or event is needed. [[google-analytics|GA4]] is delivered through GTM rather than hardcoded, so all tracking lives in one auditable place.

## Three core concepts

**Tags** — the action: a snippet sending data somewhere (GA4, a Facebook Pixel, a conversion tracker). **Triggers** — the "when": the condition that fires the tag (page load, a click, a form submission, a custom event); every tag needs at least one. **Variables** — the "what information": reusable values (page URL, click text, form ID) that tags and triggers pull from.

## Before publishing

Always use Preview mode first — it connects GTM to the live site in a debug session showing exactly which tags fired, on what trigger, with what variable values. Never hit Submit on a new or edited tag without confirming it in Preview; a bad tag going live sitewide is the tracking equivalent of shipping a broken page. If a conversion event looks wrong in GA4, check here first — a tag/trigger may be misconfigured or a container version pushed untested.

See [[ops-role-hub]].
