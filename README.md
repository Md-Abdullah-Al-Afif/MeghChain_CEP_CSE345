# MeghChain: Smart Cold-Chain Health Logistics Network

A Complex Engineering Project in Software Engineering and Information System Design, designed and authored by Md. Abdullah Al Afif.

Academic coursework project, CSE 345: Information System Design & Software Engineering, Summer 2026.

---

## About This Repository

This repository showcases my work on a Complex Engineering Project (CEP), which I completed as coursework for CSE 345. It is an academic project, and I am its sole author. The analysis, method selection, requirements, prioritisation framework, UML designs, schedule, testing strategy and cost estimate are all my own work.

The aim is to document how I approached a deliberately open-ended problem: not just what I designed, but why, with every decision traced back to a specific detail of the scenario.

## The Problem

The Sylhet–Meghalaya hill corridor of Bangladesh serves about 240 rural clinics, 9 district hospitals and 3 border quarantine posts across 5 districts. Vaccines, blood products and temperature-sensitive medicines are tracked with paper logs, radio call-ins and informal couriers. After the March 2026 floods, at least 40,000 vaccine doses were lost to undetected cold-chain breaks.

MeghChain is a fictional inter-agency initiative (USD 65 million in funding, with USD 6.2 million and 12 months for Phase 1) to digitise cold-chain visibility. The challenge spans engineering, public health policy, human behaviour and cross-border regulation.

My report uses two real failures from the scenario as its tests of success:

1. Would this design have caught the March 2026 spoilage?
2. Would health workers actually use it, unlike the abandoned smart-thermometer pilot?

## What I Did

**Task 1: Problem analysis and development method.** I identified the operational, technical, organisational and human factors that make the problem ill-structured. I proposed Staged Delivery with an Early Risk Phase and justified it against rejected Waterfall and pure Scrum, with Spiral also considered.

**Task 2: Requirements, priorities and schedule.** I wrote 18 functional, 13 non-functional and 9 constraint-driven requirements. I designed my own MeghChain Priority Score with two override rules, analysed four stakeholder conflicts and their costs, and built a 12-month Excel Gantt chart.

**Task 3: UML system design.** I produced use case, class, sequence and activity diagrams, plus a batch life-cycle table and a four-layer architecture. I applied the Adapter and Observer design patterns.

**Task 4: Testing and estimation.** I designed risk-based testing for each software category, estimated size with Function Point Analysis and effort with COCOMO II, and produced a cost plan with risks and an effort range.

## Highlights

**Method.** A three-month risk-reduction stage (Stage 0), then three delivery stages, each closed by a funder audit checkpoint, with two-week iterations inside each stage. Work that depends on outside authorities, such as NBR customs, sits on a separate track so it cannot block the schedule.

**Prioritisation framework.** The MeghChain Priority Score weighs five questions: Safety (0.30), Audit (0.20), Trust (0.20), Build order (0.15) and Disaster value (0.15). Score bands map directly to delivery stages. Rule A keeps legal items on time, and Rule B stops surveillance-like features from shipping without privacy safeguards.

**Safety built into the design.**
- Detection and blocking of unsafe stock happen fully on the phone, with no network needed.
- Safety records are never overwritten during sync.
- A flagged batch with no officer review within 72 hours moves to Unsafe automatically.

**Honest estimation.** The full brief scope (about 168 person-months, about 18.4 months nominal) does not fit in 12 months. Phase 1 is scoped to a core of about 87 person-months, with a cost plan of about USD 6.13 million including a 15 percent contingency, under the USD 6.2 million limit.

## How Constraints Shaped the Design

| Scenario constraint | Design response |
|---|---|
| Patchy or no coverage at 8 clinics | Offline-first field app with a 14-day offline requirement |
| 2011 EPI system cannot be retired in Phase 1 | Adapter-based one-way nightly feed; legacy system never the source of truth |
| NBR customs runs a disconnected platform | Offline border delivery paper; live link kept off the critical path |
| Distributors refuse to share stock and routes | Only aggregate capacity ranges are shared |
| Surveillance fears from the failed pilot | Role- and clinic-level records, clinic-level location, visible data-use screen |
| Stricter blood-product rules | Separate blood workflow with consent and chain-of-custody track |
| Funding released against audits | Four checkpoints; audit evidence produced by the system itself |

## Using This Work

I am happy for this repository to help others learn.

- Read it, learn from the reasoning, and use it as a reference for how to justify decisions against a scenario.
- Credit the author if you cite, quote or build on it: Md. Abdullah Al Afif, "MeghChain: Smart Cold-Chain Health Logistics Network", academic CEP, 2026.
- Do not submit this work, or a lightly edited version, as your own academic assignment.

You may share and adapt the report text and diagrams as long as you give appropriate credit to the author.

## Author

Md. Abdullah Al Afif, Dhaka, Bangladesh
