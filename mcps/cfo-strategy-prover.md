# CFO Strategy Prover MCP Server

A board received an AI-generated forecast: hockey stick J-curve with 90% margins and zero CAC expansion. It says 'we can always raise' as a runway strategy. It scales headcount before product-market fit. That is not financial strategy — that is a bonfire. This tool forces five CFO-level financial axes: unit economics, runway discipline, capital allocation, scenario forecasting, and risk mitigation.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/cfo-strategy-prover)

## Overview
**Category:** finance
**Tools Count:** 1

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


## Installation & Usage

To install and use the **CFO Strategy Prover** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/cfo-strategy-prover](https://vinkius.com/mcp/cfo-strategy-prover)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
