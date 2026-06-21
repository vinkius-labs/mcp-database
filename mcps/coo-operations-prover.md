# COO Operations Prover MCP Server

An operations plan said 'we will scale' without modeling arrival rates. It claims 'economies of scale' without a single cost data point. It writes SLAs that say 'best effort.' That is not operations — that is hope. This tool forces five COO-level operational axes: capacity modeling, failure isolation, cost leverage, process discipline, and accountability mechanisms.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/coo-operations-prover)

## Overview
**Category:** infrastructure
**Tools Count:** 1

## Description
## The Problem

Ask an LLM to design an operational plan. It will say 'we will scale as needed.' It will claim 'economies of scale' without showing cost at a single data point. It will accept 'case-by-case' exception handling as a process. And it will write SLAs that say 'best effort' — which means nothing.

Every LLM commits five operational reasoning failures:
1. **Capacity Blindness** — says 'we will scale' without modeling arrival rate vs service rate.
2. **Contagion Risk** — designs without bulkheads; one shard failure cascades everywhere.
3. **Cost Delusion** — claims 'economies of scale' without proof at 3 data points.
4. **Process Chaos** — accepts snowflake exceptions that destroy operational leverage.
5. **Accountability Theater** — writes SLAs without automated penalties.

## How It Works

The COO Operations Prover forces the LLM to fill 5 reflection fields and commit to 5 Decision Pivots before concluding any operational plan is execution-ready.

### The 5 Operational Axes

| Axis | Pivot | Rule |
|---|---|---|
| **Capacity Design** | Modeled | Arrival rate, service rate, utilization, queue behavior. |
| **Failure Isolation** | Contained | Bulkheads, blast radius limits, circuit breakers. |
| **Cost Leverage** | Decreasing | Per-unit cost at 3 scale points with mechanism. |
| **Process Discipline** | Standard | Exception rate below 5%, SOPs, runbooks. |
| **Accountability** | Enforced | SLA target, error budget, automated penalties. |

### The Verdict Matrix

```
Axis 1 fails → CAPACITY_BLIND
Axis 2 fails → CONTAGION_RISK
Axis 3 fails → COST_DELUSIONAL
Axis 4 fails → PROCESS_CHAOTIC
Axis 5 fails → ACCOUNTABILITY_THEATER
All pass     → OPERATIONS_PROVEN
```

## Why It Works

Tool calls are obligations. The LLM cannot say 'we will scale' — it must model the arrival rate vs service rate. It cannot claim 'economies of scale' — it must show cost at 3 data points. It cannot write 'best effort' SLAs — it must define the error budget and automated penalty. Every rejection names the exact operational axis that failed.


## Available Tools
- **validate_coo_operations**: Think like a wartime COO — not aspirational capacity charts, but battle-tested operational readiness that survives peak load, component failure, and cost pressure. You must: (1) model CAPACITY with queuing theory — arrival rate (λ), service rate (μ), utilization (ρ = λ/μ), queue length under peak, drain time after burst. "We will scale" is aspiration — show the numbers that prove capacity exceeds demand with headroom, (2) prove FAILURE ISOLATION — name every bulkhead (tenant isolation, regional failover, circuit breakers), blast radius limit (% of capacity affected by a single failure), and degradation strategy (what degrades gracefully vs what fails hard). "Cloud provider handles it" is not isolation — your application must have its own bulkheads, (3) prove COST LEVERAGE — show per-unit cost at 3 specific scale points with the mechanism driving decrease (shared compute, committed discounts, cache hit ratios). "Economies of scale" is a claim — prove it with 3 data points, (4) quantify PROCESS DISCIPLINE — SOP coverage %, exception rate (target <5%), top 3 exception categories with runbooks and resolution time. "Case-by-case" handling above 5% exception rate means your process is broken, not flexible, (5) enforce ACCOUNTABILITY — SLA target (99.9%), error budget in minutes (43.8 min/month), and the AUTOMATIC penalty when the budget burns (feature freeze, not a meeting). "Best effort" is theater — accountability requires automated consequences. If rejected, your operational plan has a fatal gap.

Structured reflection tool for wartime COO-level operational readiness validation. Forces the agent to model capacity with queuing theory, prove failure isolation with bulkheads and blast radius limits, demonstrate cost leverage at 3 scale points, quantify process discipline with exception rates and runbooks, and enforce accountability with automated SLA penalties. Catches Capacity Blindness ("we will scale" without modeling arrival rate vs service rate, utilization thresholds, or queue drain behavior under peak load), Contagion Risk (no bulkheads — one failure cascades everywhere because components share connection pools, databases, or thread pools without isolation), Cost Delusion ("economies of scale" claimed without proving marginal cost decrease at 3 data points with the specific mechanism driving the decrease), Process Chaos (exception rate >5% destroying operational leverage — "case-by-case" handling for situations that should have runbooks), and Accountability Theater (SLAs as marketing promises — no error budget, no automated penalties, no feature-freeze trigger when reliability degrades). Call once per operational plan or system design review


## Installation & Usage

To install and use the **COO Operations Prover** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/coo-operations-prover](https://vinkius.com/mcp/coo-operations-prover)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
