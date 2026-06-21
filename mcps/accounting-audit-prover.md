# Accounting & Audit Prover MCP Server

Forces AI agents to validate accounting arguments against explicit US standards (FASB ASC, PCAOB), demanding real materiality thresholds, Risk of Material Misstatement (ROMM) assessments, and grounded evidence instead of vague 'GAAP' appeals.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/accounting-audit-prover)

## Overview
**Category:** productivity
**Tools Count:** 1

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


## Installation & Usage

To install and use the **Accounting & Audit Prover** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/accounting-audit-prover](https://vinkius.com/mcp/accounting-audit-prover)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
