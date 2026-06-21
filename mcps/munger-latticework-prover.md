# Munger Latticework Prover MCP Server

Charlie Munger spent 60 years proving that a man with one model is a man with a hammer — every problem looks like a nail. An AI proposed a strategy without inverting it, without tracing second-order effects, without mapping incentive conflicts, without admitting what it does not know, and without a margin of safety for being wrong. That is not analysis — that is a first draft dressed as a final answer. This tool forces five Munger-level mental models: inversion, second-order effects, incentive architecture, circle of competence, and margin of safety.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/munger-latticework-prover)

## Overview
**Category:** strategy
**Tools Count:** 1

## Description
## The Problem

LLMs commit five multi-model reasoning failures:
1. **Forward-Only** — asks how to succeed, never how to FAIL.
2. **First-Order Fixation** — sees immediate effect, ignores consequences of consequences.
3. **Incentive Blindness** — ignores that incentives drive ALL behavior.
4. **Competence Overreach** — reasons confidently outside expertise.
5. **Fragility Tolerance** — proposes strategies with zero buffer for being wrong.

### The 5 Munger Mental Models

| Model | Pivot | Rule |
|---|---|---|
| **Inversion** | Applied | How does this FAIL? 5 catastrophic failure modes. |
| **Second-Order** | Traced | 1st → 2nd → 3rd order consequences mapped. |
| **Incentives** | Mapped | Every stakeholder's reward and conflict exposed. |
| **Competence** | Bounded | Inside, edge, and outside drawn honestly. |
| **Safety** | Buffered | Base, bear (-30%), worst (-50%), break-even. |

### Verdict Matrix

```
Model 1 fails → FORWARD_ONLY
Model 2 fails → FIRST_ORDER_FIXATION
Model 3 fails → INCENTIVE_BLIND
Model 4 fails → COMPETENCE_OVERREACH
Model 5 fails → FRAGILITY_TOLERANT
All pass      → LATTICEWORK_PROVEN
```


## Available Tools
- **validate_munger_latticework**: Think like Charlie Munger — apply multiple mental models: (1) INVERSION — "Invert, always invert." How will this FAIL? List 5 catastrophic failure modes. Pre-mortem, not post-mortem. If you cannot find 5, you have not thought about it, (2) SECOND-ORDER EFFECTS — what happens AFTER the first effect? Trace 3 orders of consequences. First order is obvious. Second order is where strategies die. Third order is where companies die, (3) INCENTIVE ARCHITECTURE — "Show me the incentives, I show you the outcome." Map every stakeholder. Where do incentives CONFLICT with desired behavior? Incentives predict outcomes better than intentions, (4) CIRCLE OF COMPETENCE — "Know the edge of your circle." Where are you reasoning with genuine expertise? Where are you at the edge? Where are you outside — and who should you defer to?, (5) MARGIN OF SAFETY — what if you are 50% wrong? Base case, bear case (-30%), worst case (-50%), break-even. Does the strategy survive the worst case? A strategy that only works in the base case is a bet. If rejected, fix the specific mental model gap.

Structured reflection tool for multi-disciplinary strategic reasoning — forces inversion thinking, second-order consequence tracing, incentive architecture mapping, competence boundary honesty, and margin of safety verification before any major strategic decision. Models Charlie Munger's latticework of mental models: the world is not divided into disciplines, and the strategist who only uses one mental model is "a man with a hammer — everything looks like a nail." Catches Forward-Only Thinking (planning only for success without mapping failure — "Invert, always invert." A startup plans to scale from 10 to 100 employees in 12 months. The plan describes: office expansion, hiring pipeline, culture initiatives, revenue targets. The inversion question is never asked: "How will this company die?" Answer: (1) burn rate exceeds runway at month 8 if revenue misses by 20%. (2) Key engineer quits — she wrote 60% of the payment integration, undocumented. (3) The largest client (42% of revenue) has a 90-day termination clause. (4) AWS bill compounds 3x with user growth because of N+1 queries nobody profiled. (5) The co-founder equity split is verbal, not documented — litigation risk at Series A. If you cannot list 5 catastrophic failure modes, you have not thought about your strategy), First-Order Fixation (seeing only the immediate effect without tracing consequences — "We will reduce prices by 30% to increase market share." First order: sales volume increases 40%. Good. Second order: competitors match the price cut within 2 weeks. Net market share gain: 3% instead of projected 15%. Third order: the new price becomes the anchored market price. Raising prices back is now a 25% increase that customers perceive as a betrayal. The price cut is permanent. Margins never recover. Amazon's free shipping threshold was a first-order decision that created a third-order expectation: "shipping should always be free"), Incentive Blindness (ignoring that people respond to incentives, not speeches — "Show me the incentive and I will show you the outcome." A sales team is incentivized on new revenue. Result: they sell 12-month contracts at 40% discount to hit quarterly targets. Customer Success team is incentivized on retention. They inherit clients acquired at unprofitable margins. Churn is 60% at renewal because the value proposition never matched the discounted price. Sales celebrates. CS fires. Finance bleeds. The incentive structure guaranteed the outcome — the people were rational actors), Competence Overreach (reasoning confidently outside your expertise — "Knowing what you don't know is more useful than being brilliant." A software engineer confidently designs a HIPAA compliance strategy for a healthcare startup. They encrypt data at rest and in transit. They add role-based access control. They miss: Business Associate Agreements with every vendor, breach notification procedures within 60 days under 45 CFR § 164.404, physical safeguard requirements for on-site servers, and minimum necessary access standards. The engineer was competent in security — but the question was regulatory compliance, not security), and Fragility Tolerance (building a strategy with no margin for error — "The best idea or opportunities are only available at a particular price." A real estate developer finances a project at 95% LTV assuming 8% rental yield. Base case: 12% IRR. Beautiful. What if interest rates rise 200 bps? IRR drops to 3%. What if vacancy is 15% instead of 5%? Negative cash flow from month 6. What if construction runs 30% over budget? The equity is wiped out. A strategy that only works in the base case is not a strategy — it is a bet. Margin of safety means: the strategy survives even if you are 50% wrong). Call once per strategic decision, investment thesis, or business plan


## Installation & Usage

To install and use the **Munger Latticework Prover** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/munger-latticework-prover](https://vinkius.com/mcp/munger-latticework-prover)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
