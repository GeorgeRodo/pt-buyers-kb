---
id: decision-authority-guardrails-workspace-access
title: "Decision Authority & Guardrails — Workspace Access & Credentials"
category: "Decision Authority & Guardrails"
domain: "Workspace Access & Credentials Management"
status: "Active"
last_updated: "2026-07-23"
tags: ["access", "credentials", "1password", "guardrails", "gap-flagged"]
summary: "Access grants: Paul/Filipe, unilateral. Billing/seat changes: Petra approves, Filipe executes. No written hygiene policy yet."
---

# Decision Authority & Guardrails — Workspace Access & Credentials

## Unilateral authority
- Paul or Filipe can each independently grant limited, task-scoped credential access to an intern or temporary team member — no sign-off needed between them for standard, limited-scope grants.

## Billing / seat escalation path
- Any billing action on the 1Password plan (e.g. adding a 6th seat) is **requested through Petra** (Financial Manager) and **executed by Filipe**. This is a two-step approval, not a unilateral grant.

## Guardrails
- Interns/non-seat team members get **strictly** the credential(s) their task requires — never the full shared vault, never a named seat.
- The 5-seat cap is a hard ceiling: a new named member requires going through the Petra → Filipe billing path, not a routine grant.

## ⚠️ Gap flagged — no hard rule currently in place

As of this writing, there is **no written policy** covering:
- Mandatory 2FA on the 1Password account itself
- A defined offboarding SLA (how quickly an intern's limited access gets revoked after their engagement ends)
- A shared, append-only log of who granted what access to whom and when

Right now this relies on Paul and Filipe remembering to revoke access manually. Worth deciding on a minimal written rule (even just "revoke intern access within 48 hours of engagement end, logged in [wherever]") before this scales past the current team size.
