# AI Ethics Prover MCP Server

An AI said 'AI should be fair and transparent' without naming a single affected group. It said 'we checked for bias' without naming a metric, attribute, or measured disparity. It said 'contact support' as the recourse mechanism. That is not ethics — that is ethics washing. This tool forces five operational axes: stakeholder identification, harm quantification, bias auditing, transparency demonstration, and recourse mechanisms.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/ai-ethics-prover)

## Overview
**Category:** ai-ml
**Tools Count:** 1

## Description
## The Problem

Ask an LLM to evaluate AI ethics. It will say 'AI should be fair' without naming who is affected. It will describe harms as 'potentially harmful' without measuring severity or probability. It will claim 'we checked for bias' without naming the metric, the protected attribute, or the measured disparity. And it will offer 'contact support' as the entire recourse mechanism.

Every LLM commits five ethics reasoning failures:
1. **Unnamed Stakeholders** — 'society' and 'users' are not stakeholders. Name specific groups with demographics, severity of impact, and vulnerability factors.
2. **Unquantified Harms** — 'potentially harmful' without severity (1-5), probability, reversibility, and affected population size.
3. **Unaudited Biases** — 'we checked for bias' without naming the protected attribute, detection metric, measured disparity, or acceptable threshold.
4. **Opaque Transparency** — 'algorithmic complexity' as an excuse for hiding decision logic from affected parties.
5. **Absent Recourse** — 'contact support' instead of a structured challenge channel with SLA, human reviewer, and appeal process.

## How It Works

The AI Ethics Prover forces the LLM to fill 5 reflection fields and commit to 5 Decision Pivots before concluding any ethics analysis is operationally adequate.

### The 5 Ethics Axes

| Axis | Pivot | Rule |
|---|---|---|
| **Stakeholders** | Identified | Named groups with impact type, severity, and vulnerability. |
| **Harms** | Quantified | Severity (1-5), probability, reversibility, population size. |
| **Biases** | Audited | Protected attribute, detection metric, measured disparity, threshold. |
| **Transparency** | Demonstrated | Explainable to affected parties with counterfactual examples. |
| **Recourse** | Available | Challenge channel, SLA, human reviewer, appeal process, remediation. |

### The Verdict Matrix

```
Axis 1 fails → STAKEHOLDERS_UNNAMED
Axis 2 fails → HARMS_UNQUANTIFIED
Axis 3 fails → BIASES_UNAUDITED
Axis 4 fails → TRANSPARENCY_OPAQUE
Axis 5 fails → RECOURSE_ABSENT
All pass     → ETHICS_PROVEN
```

## Why It Works

Tool calls are obligations. The LLM cannot skip stakeholder identification or claim bias was audited without methodology. It must name groups, score harms, cite metrics, demonstrate explainability, and define recourse. Every rejection names the exact ethics axis that failed.

**Disclaimer:** This is analytical support — it forces structured thinking about AI ethics. It does not prescribe ethical conclusions or replace qualified ethics review boards.


## Available Tools
- **validate_ai_ethics**: You must: (1) identify STAKEHOLDERS — name each affected group with demographics, impact type, severity, and vulnerability. "Society" and "users" are not stakeholders, (2) quantify HARMS — each harm has severity (1-5), probability (%), reversibility, and affected population size. "Potentially harmful" is not quantification, (3) audit BIASES — each protected attribute tested with a named metric (statistical parity, equalized odds, calibration), measured disparity, and mitigation plan. "We checked for bias" without methodology is not an audit, (4) demonstrate TRANSPARENCY — each stakeholder group gets explanation at their comprehension level with top decision factors and counterfactual "what-if" scenarios. "Algorithmic complexity" is not an excuse for opacity, (5) provide RECOURSE — structured challenge mechanism with response SLA, human reviewer, appeal process, and remediation for confirmed errors. "Contact support" is not recourse. If rejected, your ethics assessment has an analytical flaw.

Forces operationally specific AI ethics analysis before deploying AI systems. Catches Unnamed Stakeholders ("society" instead of specific groups), Unquantified Harms ("potentially harmful" without severity/probability), Unaudited Biases ("we checked" without methodology), Opaque Transparency ("algorithmic complexity" as excuse), and Absent Recourse ("contact support" instead of structured challenge). Call once per AI system ethical assessment. This is analytical support, not ethical certification


## Installation & Usage

To install and use the **AI Ethics Prover** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/ai-ethics-prover](https://vinkius.com/mcp/ai-ethics-prover)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
