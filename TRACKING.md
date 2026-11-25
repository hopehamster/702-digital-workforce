# Tracking — where the work lives

This repository (`702-digital-workforce`) is the **public face** of the 702 Digital Workforce program: vision, catalogue, and blueprint.

**Day-to-day program tracking lives in the main 702 AI Services repository**, alongside the rest of the company's work:

- **Program board:** [702 Digital Workforce — Program Board](https://github.com/users/hopehamster/projects/16) — every program issue on one board
- **Program epic:** [#140 — PROGRAM EPIC: 702 Digital Workforce](https://github.com/hopehamster/702aiservices/issues/140)
- **All workforce issues:** [search `wf:` labels](https://github.com/hopehamster/702aiservices/issues?q=is%3Aissue+label%3Awf%3Aphase-0%2Cwf%3Aphase-1%2Cwf%3Aphase-2%2Cwf%3Aphase-3%2Cwf%3Aphase-4)
- **Milestones:** the "Workforce Phase 0–4" milestones on the [milestones page](https://github.com/hopehamster/702aiservices/milestones)
- **Labels:** everything for this program is namespaced with the `wf:` prefix in that repo — `wf:type-*` (epic / spec / build / research / decision), `wf:phase-0` … `wf:phase-4`, `wf:priority-*` (now / next / later), and `wf:area-*` (platform / employee / factory / billing / customer).

## Epics

| Epic | Issue | Phase |
|---|---|---|
| Program epic | [#140](https://github.com/hopehamster/702aiservices/issues/140) | — |
| Master Architecture Specification | [#141](https://github.com/hopehamster/702aiservices/issues/141) | 0 — Foundations |
| Digital Employee Standard | [#142](https://github.com/hopehamster/702aiservices/issues/142) | 0 — Foundations |
| Digital Workforce Factory Specification | [#143](https://github.com/hopehamster/702aiservices/issues/143) | 0 — Foundations |
| Engineering Implementation Plan | [#144](https://github.com/hopehamster/702aiservices/issues/144) | 0 — Foundations |
| Prototype hardening — Employee Standard proven on the prototype | [#145](https://github.com/hopehamster/702aiservices/issues/145) | 1 |
| Billing & customer lifecycle | [#146](https://github.com/hopehamster/702aiservices/issues/146) | 2 |
| Catalogue — 18 roles × 5 grades | [#147](https://github.com/hopehamster/702aiservices/issues/147) | 4 |

First work items (#148–#155) — the Sandbox vs Computer decision, the Unkernel sync model, the credential & security model, the identity schema, the skill-package format, certification gates, cost telemetry, and the Browser Run evaluation — hang under their epics as sub-issues.

## Program structure

- **Phase 0 — Foundations.** The four foundational documents: Master Architecture Specification, Digital Employee Standard, Digital Workforce Factory Specification, Engineering Implementation Plan.
- **Phase 1 — Employee Standard proven on the prototype.** The already-operating prototype employee is hardened against the standard: identity, memory, skills packaging, supervision/QA loop.
- **Phase 2 — Factory v1.** Manufacture one employee end to end from the factory specification.
- **Phase 3 — First external pilot employee.** A leased employee working for a real customer.
- **Phase 4 — Catalogue launch.** The 18-role × 5-grade catalogue, live.

Each phase and each foundational document is tracked as an epic in the main repository, with the concrete decisions and work items as its sub-issues.
