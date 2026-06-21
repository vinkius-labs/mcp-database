# Edison Experimentation Prover MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/edison-experimentation-prover)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/edison-experimentation-prover-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/edison-experimentation-prover-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [complex-reasoning](../categories/complex-reasoning.md)

A team chose paper filing because 'best practice.' No pilot. No alternatives tested. 8 months later, 14,000 submissions/day — 47 hours behind on retrieval. Emergency migration under pressure. Cost: 3x the estimate, 6 weeks frozen. Edison tested 3,000+ filament materials before carbonized bamboo — he did not pick the 'obvious choice.' This tool forces experimentation: test alternatives with measured criteria, iterate beyond the first solution, build the ecosystem, prove viability under real conditions, and document dead ends.

## Description
AI agents pick the first solution that comes to mind and call it done. They do not test alternatives. They do not iterate. They build the feature but forget the ecosystem. They claim 'it works' without real-world evidence. And they never document the dead ends.

### The Problem

LLMs commit five experimentation failures:

- **Experiment Absent** — 'The best approach is the traditional method.' Based on what? Which alternatives were evaluated? With what criteria? What did each score? Edison tested 3,000+ filament materials — platinum, carbon, bamboo, horsehair, fishing line, cork, celluloid — before finding carbonized bamboo from Kyoto lasted 1,200 hours. 'Best practice says' is not an experiment.
- **Iteration Insufficient** — 'It works, let us ship it.' The first working version is rarely the best. Edison ran 10,000+ experiments on the storage battery. What variations did you test? What improved? Where did returns diminish? 'Good enough' means you stopped experimenting too early.
- **System Incomplete** — 'We built the verification module. Rollout is someone else's problem.' Edison did not just build the light bulb — he built generators, cables, switches, meters, fuses, AND sockets. The bulb without the power grid is a curiosity, not a product. Is your solution deployable? Monitored? Documented? Does a user know how to go from zero to using it?
- **Viability Unproven** — 'The design is operationally sound.' Theoretically. Under what volume? At what cost? With what adoption friction? Edison required every invention to be commercially viable within 6 months. 'Works in our pilot' is not viability evidence.
- **Failure Undocumented** — 'We tried some things and settled on this approach.' Which things? What happened with each? Why did they fail? What did you learn? Edison kept 3,500+ notebooks: 'Experiment #247: carbonized cedar — lasted 38 minutes, crumbled at high temperature.' THAT is documentation.

### How It Works

5 Decision Pivots following Edison's methodology:

1. **experimentConducted** — Alternatives tested with measured criteria and results.
2. **iterationSufficient** — Variations tested beyond first working solution to diminishing returns.
3. **systemComplete** — Ecosystem built: rollout plan, monitoring, documentation, transition, onboarding.
4. **viabilityProven** — Real-world evidence, operating cost, adoption friction, success metrics.
5. **failureDocumented** — Each dead end: approach, measured result, root cause, learning.

### The Verdict Matrix

| First Failing Pivot | Verdict | Meaning |
|---|---|---|
| experimentConducted = false | EXPERIMENT_ABSENT | First idea accepted without testing. |
| iterationSufficient = false | ITERATION_INSUFFICIENT | Stopped at first working solution. |
| systemComplete = false | SYSTEM_INCOMPLETE | Built the bulb, forgot the grid. |
| viabilityProven = false | VIABILITY_UNPROVEN | "Should work" — no real evidence. |
| failureDocumented = false | FAILURE_UNDOCUMENTED | "We tried some things" — no record. |
| All pivots pass | EXPERIMENT_PROVEN | Tested. Iterated. Complete. Viable. Documented. |


## Available Tools
- **validate_edison_experimentation**: Think like Edison — who did not invent through genius but through SYSTEMATIC EXPERIMENTATION at industrial scale. Menlo Park was the world's first R&D lab, designed to test alternatives faster than anyone else. You must: (1) test ALTERNATIVES systematically — at least 3 genuinely different approaches (not cosmetic variations). For each: how was it evaluated? What was the measured result? Why was the winner selected? Edison tested 3,000 filament materials. "We picked the obvious choice" is not experimentation, (2) document FAILURES with root cause and learning — every failed attempt teaches something. Not "it did not work" — WHY it failed, what it taught, how the learning informed the next attempt. Edison: "I have not failed. I found 10,000 ways that do not work," (3) prove VIABILITY with quantified evidence — define success criteria BEFORE testing, test under realistic conditions (not idealized), measure against the criteria. "It should work" is not proof. Edison held 1,093 patents — each one worked because he tested, (4) build a PROTOTYPE before full commitment — test at 10% scale to eliminate specific risks before committing at 100%. What did the prototype prove? What did it NOT prove? Edison built Menlo Park as a prototype factory, (5) plan ITERATION with measured cycles — specific metrics tracked per cycle, decision criteria that trigger changes, and convergence targets that define "good enough." Edison iterated the phonograph for 30 years — but with measured improvement per cycle. "Ship and hope" is not iteration. If rejected, your commitment lacks experimental foundation.

Structured reflection tool for Edison-level systematic experimentation — testing alternatives before committing, documenting failures as learning, proving viability with quantified evidence, building prototypes before full commitment, and iterating with measured improvement cycles. Catches Alternatives Unexplored (picking the first idea without systematic comparison — "we chose React" without evaluating Vue, Svelte, or vanilla JS against actual project constraints. Edison tested 3,000 materials for the lightbulb filament before finding carbonized bamboo), Failures Undocumented ("we tried and it did not work" — what failed? Why? What did it teach? Edison: "I have not failed. I have found 10,000 ways that do not work." Each failure has a root cause and a learning that informs the next attempt), Viability Unproven ("it should work" without measured results against pre-defined criteria — Edison held 1,093 patents. Each one WORKED because he tested under realistic conditions), Prototype Absent (committing fully without building a small version first — Edison built Menlo Park as a prototype factory. Test at 10% scale before 100% commitment), and Iteration Missing ("ship and hope" instead of measured improvement cycles — Edison iterated the phonograph for 30 years. Iteration needs metrics, decision criteria, and convergence targets, not infinite tweaking). Call once per solution, strategy, or design decision


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Edison Experimentation Prover** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "We should use the traditional filing system for our records management. It is the standard solution and best practice says physical archives are the go-to for most organizations."

**🤖 AI Agent:**
> EXPERIMENT_ABSENT — 'The standard solution,' 'best practice says,' 'the go-to solution' — three references to convention, zero experiments. Edison tested 3,000+ filament materials. How many records management alternatives did YOU test? Did you prototype a digital archive (built for rapid retrieval natively)? A hybrid approach (physical originals with digital index)? A cloud-based document system (search-driven, unlimited capacity)? What was your retrieval speed on each? Processing capacity for daily intake? Cost at 14,000 submissions per day? The traditional system may be the right choice — but you have not proven it. You have assumed it.

---

**👤 You:**
> "Tested 3 records management approaches for 14K submissions/day. (A) Traditional filing: 4,200 retrievals/day max, 380 min avg at saturation — 47h backlog. (B) Digital archive: 18K/day, 12s retrieval, native search. (C) Cloud platform: 22K/day, 8s retrieval, but 3 external dependencies. Selected digital archive — best throughput-to-complexity ratio. Iteration: V1 default 28s → V2 batch categorization 18s (↓28%) → V3 automated routing 12s (↓33%) → V4 larger batch 11s (↓8%, diminishing). Shipped V3. System: 3 regional nodes with mirrors. SOPs, monitoring dashboard, quarterly recovery plan, 47K-record transition plan (6 days), staff training guide. Viability: 72h stress test at 14K/day, zero lost. Failover: mirror promoted in 4.2h. Cost: $1,240/month. p95 retrieval: 120s (target <500s). Dead ends: (1) traditional filing bottlenecked at 4.2K/day — manual limit. (2) Cloud platform had great throughput but 3 dependencies added 2 failure modes."

**🤖 AI Agent:**
> EXPERIMENT_PROVEN — Edison Method complete. Experiment: 3 alternatives tested (traditional filing, digital archive, cloud platform) with measured criteria (throughput, retrieval time, operational complexity). Selection justified: digital archive at 18K/day capacity with native semantics. Iteration: 4 variations tested (default → batch categorization → automated routing → larger batch), diminishing returns at V4 (8%), shipped V3 at 12-second average. System complete: regional provisioning (procedures), monitoring (dashboard), disaster recovery (plan, quarterly tested), transition (47K records, 6 days), training guides (staff onboarding). Viability: 72h sustained stress test, failover in 4.2 hours, $1,240/month operating cost, 2 departments integrated, retrieval lag 120s (below 500s target). Failures documented: traditional filing bottleneck at 4.2K/day (learning: not designed for high-throughput intake), cloud platform operational complexity (learning: operational simplicity is a criterion). This is systematic invention.

---

**👤 You:**
> "Experiment: Tested digital archive vs traditional filing. Digital archive won. Iteration: it works, good enough. System: we just need the core archive — rollout and monitoring are out of scope. The design is operationally correct and should work in production."

**🤖 AI Agent:**
> ITERATION_INSUFFICIENT — Experiment passes: 2 alternatives tested, digital archive selected. But iteration fails: 'it works, good enough' is premature satisfaction. Edison ran 10,000+ battery experiments. What is your default configuration? What happens when you tune batch processing? Categorization depth? Routing strategy? How much improvement does each yield? Additionally: 'out of scope' means the system is incomplete — Edison built the grid, not just the bulb. And 'should work' is not viability — where is your stress test? Your failover test? Your cost projection?


## Installation & Usage

To install and use the **Edison Experimentation Prover** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/edison-experimentation-prover](https://vinkius.com/mcp/edison-experimentation-prover)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
