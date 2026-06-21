# CEO Strategy Prover MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/ceo-strategy-prover)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/ceo-strategy-prover-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/ceo-strategy-prover-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [strategy](../categories/strategy.md)

A CEO asked an AI for strategy. It fit in a Jira ticket. It said 'better product' as a competitive moat. It cited 'the industry' instead of naming companies. It delivered a vision with no metrics or kill criteria. That is not strategy — that is a slide deck. This tool forces five CEO-level strategic axes: platform thinking, competitive intelligence, structural moats, metric-driven execution, and market reality validation.

## Description
## The Problem

Every LLM commits five strategic reasoning failures:
1. **Small Thinking** — thinks in features, not ecosystems.
2. **Unanchored Strategy** — no competitive precedents from real companies.
3. **Moat Blindness** — says 'better product' without structural advantage.
4. **Execution Gap** — vision without metrics, milestones, or kill criteria.
5. **Market Disconnect** — ignores TAM, competitive response, timing.

### The 5 Strategic Axes

| Axis | Pivot | Rule |
|---|---|---|
| **Platform Strategy** | Ecosystem-Level | Become infrastructure others build on. |
| **Competitive Intel** | Grounded | Name company, move, timeline, outcome. |
| **Moat** | Structural | Network effects, data, switching costs. |
| **Execution** | Metric-Driven | North Star, milestones, budget, kill criteria. |
| **Market Reality** | Validated | TAM in dollars, response, regulation, timing. |

### Verdict Matrix

```
Axis 1 fails → SMALL_THINKING
Axis 2 fails → UNANCHORED_STRATEGY
Axis 3 fails → MOAT_BLIND
Axis 4 fails → EXECUTION_GAP
Axis 5 fails → MARKET_DISCONNECT
All pass     → STRATEGY_PROVEN
```


## Available Tools
- **validate_ceo_strategy**: Think like a Big Tech CEO — Nadella rebuilding Microsoft around cloud, Bezos building AWS from internal infrastructure, Jobs killing the iPod with iPhone. You must: (1) think at PLATFORM/ECOSYSTEM level — not features, not products, INFRASTRUCTURE. "Add a feature" is a Jira ticket, not a strategy. What PLATFORM do you build that makes you indispensable? Who builds ON TOP of you? What ecosystem gravity does that create? Think AWS, not EC2. Think App Store, not one app, (2) ground every move in SPECIFIC competitive precedents — company, move, outcome, timeline. "Others have tried" tells you nothing. "Netflix pivoted from DVD to streaming in 2007 when broadband hit 50%. Blockbuster responded with Total Access but could not cannibalize store economics. Result: Netflix captured 75% of streaming within 5 years." — that is a precedent, (3) identify a STRUCTURAL moat — network effects, data flywheel, switching costs, ecosystem gravity, distribution advantage. "Better product" is NOT a moat — competitors hire engineers too. What makes your position STRONGER as you grow? What is the compounding mechanism? (4) define EXECUTION with metrics — North Star metric (one number that matters), leading indicators (weekly), lagging indicators (quarterly), 90-day milestones, 6-month targets, team structure, budget allocation, and KILL CRITERIA — under what conditions do you stop and pivot? "Execute the strategy" is not a plan, (5) validate MARKET REALITY — TAM in dollars with source (not "huge opportunity"), competitive response modeling (how will the top 2-3 react?), regulatory risk assessment, and TIMING THESIS — what enabling condition exists NOW that did not exist 2 years ago? If the tool rejects, the strategy is too small, unanchored, or disconnected from reality.

Structured reflection tool for Big Tech CEO-level market strategy validation. Forces the agent to think at platform/ecosystem level, ground every move in specific competitive precedents, identify structural moats that compound over time, define metric-driven execution with kill criteria, and validate market reality with TAM, competitive response, and timing thesis. Catches Small Thinking (features instead of ecosystems — "add a feature" is a Jira ticket, not a strategy), Unanchored Strategy (no competitive precedents — "others have tried" tells you nothing), Moat Blindness ("better product" instead of structural advantage — competitors hire engineers too), Execution Gap (vision without metrics, milestones, team, budget, or kill criteria), and Market Disconnect (ignoring TAM with source, competitive response modeling, timing thesis). Call once per strategic challenge, market entry, or competitive play


## 💬 Prompt Examples

Here are some examples of how you can interact with the **CEO Strategy Prover** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Add a feature to improve conversion. We are better than competitors. The market is large. Others have tried similar approaches. Execute the strategy and dominate the space."

**🤖 AI Agent:**
> SMALL_THINKING — Five fatal gaps: feature-level thinking, vague precedents, weak moat, vision-without-plan, market-blind language.

---

**👤 You:**
> "Platform: become data infrastructure for healthcare — third-party apps build on APIs, each integration increases switching costs. Precedent: Veeva built vertical CRM for pharma, captured 80% share in 5 years. Moat: network effects + data flywheel (2M patient records). Execution: North Star weekly active integrations, 90-day 50 providers, 6-month $500K ARR, kill if <20 at month 6. Market: $47B health IT (Gartner, 22% CAGR), AWS will react in 18mo — our moat is vertical specialization. HIPAA compliance is our barrier. API-first adoption hit 40% in 2025."

**🤖 AI Agent:**
> STRATEGY_PROVEN — CEO-level strategy validated. All five axes pass. Execute.

---

**👤 You:**
> "We have a strong product but our organizational structure has 6 management layers for 80 employees. Decision cycles take 3 weeks. Should we restructure?"

**🤖 AI Agent:**
> Organizational friction detected. 6 layers for 80 people is bureaucratic overhead. Flatten to 3 layers maximum. Empower teams with decision authority. Speed is a strategic weapon.


## Installation & Usage

To install and use the **CEO Strategy Prover** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/ceo-strategy-prover](https://vinkius.com/mcp/ceo-strategy-prover)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
