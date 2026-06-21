# Estimation Prover MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/estimation-prover)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/estimation-prover-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/estimation-prover-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

An AI estimated a database migration at 2 weeks. It took 11 weeks, cost $340K in delayed revenue, and left 3 engineers stuck in feature freeze. The estimate had no scope decomposition, no unknowns identified, no historical precedent, and no buffer. This tool forces granular scope breakdown, explicit unknown quantification, precedent mapping, and realistic buffer calculation before any timeline is committed.

## Description
Software estimations are notoriously unreliable. The Planning Fallacy causes developers and AI agents to systematically underestimate timelines. Estimation Prover acts as a pre-commitment filter, enforcing structured estimation techniques based on historical references and decomposition.

### The Problem It Solves

Software estimates fail on five key axes:

- **Vague scope** — Giving a single timeline (e.g. "3 weeks") without breaking down the work. This makes tracking impossible.
- **Hidden unknowns** — Ignoring architectural risks, external API integrations, or library deprecations, assuming perfect execution.
- **Lack of precedent** — Fabricating estimates from thin air, completely disconnected from how long similar tasks actually took in the past.
- **Missing buffer** — Failing to allocate contingency time. If a single task runs late, the entire project timeline slips.
- **Implicit assumptions** — Leaving team availability or scope boundaries unstated. When these change, the estimate fails.

### How It Works

Estimation Prover uses 5 Decision Pivots to evaluate and validate estimates:

1. **scopeDecomposed** — Is the work broken down into discrete units (ideally ≤2 days each)?
2. **unknownsIdentified** — Are technical risks and external dependencies documented with impact ranges?
3. **historicalReferenced** — Is the timeline supported by concrete base rates from past tasks?
4. **bufferApplied** — Is a realistic contingency buffer (minimum 20% for known work, 40%+ for novel tasks) included?
5. **assumptionsStated** — Are all dependencies, resource availability, and scope limits explicitly defined?

### Why It Works

- **Decomposition enforcement.** Forcing the breakdown of complex milestones into micro-tasks immediately exposes scope creep.
- **Reference Class Forecasting.** By grounding estimates in historical data, it shifts the focus from optimistic predictions to historical reality. Past overruns are used as warning metrics for new tasks.


## Available Tools
- **validate_estimation**: The Planning Fallacy (Kahneman 1979) proves humans systematically underestimate by 25-50% — even when they KNOW about the bias. The only defense is structured estimation. You must: (1) DECOMPOSE scope into units ≤2 days each — each with its own estimate. A single estimate for a multi-day task is a guess. Decomposition forces specificity, (2) MAP unknowns — technical risks, knowledge gaps, dependency uncertainties. For each: name, likelihood (low/med/high), impact on timeline if it materializes. The unknowns will blow the estimate, not the knowns, (3) cite a SPECIFIC historical precedent — not "based on experience." Reference Class Forecasting (Flyvbjerg 2006): name the project, how long it took, how accurate the original estimate was, and how THIS task compares, (4) apply a CONTINGENCY buffer with a NUMBER — ≥20% for familiar work, 40-60% for novel work with unknowns. The Cone of Uncertainty (McConnell) shows early estimates are 4x off. A buffer without a number is not a buffer, (5) state EVERY assumption — team availability, scope stability, API reliability, reviewer responsiveness, infrastructure readiness. "No assumptions" means you have not examined. If rejected, your estimate has a blind spot.

Structured reflection tool for project estimation — forces decomposition, unknown mapping, historical grounding, contingency buffers, and explicit assumptions BEFORE committing to a timeline. Based on Reference Class Forecasting (Kahneman/Flyvbjerg), Cone of Uncertainty (McConnell), and Planning Fallacy research (universal 25-50% underestimation). Catches Scope Vague ("auth work" instead of "migrate JWT to OAuth 2.1 with refresh token rotation, update 3 API endpoints, update React auth context, write migration tests" — vague scope produces vague estimates), Unknowns Hidden (estimating without mapping technical risks, knowledge gaps, and dependency uncertainties — the things you do not know will blow the timeline, not the things you do know), No Precedent ("based on experience" instead of "the auth migration at Company X took 3 sprints, estimated at 1.5 sprints, because OAuth discovery flow testing took 2x longer than expected" — Reference Class Forecasting requires SPECIFIC historical precedent), No Buffer (estimates without contingency — Kahneman proved humans underestimate by 25-50%. A buffer is not padding — it is correcting for a known cognitive bias), and Assumptions Implicit ("2 weeks" without stating that this assumes full-time allocation, stable scope, available API documentation, responsive code reviewers, and working CI pipeline). Call once per estimation


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Estimation Prover** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Let's build a new mobile catalog. It should take around 2 weeks since the requirements are straightforward."

**🤖 AI Agent:**
> Verdict: SCOPE_VAGUE. A single 2-week estimate lacks task decomposition. Break the catalog work into clear components: database sync, listing UI, navigation actions, cache storage, and reviews. Define time estimates for each unit to build a reliable timeline.

---

**👤 You:**
> "Task: build mobile catalog. Breakdown: 1. local SQLite DB sync (2 days), 2. layout grid UI (2 days), 3. detail views (1 day), 4. offline image caching (2 days). Unknowns: SQLite sync conflicts. Precedent: last year's web catalog SQLite sync took 3 days due to sync conflicts. Buffer: 30% added (2.1 days buffer on 7 days total). Assumptions: requirements do not change during development, team size is 1 developer."

**🤖 AI Agent:**
> Verdict: ESTIMATION_PROVEN. Scope is decomposed into tasks ≤2 days. SQLite risks are identified. Grounded in precedent (last year's sync issues). Realistic 30% buffer applied. Scope assumptions are explicit. This estimate is verified.

---

**👤 You:**
> "Task: mobile catalog. Decomposition: SQLite sync (2 days), grid UI (2 days), detail views (1 day), image caching (2 days). Unknowns: Sync conflicts. Precedent: last year's SQLite sync. Buffer: none needed since requirements are simple. Assumptions: requirements do not change, 1 dev."

**🤖 AI Agent:**
> Verdict: NO_BUFFER. You have omitted a contingency buffer. Even if requirements seem simple, SQLite sync conflicts are an identified risk. Apply a minimum 20% buffer to account for integration delays.


## Installation & Usage

To install and use the **Estimation Prover** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/estimation-prover](https://vinkius.com/mcp/estimation-prover)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
