---
title: "Registo Predial — Land Registry"
type: entity
tags: [phase-4, phase-7, agency, cpcv]
status: draft
created: 2026-07-14
updated: 2026-07-14
sources: [src-buyers-agent-playbook-2026]
brand: shared
verified: false
---

# Registo Predial — land registry

The *Conservatória do Registo Predial* is Portugal's land registry: the authority of record for title, encumbrances, and ownership chain. Promoted from a one-liner in [[entities-hub]] on 2026-07-14 — cited across [[phase-4-due-diligence|Phase 4]], [[phase-7-closing|Phase 7]], and [[cpcv]] with no dedicated page.

## What it issues

- **Certidão predial permanente** (perpetual registry certificate) — title, description, encumbrances, liens, mortgages, and *usucapião* (adverse possession) actions. Must be issued within 30 days of CPCV signing to be considered current.
- **Certidão matricial** (for older properties) — historic ownership chain; gaps here (transfers that were never registered) are a title red flag in their own right.

This is distinct from the **caderneta predial**, which is the *fiscal* description (ownership, area, tax value) issued by the Autoridade Tributária, not the Registo Predial — the two documents are cross-checked against each other precisely because they can diverge.

## DD role ([[phase-4-due-diligence|Phase 4]])

The certidão predial is the primary tool for detecting: unregistered inheritance or prior transfers (title gap), pending litigation actions registered against the property, liens and unresolved mortgages, and reservations that could block a clean sale. A seller who cannot produce a clean certidão predial within 7 days of CPCV is treated as a walk-away signal — unresolved title, inheritance, or encumbrance is the near-universal cause.

## Area discrepancy check

The certidão predial's stated area is cross-checked against the caderneta predial and the property's actual measured area. This is the source of the wiki's one unresolved numeric conflict:

> [!warning] `phase-4-due-diligence.md`'s desktop-audit step flags a discrepancy at **>2%**; the playbook's own Phase 4/CPCV-stage red flag (Appendix C.4, §5.1.1) uses **>5%** for what appears to be the same "unlicensed alteration" check. See [[cpcv]] for the fuller reconciliation note — unresolved as of 2026-07-14, pending Paul's call on which threshold governs where.

## Post-deed role ([[phase-7-closing|Phase 7]])

Registration of the buyer's ownership at the Registo Predial happens 1–10 days after the deed, coordinated by the buyer's lawyer/notary — this is the final step that makes the transaction legally complete, distinct from and after the *escritura* itself. Registry fees (€200–600) are payable after deed.

Up: [[entities-hub]] · Feeds: [[phase-4-due-diligence]], [[phase-7-closing]], [[cpcv]]
