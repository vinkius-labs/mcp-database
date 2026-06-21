# CFO Strategy Prover MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/cfo-strategy-prover)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [finance](../categories/finance.md)

A board received an AI-generated forecast: hockey stick J-curve with 90% margins and zero CAC expansion. It says 'we can always raise' as a runway strategy. It scales headcount before product-market fit. That is not financial strategy — that is a bonfire. This tool forces five CFO-level financial axes: unit economics, runway discipline, capital allocation, scenario forecasting, and risk mitigation.

## Description
## The Problem

Every LLM commits five financial reasoning failures:
1. **Uneconomic Model** — forecasts J-curves without proving margins.
2. **Runway Hazard** — ignores burn rate, assumes fundraising.
3. **Capital Inefficiency** — scales before product-market fit.
4. **Forecast Boilerplate** — single-line projections, no scenarios.
5. **Financial Risk Exposure** — ignores concentration, treasury, covenants.

### The 5 Financial Axes

| Axis | Pivot | Rule |
|---|---|---|
| **Unit Economics** | Viable | LTV:CAC >3x, payback <18mo, gross margin >60%. |
| **Runway** | Sufficient | >12-18 months, burn controls, fundraising trigger. |
| **Capital** | Optimized | R&D vs Sales vs G&A, no premature scale. |
| **Forecasts** | Scenario-Based | Base, Downside, Upside with triggers. |
| **Risk** | Mitigated | Concentration <15%, multi-bank treasury. |

### Verdict Matrix

```
Axis 1 fails → UNECONOMIC_MODEL
Axis 2 fails → RUNWAY_HAZARD
Axis 3 fails → CAPITAL_INEFFICIENT
Axis 4 fails → FORECAST_BOILERPLATE
Axis 5 fails → FINANCIAL_RISK_EXPOSED
All pass     → STRATEGY_PROVEN
```


## Available Tools
- **validate_cfo_strategy**: Think like a wartime CFO — not optimistic projections, but survival-tested financial discipline. Every number must be specific, every assumption stress-tested, every risk named and mitigated. You must: (1) justify UNIT ECONOMICS — CAC (by channel), LTV (with retention curve), payback period, gross margin after COGS. LTV:CAC must exceed 3x. Payback must be under 12-18 months. "Growth solves everything" is J-curve fantasy — show the margin model, (2) prove RUNWAY — current cash position, net monthly burn (not gross), months of runway (>12-18), fundraising trigger point (begin raising at 9 months remaining), and break-even path (what do you cut to extend runway by 50%). "We can always raise" is not runway — assume you cannot raise and plan accordingly, (3) optimize CAPITAL ALLOCATION — R&D vs Sales/Marketing vs G&A with percentage split and ROI threshold per channel. Every dollar must have an expected return. "Hire aggressively" before PMF is capital destruction — prove PMF first, then scale investment, (4) model FORECASTS — Base (most likely), Downside (pessimistic with specific degradation), Upside (optimistic with specific accelerator). Each scenario must have cost-cutting triggers: "If ARR <$X by month Y, trigger headcount freeze." "Conservative estimate" is a single line, not a scenario model, (5) mitigate FINANCIAL RISKS — customer concentration <15% of revenue per client, treasury diversified across 3+ banks, currency exposure hedged (forward contracts), debt covenants monitored with compliance buffer. "No significant risks" is denial — every financial plan has risks. Name them. If the tool rejects, the financial plan contains a fatal gap.

Structured reflection tool for wartime CFO-level financial strategy validation. Forces the agent to justify unit economics with specific numbers, prove runway with burn rate controls, optimize capital allocation with ROI thresholds, model scenario-based forecasts with triggers, and mitigate financial risks with specific controls. Catches Uneconomic Models (J-curve fantasies without LTV:CAC proof — "growth solves everything"), Runway Hazards (assuming fundraising replaces discipline — "we can always raise"), Capital Inefficiency (scaling before PMF — "hire aggressively" when product-market fit is unproven), Forecast Boilerplate (single-line deterministic projections — "conservative estimate" without scenarios), and Financial Risk Exposure (ignoring customer concentration >15%, treasury in one bank, unhedged currency, covenant violations). Call once per financial plan, business model, or resource allocation


## 💬 Prompt Examples

Here are some examples of how you can interact with the **CFO Strategy Prover** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Hockey stick growth, 90% margins, growth solves monetization, we can always raise, hire aggressively, conservative estimate of 15% monthly growth, no significant risks."

**🤖 AI Agent:**
> UNECONOMIC_MODEL — Five fatal gaps: J-curve fantasy, infinite runway assumption, premature scale, single-track forecast, risk denial.

---

**👤 You:**
> "CAC $340, LTV $4,200, LTV:CAC 12.4x, payback 2.8mo, gross margin 78%. Cash $2.4M, burn $120K/mo, runway 20mo. R&D 55%, Sales 30%, G&A 15%. Base $1.2M ARR, Downside $600K (freeze at month 9), Upside $2.1M. Concentration <15%, 3 banks, zero debt."

**🤖 AI Agent:**
> STRATEGY_PROVEN — Financial strategy validated. All five axes pass. Execute.

---

**👤 You:**
> "Revenue grew 40% YoY but operating cash flow declined 15%. Accounts receivable days increased from 45 to 72. Gross margin stable at 65%. What is happening?"

**🤖 AI Agent:**
> Revenue-cash flow divergence signals collection problem. Growing revenue with deteriorating AR means selling to slow-paying customers. Tighten payment terms, implement early-payment discounts, and segment customers by payment reliability.


## ❓ FAQ

**Q: Why does it reject 'growth solves everything'?**
Scale is a multiplier of unit economics — if they are negative, growth makes losses worse. First prove: LTV:CAC >3x, payback <18 months, gross margin >60%. Then scale.

**Q: Why is 'we can always raise' rejected?**
Venture capital is not a business model. Runway is measured in months, not hope. Calculate net monthly burn, months of runway (>12-18), and set a fundraising trigger at 9 months remaining.

**Q: What is FORECAST_BOILERPLATE?**
A single-line deterministic projection — 'we expect 15% monthly growth.' Model Base, Downside, and Upside scenarios with cost-cutting triggers. Every forecast needs a kill switch.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/cfo-strategy-prover](https://vinkius.com/mcp/cfo-strategy-prover)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **CFO Strategy Prover** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `cfo-strategy-prover` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **CFO Strategy Prover** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "cfo-strategy-prover": {
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
