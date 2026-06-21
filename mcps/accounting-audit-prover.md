# Accounting & Audit Prover MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/accounting-audit-prover)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Forces AI agents to validate accounting arguments against explicit US standards (FASB ASC, PCAOB), demanding real materiality thresholds, Risk of Material Misstatement (ROMM) assessments, and grounded evidence instead of vague 'GAAP' appeals.

## Description
AI agents generate accounting memos and audit plans that look professional but fail fundamentally on regulatory compliance. They rely on vague appeals to 'GAAP' rather than citing specific Codification (ASC) sections, and they propose audit procedures without first quantifying Materiality or the Risk of Material Misstatement (ROMM). In auditing, 'looks correct' is not an opinion.

### The Problem It Solves

AI-generated accounting/audit reasoning fails for five specific reasons:

- **Standard blindness** — Vague references to "GAAP" without citing specific FASB ASC or PCAOB standards.
- **Unquantified materiality** — Analyzing misstatements without establishing a quantitative materiality threshold (e.g., 5% of Pre-Tax Income).
- **Ignored ROMM** — Proposing audit procedures without assessing the Risk of Material Misstatement (Inherent Risk x Control Risk).
- **Vague procedures** — Recommending generic 'testing' instead of specific substantive procedures (vouching, tracing, confirmation).
- **Ungrounded evidence** — Relying on assumptions rather than requiring sufficient, appropriate audit evidence.

### How It Works

Accounting & Audit Prover uses 5 Decision Pivots grounded in US accounting practice:

1. **standardComplianceValidated** — Is the conclusion explicitly validated against a stated, specific US standard (FASB ASC, PCAOB)?
2. **materialityQuantified** — Is materiality explicitly quantified and applied to the issue?
3. **rommAssessed** — Is the Risk of Material Misstatement (ROMM) explicitly assessed before designing procedures?
4. **proceduresSpecified** — Are specific substantive audit procedures or accounting treatments detailed?
5. **evidenceGrounded** — Is the conclusion grounded in specific, sufficient, and appropriate evidence requirements?


## Available Tools
- **validate_accounting_audit**: You must: (1) define the AUDIT SCOPE — specific financial statement area, account balance, or transaction class. "Revenue" is too broad — "Revenue recognition for multi-year SaaS contracts under ASC 606" is a scope, (2) cite the APPLICABLE STANDARD — exact FASB ASC topic or PCAOB auditing standard with reference number. "GAAP principles" and "standard practices" are not citations — "ASC 606-10-25" and "PCAOB AS 2315" are, (3) quantify MATERIALITY — specific dollar thresholds or percentage benchmarks. "5% of pre-tax income = $2.3M overall materiality, $1.7M performance materiality" — not "significant amount", (4) assess ROMM — identify what could go wrong (inherent risk), evaluate control design and operating effectiveness (control risk), and determine the nature, timing, and extent of substantive procedures that respond to the assessed risks, (5) detail PROCEDURES — name specific substantive or analytical tests: vouching to third-party invoices, recalculating depreciation schedules, confirming balances with banks, performing cut-off testing, analytical procedures comparing current to prior period with expectation and threshold, (6) specify EVIDENCE — the exact documentary proof relied upon: bank confirmations, third-party invoices, signed contracts, board minutes, external legal counsel letters, management representations, (7) state the AUDIT CONCLUSION — unmodified/qualified/adverse opinion basis, or specific accounting treatment conclusion with ASC reference. If the tool rejects, your accounting/audit reasoning has a structural deficiency. Fix it before advising.

Structured reflection tool for US accounting and audit reasoning (GAAP/FASB ASC/PCAOB/AICPA). Forces the agent to construct rigorous, standard-grounded financial analysis before concluding. Catches Standard Blindness (vague "GAAP rules" without citing ASC/PCAOB codification), Unquantified Materiality (no numerical thresholds — "significant" is not a number), Ignored ROMM (proposing procedures without assessing Risk of Material Misstatement or internal controls), Vague Procedures ("we will audit" without naming substantive or analytical tests), and Ungrounded Evidence (concluding without citing specific documentary proof). Call once per accounting issue or audit engagement area


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Accounting & Audit Prover** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "A client recognized $50M in revenue before delivering the software. According to GAAP, this is wrong. They should wait until delivery. Validate this using the prover."

**🤖 AI Agent:**
> Verdict: STANDARD_COMPLIANCE_BLIND. 'According to GAAP' is not a citation. Cite FASB ASC 606, identify the specific performance obligation, quantify materiality, and specify the audit evidence required to verify delivery.

---

**👤 You:**
> "Analyze the revenue recognition of a $5M software contract under ASC 606. Validate the conclusion with the prover, quantifying materiality at $100k, assessing ROMM as High due to complex performance obligations, and detailing specific vouching procedures."

**🤖 AI Agent:**
> Verdict: REASONING_PROVEN. Standard compliance validated (ASC 606), materiality quantified ($100k), ROMM explicitly assessed (High), substantive procedures detailed, and grounded in evidence.

---

**👤 You:**
> "Under PCAOB AS 2315, we will audit the inventory balance. The materiality is $500k. We will perform tests of details on the warehouse counts. Validate this plan."

**🤖 AI Agent:**
> Verdict: ROMM_IGNORED. You cited the standard, set materiality, and proposed procedures, but completely skipped the Risk of Material Misstatement assessment. Is inherent risk high? Control risk low? Assess ROMM before testing.


## ❓ FAQ

**Q: Can this MCP perform financial reconciliations?**
No. This is a strictly stateless reasoning gatekeeper. It does not perform mathematical reconciliations, access ERP systems, or review ledgers. It validates the logical structure of the AI's accounting/audit reasoning based on the inputs provided.

**Q: Why did the Prover reject my accounting memo with STANDARD_COMPLIANCE_BLIND?**
Because the reasoning relied on vague appeals like 'according to GAAP' or 'standard accounting practice'. To pass the Prover, you must cite specific US standards (e.g., FASB ASC 606, PCAOB AS 2110).

**Q: What does ROMM mean and why is it required?**
ROMM stands for Risk of Material Misstatement. In auditing, you cannot propose substantive procedures without first assessing the inherent and control risks that could lead to a material error. The Prover forces this assessment.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/accounting-audit-prover](https://vinkius.com/mcp/accounting-audit-prover)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Accounting & Audit Prover** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `accounting-audit-prover` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Accounting & Audit Prover** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "accounting-audit-prover": {
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
