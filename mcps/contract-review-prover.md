# Contract Review Prover MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/contract-review-prover)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/contract-review-prover-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/contract-review-prover-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

AI models summarize contracts instead of analyzing them. This tool forces clause-level rigor: score risk per clause (1-5), identify missing legal protections, verify jurisdiction conflicts, quantify financial exposure in currency, and map negotiation leverage. This is structured analysis, not legal advice.

## Description
60% of contract disputes arise from clauses that were 'standard' and unreviewed. AI models produce contract summaries, not analysis — they miss the clause that costs you $2M.

### The 5 Review Failures This Tool Prevents

1. **RISK_UNSCORED** — Clauses listed without risk quantification. Each clause needs a 1-5 risk score with justification.
2. **PROTECTION_MISSING** — Standard protections absent. Checked: limitation of liability, IP ownership, termination, indemnification, confidentiality, data processing, force majeure, audit rights, warranty, dispute resolution.
3. **JURISDICTION_UNVERIFIED** — Governing law and venue not analyzed. Multi-jurisdiction contracts need conflict assessment.
4. **EXPOSURE_UNQUANTIFIED** — Financial risk stated as 'significant' instead of '$X over Y months.' Every risk needs a currency figure.
5. **LEVERAGE_UNMAPPED** — No negotiation strategy. Which clauses are negotiable? What are your alternatives?

**This tool provides structured analytical support. It is NOT legal advice. Always consult qualified legal counsel for binding decisions.**


## Available Tools
- **validate_contract_review**: You must: (1) score EVERY material clause 1-5 for risk with exposure and countermeasure, (2) check 10 standard protections (liability cap, indemnification, IP, confidentiality, termination, force majeure, data protection, non-compete, warranty, dispute resolution) — each PRESENT or MISSING, (3) analyze governing law, dispute venue, arbitration rules, cross-border enforceability, (4) calculate worst-case financial exposure with actual numbers — scenario × probability × impact, (5) map negotiation leverage for BOTH parties — switching costs, alternatives, time pressure, BATNA. If rejected, your review is a summary, not a risk analysis.

Structured reflection tool for rigorous contract analysis with clause-level risk quantification. Catches High-Risk Clauses (uncapped liability, unlimited indemnification without countermeasure), Missing Protections (absent liability cap, no IP clause, no data protection — 10 standard protections unchecked), Jurisdiction Conflicts (governing law mismatches, unfavorable arbitration venue, cross-border enforcement gaps), Financial Exposure ("minimal risk" instead of "$2M+ uncapped consequential damages"), and Leverage Blindness (no BATNA, no switching cost analysis, no counterparty leverage mapped). Call once per contract review. Analytical framework, not legal advice


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Contract Review Prover** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "This SaaS contract looks standard. The vendor says everyone signs it as-is."

**🤖 AI Agent:**
> Verdict: RISK_UNSCORED + LEVERAGE_UNMAPPED. 'Standard' is not a risk assessment. Score each clause 1-5. 'Everyone signs it' is a negotiation tactic, not a fact. Which clauses are genuinely non-negotiable? What are your alternatives? Map your BATNA.

---

**👤 You:**
> "The liability clause caps damages at the fees paid in the last 12 months."

**🤖 AI Agent:**
> Verdict: EXPOSURE_UNQUANTIFIED. What ARE the fees in the last 12 months? If annual contract is $50K but a breach causes $2M in damages, the cap exposes you to $1.95M uncovered risk. Quantify: 'Annual fees: $50K. Worst-case exposure: $2M. Gap: $1.95M. Risk score: 5/5.'

---

**👤 You:**
> "The contract is governed by the laws of Delaware but our company is in Germany."

**🤖 AI Agent:**
> Verdict: JURISDICTION_UNVERIFIED. Delaware vs. Germany creates a jurisdiction conflict. Key questions: (1) Is the venue clause exclusive or non-exclusive? (2) Does GDPR override Delaware law for data processing? (3) What are enforcement costs of litigating in Delaware from Germany? (4) Are arbitration clauses available as alternative?


## Installation & Usage

To install and use the **Contract Review Prover** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/contract-review-prover](https://vinkius.com/mcp/contract-review-prover)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
