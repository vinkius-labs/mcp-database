# Compliance Governance Prover MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/compliance-governance-prover)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [ai-ml](../categories/ai-ml.md)

An AI said 'comply with GDPR' without naming a single article. It said 'we have controls' without mapping any to a regulation. It said 'low risk' without measuring severity or fine exposure. The auditor found 4 critical gaps. That is not compliance — that is compliance theater. This tool forces five audit-grade axes: specific regulation naming, control mapping, evidence documentation, gap quantification, and named accountability.

## Description
## The Problem

Ask an LLM to analyze compliance. It will say 'comply with GDPR' without citing Article 6(1)(a) or Article 32. It will say 'we have security controls' without mapping any control to a specific regulation. It will say 'low risk' without measuring severity, fine exposure, or remediation cost. And it will assign ownership to 'the team.'

Every LLM commits five compliance reasoning failures:
1. **Unnamed Regulations** — 'industry standards' and 'best practices' are not regulations. Name the law, jurisdiction, and article number.
2. **Unmapped Controls** — 'we have controls' without linking each control to the regulation it satisfies.
3. **Undocumented Evidence** — claims without audit artifacts, test dates, or coverage percentages.
4. **Unquantified Gaps** — 'low risk' and 'minor issue' without severity scoring, fine exposure, or remediation cost.
5. **Unassigned Accountability** — controls owned by 'the team' instead of a named person with review cadence.

## How It Works

The Compliance Governance Prover forces the LLM to fill 5 reflection fields and commit to 5 Decision Pivots before concluding any compliance analysis is audit-ready.

### The 5 Compliance Axes

| Axis | Pivot | Rule |
|---|---|---|
| **Regulations** | Identified | Specific law, jurisdiction, article/section number with applicability rationale. |
| **Controls** | Mapped | Each regulation paired with a named technical or administrative control. |
| **Evidence** | Documented | Audit artifacts with test dates, coverage, and retention policy. |
| **Gaps** | Quantified | Severity (1-5), fine exposure, remediation cost, timeline. |
| **Accountability** | Assigned | Named owner, review cadence, escalation path. |

### The Verdict Matrix

```
Axis 1 fails → REGULATIONS_UNNAMED
Axis 2 fails → CONTROLS_UNMAPPED
Axis 3 fails → EVIDENCE_MISSING
Axis 4 fails → GAPS_UNQUANTIFIED
Axis 5 fails → ACCOUNTABILITY_ABSENT
All pass     → COMPLIANCE_PROVEN
```

## Why It Works

Tool calls are obligations. The LLM cannot skip regulation naming or ignore gap quantification. It must cite specific articles, map controls, document evidence, score severity with exposure, and name owners. Every rejection names the exact compliance axis that failed.

**Disclaimer:** This is analytical support — it forces structured thinking about compliance. It does not certify compliance or replace qualified legal, regulatory, or compliance professionals.


## Available Tools
- **validate_compliance_governance**: Think like an external auditor preparing a SOC 2 report or GDPR readiness assessment — every claim must be traceable to a specific regulation, a specific control, a specific artifact. You must: (1) inventory REGULATIONS — name each applicable law with jurisdiction (EU/US/state), specific article or section number, and applicability rationale (WHY does this regulation apply to this system/data/process?). "Industry standards" and "applicable regulations" are not regulations. GDPR Art. 6(1)(a) Consent is a regulation. SOC 2 Type II CC6.1 Logical Access is a regulation, (2) map CONTROLS — each regulation must pair with a specific technical or procedural control. Not "we have security measures" — name the control, classify it (technical/procedural/administrative), describe the implementation, and define the verification method (how do you PROVE it works?), (3) document EVIDENCE — each control must have named audit artifacts: reports, logs, test results, certifications with dates, coverage periods, and assessor identity. "We can demonstrate compliance" is not evidence — "SOC 2 Type II report, Ernst & Young, coverage Jan-Dec 2023, 0 exceptions" is evidence, (4) quantify GAPS — each compliance gap must have: severity (1-5), fine exposure in currency with calculation basis (e.g., "up to €10M or 2% annual turnover per GDPR Art. 83"), remediation cost (engineering hours + external costs), timeline to remediation, and residual risk after remediation. "Minor gap" and "acceptable risk" are not quantification, (5) assign ACCOUNTABILITY — each control must have a named owner (person, not team), review cadence (monthly, quarterly), escalation path (who gets notified if the control fails), and last review date. "Shared responsibility" means nobody is accountable. "The compliance team handles it" is theater. If rejected, your compliance assessment has a governance flaw. Fix it before certifying.

Structured reflection tool for audit-grade compliance governance analysis. Forces the agent to inventory applicable regulations by jurisdiction and article, map each regulation to specific technical/procedural controls with implementation details, document audit-ready evidence artifacts with dates and coverage, quantify compliance gaps with severity and financial exposure, and assign named accountability with review cadence and escalation paths. Catches Unnamed Regulations (citing "industry standards" or "applicable regulations" without specific articles — GDPR Art. 17, SOC 2 CC6.1, PCI DSS Req. 3.4 are regulations, "best practices" is not), Unmapped Controls (claiming "we have security measures" without linking each control to the regulation it satisfies), Undocumented Evidence (asserting "we can demonstrate compliance" without naming audit artifacts, dates, and coverage periods), Unquantified Gaps (describing gaps as "minor risk" without severity scoring, fine exposure in currency, and remediation cost), and Unassigned Accountability (controls owned by "the team" or "shared responsibility" — no named person, no review date, no escalation path). Call once per compliance assessment. Analytical support, not legal advice


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Compliance Governance Prover** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Our SaaS platform complies with industry standards and has security measures in place. We follow best practices for data protection. The team reviews compliance periodically."

**🤖 AI Agent:**
> REGULATIONS_UNNAMED — 'Industry standards' is not a regulation. 'Best practices' is not a law. Name the specific regulation: GDPR Article 6(1)(a) — lawful basis for processing. SOC 2 CC6.1 — logical access controls. PCI DSS Requirement 3.4 — render PAN unreadable. For each: jurisdiction, applicability rationale, and the specific articles that apply to your data processing operations.

---

**👤 You:**
> "GDPR Art. 6(1)(a) — consent-based processing, EU jurisdiction. Control: ConsentManager SDK with granular opt-in, audit log. Evidence: penetration test (2025-03-15), 94% coverage, report #PT-2025-Q1. Gap: Art. 17 erasure SLA — severity 3, €2M exposure, €45K remediation, 6-week timeline. Owner: Sarah Chen (DPO), quarterly review, escalation to CISO within 48h."

**🤖 AI Agent:**
> COMPLIANCE_PROVEN — Audit-grade compliance analysis validated. Regulations: GDPR Art. 6(1)(a) with jurisdiction and basis. Controls: ConsentManager SDK with granular consent and audit logging. Evidence: penetration test dated 2025-03-15, 94% coverage, report referenced. Gaps: Art. 17 erasure scored severity 3, €2M exposure, €45K remediation, 6-week timeline. Accountability: Sarah Chen (DPO), quarterly review, 48h CISO escalation. Production-ready compliance posture.

---

**👤 You:**
> "We comply with GDPR Article 32 — security of processing. Controls: encryption at rest (AES-256) and TLS 1.3 in transit. Last audit: Q2 2024. Risk level: low. Owner: Engineering team, reviews annually."

**🤖 AI Agent:**
> GAPS_UNQUANTIFIED — Regulation and controls pass, but gap analysis fails. 'Low risk' is not a measurement — assign severity (1-5), calculate fine exposure (Art. 83: up to €20M or 4% global turnover), estimate remediation cost, and set a timeline. Also: 'engineering team' is not an owner — name a person. And Q2 2024 audit is over a year old — what is the next scheduled assessment?


## ❓ FAQ

**Q: Does this replace legal advice?**
No. This is analytical support — it forces structured thinking about compliance. It does not certify compliance or replace qualified legal, regulatory, or compliance professionals. It catches structural gaps in reasoning, not legal deficiencies in controls.

**Q: What does it catch that a prompt doesn't?**
A prompt says 'be thorough about compliance.' The LLM says 'comply with GDPR and implement security controls' — and the prompt is satisfied. This tool rejects that because no article number was cited, no control was mapped, and no gap was scored. Tool calls are obligations — the LLM cannot skip the structural checks.

**Q: Which regulations does it support?**
Any regulation — it is framework-agnostic. GDPR, SOC 2, PCI DSS, HIPAA, ISO 27001, EU AI Act, CCPA, NIST. It does not validate whether your controls satisfy a regulation — it validates whether your analysis is structurally complete. The depth of your reasoning is what it enforces.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/compliance-governance-prover](https://vinkius.com/mcp/compliance-governance-prover)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Compliance Governance Prover** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `compliance-governance-prover` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Compliance Governance Prover** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "compliance-governance-prover": {
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
