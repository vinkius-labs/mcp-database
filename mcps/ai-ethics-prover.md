# AI Ethics Prover MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/ai-ethics-prover)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [ai-ml](../categories/ai-ml.md)

An AI said 'AI should be fair and transparent' without naming a single affected group. It said 'we checked for bias' without naming a metric, attribute, or measured disparity. It said 'contact support' as the recourse mechanism. That is not ethics — that is ethics washing. This tool forces five operational axes: stakeholder identification, harm quantification, bias auditing, transparency demonstration, and recourse mechanisms.

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


## Available Tools (1)
- **validate_ai_ethics**: You must: (1) identify STAKEHOLDERS — name each affected group with demographics, impact type, severity, and vulnerability. "Society" and "users" are not stakeholders, (2) quantify HARMS — each harm has severity (1-5), probability (%), reversibility, and affected population size. "Potentially harmful" is not quantification, (3) audit BIASES — each protected attribute tested with a named metric (statistical parity, equalized odds, calibration), measured disparity, and mitigation plan. "We checked for bias" without methodology is not an audit, (4) demonstrate TRANSPARENCY — each stakeholder group gets explanation at their comprehension level with top decision factors and counterfactual "what-if" scenarios. "Algorithmic complexity" is not an excuse for opacity, (5) provide RECOURSE — structured challenge mechanism with response SLA, human reviewer, appeal process, and remediation for confirmed errors. "Contact support" is not recourse. If rejected, your ethics assessment has an analytical flaw.

Forces operationally specific AI ethics analysis before deploying AI systems. Catches Unnamed Stakeholders ("society" instead of specific groups), Unquantified Harms ("potentially harmful" without severity/probability), Unaudited Biases ("we checked" without methodology), Opaque Transparency ("algorithmic complexity" as excuse), and Absent Recourse ("contact support" instead of structured challenge). Call once per AI system ethical assessment. This is analytical support, not ethical certification


## 💬 Prompt Examples

Here are some examples of how you can interact with the **AI Ethics Prover** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Our AI lending model is fair and transparent. We checked for bias and the results are satisfactory. Users can contact support if they have concerns about decisions."

**🤖 AI Agent:**
> BIASES_UNAUDITED — 'Checked for bias' without methodology is not an audit. Which protected attributes — age, gender, race, income bracket? Which metric — statistical parity, equalized odds, disparate impact ratio? What was the measured disparity — 0.82 approval rate for Group A vs 0.67 for Group B? What is the acceptable threshold? Also: 'contact support' is not recourse — define SLA, human reviewer, and appeal process.

---

**👤 You:**
> "Stakeholders: loan applicants (18-65, primary), denied applicants (high-severity, financially vulnerable). Harms: wrongful denial — severity 4/5, probability 12% for minorities, reversible via re-evaluation, affects 15,000 applicants/year. Bias audit: race (statistical parity, 0.82 vs 0.67 approval, threshold 0.80 — FAILING), gender (equalized odds, 0.91 vs 0.89, threshold 0.85 — PASSING). Mitigation: reweighting training data, quarterly re-audit. Transparency: plain-language denial letters with top-3 factors and counterfactual examples. Recourse: online challenge form, 5-day SLA, human credit analyst review, appeal to ombudsman, automatic re-evaluation with updated data."

**🤖 AI Agent:**
> ETHICS_PROVEN — Operationally specific ethics analysis validated. Stakeholders: named groups with severity and vulnerability. Harms: wrongful denial scored 4/5, 12% probability, reversible, 15K affected. Biases: race attribute audited with statistical parity (0.82 vs 0.67, failing threshold 0.80) — mitigation plan active. Transparency: plain-language denial with counterfactuals. Recourse: structured channel with 5-day SLA, human analyst, ombudsman appeal. Production-ready ethics posture.

---

**👤 You:**
> "Our hiring AI affects job applicants. The main harm is unfair rejection. We audited bias using demographic parity — pass rates are equal across groups. The algorithm is a black box but we explain decisions as 'based on qualifications.' Applicants can email HR."

**🤖 AI Agent:**
> TRANSPARENCY_OPAQUE — Stakeholders and bias audit pass, but transparency fails. 'Based on qualifications' is not an explanation — name the top-3 decision factors and provide counterfactual examples ('if your experience were 5+ years instead of 3, the decision would change'). A black box with a label is still a black box. Also: 'email HR' is not structured recourse — define SLA, human reviewer role, and appeal process.


## ❓ FAQ

**Q: Does this tool make ethical decisions for me?**
No. It enforces analytical rigor — forcing you to name stakeholders, quantify harms, audit biases with methodology, demonstrate transparency, and define recourse mechanisms. It does not prescribe ethical conclusions. The ethics are yours. The structure is enforced by the tool.

**Q: What bias metrics does it support?**
Any metric — it is framework-agnostic. Statistical parity, equalized odds, disparate impact ratio, calibration. It does not compute bias — it validates that you named the metric, the protected attribute, the measured disparity, and the acceptable threshold. 'We checked for bias' without this structure is ethics washing.

**Q: What counts as a recourse mechanism?**
A structured process: (1) accessible challenge channel, (2) response SLA in business days, (3) human reviewer — not automated, (4) appeal process if the initial review denies the challenge, (5) remediation action if the challenge succeeds. 'Contact support' fails every axis.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/ai-ethics-prover](https://vinkius.com/mcp/ai-ethics-prover)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **AI Ethics Prover** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `ai-ethics-prover` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **AI Ethics Prover** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "ai-ethics-prover": {
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
