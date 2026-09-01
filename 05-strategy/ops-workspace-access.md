---
title: Workspace Access & Credentials Management
type: concept
tags: [agency, inspection]
status: draft
created: 2026-07-23
updated: 2026-07-23
sources: [src-role-knowledge-base]
brand: shared
verified: false
---

# Workspace access & credentials management

Administration of the 1Password Families account (`hello@inspectos.pt`) that holds InspectOS and HomeOS credentials — the master credential store for both brands.

## Seat structure

Families plan, 5 seats, all currently filled:

| # | Seat holder | Role |
|---|---|---|
| 1 | Paul | Manager |
| 2 | Filipe | Manager |
| 3 | Petra | Financial Manager |
| 4 | Juan | HR |
| 5 | `hello@inspectos.pt` | Shared admin account (not personal) |

A shared vault holds social media and other logins for InspectOS and HomeOS, tagged and organized so any seat-holder can find what they need. No seat headroom remains — adding a new named member requires the billing escalation path below.

## Access-granting authority

Paul and Filipe each independently hold authority to grant limited, task-scoped credential access to interns or temporary team members — not a strict single point of approval, and no sign-off needed between them for standard, limited-scope grants. Interns and non-seat team members never get a full vault or a named seat — strictly the specific credential(s) their task requires, decided case by case.

## Billing / seat escalation

Any billing action on the plan (e.g. adding a 6th seat) is requested through **Petra** (Financial Manager) and executed by **Filipe** — a two-step approval, not a unilateral grant. See [[ops-tools-billing]] for the broader billing-ownership pattern (Paul/Filipe own it; Petra is the financial approval layer specifically for this plan).

## Gap flagged — no written hygiene policy

As of 2026-07-23, there is no written policy covering: mandatory 2FA on the 1Password account itself, a defined offboarding SLA (how quickly an intern's access gets revoked after engagement ends), or a shared, append-only log of who granted what access to whom and when. This currently relies on Paul and Filipe remembering to revoke access manually. Worth a minimal written rule (e.g. "revoke intern access within 48 hours of engagement end, logged in [wherever]") before this scales past the current team size.

Parent: [[ops-role-hub]].
