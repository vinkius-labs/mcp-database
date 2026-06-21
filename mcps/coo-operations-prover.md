# COO Operations Prover MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/coo-operations-prover)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [infrastructure](../categories/infrastructure.md)

An operations plan said 'we will scale' without modeling arrival rates. It claims 'economies of scale' without a single cost data point. It writes SLAs that say 'best effort.' That is not operations — that is hope. This tool forces five COO-level operational axes: capacity modeling, failure isolation, cost leverage, process discipline, and accountability mechanisms.

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


## 💬 Prompt Examples

Here are some examples of how you can interact with the **COO Operations Prover** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "We will scale our platform as needed using auto-scaling groups. We have economies of scale. Our processes handle exceptions on a case-by-case basis. Our SLA commits to best effort uptime."

**🤖 AI Agent:**
> CAPACITY_BLIND — Four fatal gaps. First: 'auto-scaling' is not capacity modeling — define arrival rate, service rate, and utilization threshold. Second: 'economies of scale' is a claim — show cost per unit at 3 data points. Third: 'case-by-case' is process chaos — quantify exception rate and provide runbooks. Fourth: 'best effort' is accountability theater — define error budget and automated penalties.

---

**👤 You:**
> "Peak arrival: 1,200 req/s. Service capacity: 1,800 req/s across 6 workers (300/s each). Utilization: 67%. Queue drain: 200ms p99. Headroom: 33%. Tenant isolation: database-per-tenant. Regional blast radius: max 8% per region (12 regions). Circuit breaker on payment: 5s timeout, 3 retries. Cost: $0.12/user at 10K, $0.04 at 100K, $0.008 at 1M (committed use + CDN 94% hit). SOP coverage: 94%. Exception rate: 3.2%. Top 3 categorized with runbooks, 15min resolution. SLA: 99.9%. Error budget: 43.8 min/month. If burned: feature deploys freeze. If 50% burned mid-sprint: escalation to VP Eng."

**🤖 AI Agent:**
> OPERATIONS_PROVEN — Wartime COO operations validated. Capacity: 1,200/1,800 req/s (67% utilization, 33% headroom). Failure isolation: database-per-tenant, 8% max blast radius, circuit breaker on payments. Cost leverage: $0.12 → $0.04 → $0.008/user across 3 scale points. Process discipline: 94% SOP, 3.2% exception rate, runbooks with 15min resolution. Accountability: 99.9% SLA, 43.8 min/month error budget, automatic deploy freeze. Execute.

---

**👤 You:**
> "Our infrastructure uses auto-scaling on AWS. Costs will decrease as we grow — volume discounts. We handle exceptions flexibly. SLA: 99.9% uptime, we will investigate any incidents and send a post-mortem within 48 hours."

**🤖 AI Agent:**
> CAPACITY_BLIND — Four fatal gaps in sequence. (1) 'Auto-scaling on AWS' is not capacity modeling — where is the arrival rate, service rate, and utilization threshold? (2) 'Volume discounts' is cost delusion — show the per-unit cost at 10K, 100K, and 1M with the mechanism. (3) 'Flexibly' handling exceptions is process chaos — quantify the exception rate. (4) 'Investigate and post-mortem' is accountability theater — that is a press release, not an error budget with automated consequences.


## ❓ FAQ

**Q: Why does it reject 'we will scale as needed'?**
'We will scale' is hope, not a capacity model. A wartime COO demands numbers: arrival rate (1,200 req/s), service rate (1,800 req/s across 6 workers), utilization (67%), and queue drain behavior under burst (200ms p99). Without these numbers, you do not know when the system saturates. 'Auto-scale' is not modeling — it is outsourcing the thinking to the cloud provider.

**Q: Why does it demand cost at 3 data points?**
Because 'economies of scale' is a claim — not proof. Anyone can say costs decrease at scale. Proof means showing per-unit cost at 3 specific volume points: '$0.12/user at 10K, $0.04/user at 100K, $0.008/user at 1M.' And naming the mechanism: shared compute amortization, committed use discounts, CDN cache hit ratio. If the cost per unit stays flat, you have a service agency, not a platform.

**Q: What is 'Accountability Theater'?**
It is when you write an SLA that says '99.9% uptime' but the consequence for missing it is 'we will investigate.' That is a press release, not accountability. SRE error budgets require automated penalties: if the error budget burns (43.8 minutes/month for 99.9%), feature deploys freeze automatically until reliability recovers. 'Best effort' is the opposite of a mechanism.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/coo-operations-prover](https://vinkius.com/mcp/coo-operations-prover)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **COO Operations Prover** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `coo-operations-prover` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **COO Operations Prover** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "coo-operations-prover": {
      "url": "https://edge.vinkius.com/[TOKEN]/mcp"
    }
  }
}
```

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
