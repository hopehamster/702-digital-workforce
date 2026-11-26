# 702 Digital Workforce

**702 AI Services is becoming a digital staffing platform.** We hire, place, bill for, and supervise AI *digital employees* that businesses lease the way they would lease staff from a staffing agency — except the employee is software: a persistent professional identity with skills, memory, and a workspace, matched to a role and a grade.

This repository is the **public home of the program**: the vision, the employee catalogue, and the research blueprint behind it. Day-to-day program tracking (epics, issues, milestones) lives in the main 702 AI Services repository — see [TRACKING.md](TRACKING.md).

## The idea in one paragraph

A digital employee doesn't need a computer running all the time. It needs a **persistent identity with access to computing resources on demand**. The employee keeps its professional skills, memory, personality, documents, permissions, and assignments; compute is provisioned only when there is work to do. So instead of hand-crafting one-off bots, we are building a **factory that manufactures digital employees** — configured, certified, and deployed to a standard.

## Two places to work

- **The workstation — a dedicated cloud server.** Each employee runs on its own dedicated server, hosted and operated by 702 AI Services: one worker, one machine, isolated per customer. (The program also works with local-compute technology such as [Unkernel](https://github.com/unkernel), a Linux kernel that runs in the browser; running on customer hardware is not part of the current offer.)
- **The office — Cloudflare Computer.** A persistent workspace (memory, files, skills, documents) the employee returns to between shifts, so work and context survive between assignments.

## The model

- Businesses browse employees by **role** and **grade**, subscribe monthly, and the employee starts work — supervised by 702 AI Services, with performance reviews and replacement if an employee underperforms.
- Pricing is a **flat monthly grade price** — no revenue split in either direction. 702 AI Services hosts and runs the worker on its own infrastructure; the customer provides no hardware and bears no hosting burden.

## Catalogue at a glance

18 professional roles across administration, finance, sales & marketing, technical, and project/operations work — each offered at five grades from **Entry Level ($599/mo)** to **Expert ($10,000/mo)**. Full catalogue: [docs/VISION.md](docs/VISION.md).

## Product tiers

Digital Employee → Digital Team → Digital Department → Digital Office → Personal AI Computer.

## Documents

- [docs/VISION.md](docs/VISION.md) — the concept, the model, the full roles × grades catalogue, and the tiers.
- [docs/BLUEPRINT-SUMMARY.md](docs/BLUEPRINT-SUMMARY.md) — the research blueprint: recommended architecture, cost model, and the findings the program is built on.
- [TRACKING.md](TRACKING.md) — where the work is tracked and how to follow along.

## Status

In active development. A prototype digital employee built on this exact architecture is already in daily operation inside 702 AI Services, and the program is working through its foundation phase: the architecture specification, the employee standard, the factory specification, and the implementation plan.
