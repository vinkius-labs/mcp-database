# Financial Audit Prover MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/financial-audit-prover)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Forces AI to ground every financial conclusion in ASC codification, trace numbers to source documents, reconcile statements, and identify required disclosures instead of generating plausible numbers without audit trails.

## Description
AI agents generate financial analysis that looks numerically sound but violates fundamental accounting principles. They apply IFRS rules to US GAAP entities. They produce figures without audit trails. They skip materiality assessment entirely. And they reference 'required disclosures' without naming a single ASC topic or SEC regulation.

### The Problem It Solves

AI-generated financial reasoning fails for five specific reasons:

- **GAAP violation** — Applies the wrong accounting standard. Mixes IFRS concepts (revaluation model, IAS references) with US GAAP entities. Cites 'GAAP requires' without naming the specific ASC topic.
- **Broken audit trail** — Conclusions based on 'financial data' or 'per the records' without tracing to source documents. No GL account numbers, no invoice references, no confirmation results.
- **Cross-check failure** — Numbers between financial statements don't reconcile. Net income doesn't tie to equity rollforward. Cash flow statement doesn't reconcile to balance sheet cash.
- **Materiality blindness** — Ignores SAB 99's dual requirement for quantitative thresholds AND qualitative evaluation. 'Immaterial' without a number is not an assessment.
- **Missing disclosure** — References 'appropriate disclosures' without identifying which ASC topic requires the footnote, which Reg S-K item requires the narrative, or which SOX section requires certification.

### How It Works

Financial Audit Prover uses 5 Decision Pivots grounded in US accounting standards:

1. **gaapCompliant** — Correct ASC topic applied? Recognition, measurement, and presentation criteria met? No IFRS leakage?
2. **auditTrailComplete** — Every number traces to source documents? GL entries, invoices, confirmations, bank statements? Per PCAOB AS 2810?
3. **crossCheckPassed** — Balance sheet equation balances? Income ties to equity? Cash flow reconciles to cash change? Account rollforwards prove out?
4. **materialityAssessed** — Quantitative threshold stated (5% pre-tax per SAB 99)? Qualitative factors evaluated (trend masking, covenant impact, compensation effect)?
5. **disclosureComplete** — Specific ASC footnote topics identified? Reg S-K items named? Reg S-X rules cited? SOX certifications addressed?

The engine catches IFRS leakage by detecting international standard terminology in US GAAP analysis. It validates that audit trails reference specific documents — not 'based on financial data.' It requires both quantitative AND qualitative materiality per SAB 99.

### US Financial Framework Coverage

- **FASB ASC Codification** — The authoritative source of US GAAP
- **SEC Regulation S-X** — Financial statement form and content requirements
- **SEC Regulation S-K** — Non-financial disclosure requirements (MD&A, risk factors)
- **PCAOB Auditing Standards** — AS 2201 (internal controls), AS 2401 (fraud), AS 2810 (evidence)
- **Sarbanes-Oxley Act** — Section 302 (CEO/CFO certification), Section 404 (internal controls)
- **SAB 99** — Quantitative and qualitative materiality assessment
- **IRS Internal Revenue Code** — Title 26 tax compliance where applicable


## Available Tools (1)
- **validate_financial_audit**: Financial reporting is not opinion — it is codified standards, traceable evidence, and mathematical reconciliation. You must: (1) cite the specific US GAAP basis — ASC topic-subtopic-section-paragraph. "GAAP requires" is not a citation. "ASC 606-10-25-27 point-in-time recognition criteria" is, (2) provide an AUDIT TRAIL — trace every material number to source documents. GL account, journal entry reference, invoice/contract/confirmation reference, reconciliation to trial balance, financial statement line item, (3) demonstrate CROSS-CHECKS — the financial statements must reconcile internally. Total assets = total liabilities + equity. Net income flows to retained earnings. Cash flow statement reconciles to cash change. Show actual numbers, (4) assess MATERIALITY — quantitative threshold (5% pre-tax income per SAB 99 benchmark) AND qualitative factors (trend masking, covenant impact, compensation effect, unlawful activity concealment). Both dimensions are mandatory, (5) identify all required DISCLOSURES — specific ASC footnote topics, Reg S-K narrative items, Reg S-X presentation rules, SOX certifications. If rejected, your financial analysis has a structural deficiency.

Structured reflection tool for US financial reasoning — forces audit-grade analysis grounded in US GAAP (FASB ASC codification), PCAOB standards, SEC regulations, and SOX requirements. Catches GAAP Violation (applying revenue recognition without citing ASC 606-10-25-27 vs 25-31 — "per GAAP" is not a reference. The specific ASC paragraph that governs your treatment is the reference. IFRS is not US GAAP), Trail Broken ("per the records" without tracing to source documents — GL entry, invoice number, bank confirmation, contract date. Per PCAOB AS 2810, every material assertion requires sufficient appropriate audit evidence), Crosscheck Failed (financial statements that do not reconcile internally — assets ≠ liabilities + equity, net income does not flow to retained earnings, cash flow does not reconcile to cash balance change. If the B/S does not balance, nothing is reliable), Materiality Ignored ("immaterial" without quantitative threshold per SAB 99 (5% pre-tax income is the benchmark, not a rule) AND qualitative assessment — does it mask a trend? Affect covenant compliance? Involve management compensation?), and Disclosure Missing (accounting treatment without identifying required footnotes — ASC 235 policies, ASC 275 risks, ASC 450 contingencies, ASC 855 subsequent events, Reg S-K Item 303 MD&A, SOX 302/404 certifications). Call once per financial analysis or audit issue


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Financial Audit Prover** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "The company recognized $5M in revenue from a multi-year software licensing deal. Is this correct under GAAP?"

**🤖 AI Agent:**
> Verdict: GAAP_VIOLATED. 'Under GAAP' is not a citation. Revenue recognition for software requires ASC 606 five-step analysis: (1) identify the contract (ASC 606-10-25-1), (2) identify performance obligations (distinct software license vs. ongoing services? — ASC 606-10-25-19), (3) determine transaction price ($5M — is there variable consideration?), (4) allocate to performance obligations (standalone selling prices), (5) recognize when satisfied (point-in-time for license under ASC 606-10-25-27, or over-time for SaaS under ASC 606-10-25-31?). Which step supports full upfront recognition?

---

**👤 You:**
> "Issue: Whether $2.8M goodwill impairment is required. GAAP: ASC 350-20-35-1, qualitative election per 35-3A. Five factors assessed — stable industry, no customer loss, share price above book, no regulatory changes, CFO replaced in 60 days. Conclusion: fair value exceeds carrying. Audit: GL 1800, $2.8M from 2022 DataVault acquisition (WP-805-22). Cross-check: rollforward reconciles. Materiality: 7.2% of $38.9M pre-tax. Disclosures: ASC 350-20-50-1/50-2, Reg S-K Item 303."

**🤖 AI Agent:**
> Verdict: AUDIT_PROVEN. GAAP compliant — ASC 350-20-35-1 through 35-19 correctly cited with qualitative election per 35-3A. Audit trail complete — GL 1800 traced to 2022 acquisition, work paper WP-805-22 referenced. Cross-check passed — intangible rollforward reconciles ($2.8M beginning = $2.8M ending). Materiality assessed — both quantitative (7.2% > 5% threshold) and qualitative (strategic acquisition signaling). Disclosures identified — ASC 350-20-50-1/50-2 footnotes, Reg S-K Item 303 MD&A discussion. This analysis meets audit memo standard.

---

**👤 You:**
> "The company has approximately $1.2M in accounts receivable. Based on financial data, this seems reasonable. Required disclosures have been made. The amount is immaterial."

**🤖 AI Agent:**
> Multiple rejections. (1) TRAIL_BROKEN — 'approximately $1.2M' is hedged language suggesting fabricated precision. What is the exact GL balance? Which invoices? What aging bucket? What confirmation results? (2) 'Based on financial data' is not an audit trail — name the source documents. (3) MATERIALITY_IGNORED — 'immaterial' without a threshold is not an assessment. What is 5% of pre-tax income? How does $1.2M compare? (4) DISCLOSURE_MISSING — 'required disclosures have been made' names zero specific ASC topics. ASC 310-10-50 (receivables), ASC 326-20 (CECL allowance), ASC 820-10-50 (fair value hierarchy if measured at FV)? Which disclosures specifically?


## ❓ FAQ

**Q: Does it perform calculations or generate financial statements?**
No. Financial Audit Prover generates zero content and performs zero calculations. It validates the REASONING behind financial conclusions — whether the correct GAAP standard is applied, whether numbers trace to source documents, whether statements reconcile, whether materiality is properly assessed, and whether required disclosures are identified. The agent does the financial analysis; the tool proves whether that analysis meets audit-grade standards.

**Q: Does it support IFRS or only US GAAP?**
US GAAP only. The engine actively detects IFRS terminology leakage (IAS references, 'revaluation model', 'true and fair view') and rejects it. US GAAP and IFRS differ materially on inventory (LIFO), development costs, leases, and revenue recognition implementation. Mixing frameworks produces unreliable analysis. If you need IFRS validation, a separate tool would be required — this one validates ASC codification exclusively.

**Q: What types of entities does it cover?**
Any US entity reporting under GAAP: SEC registrants (10-K/10-Q filers), private companies (including private company alternatives under ASC), nonprofits (ASC 958), and tax-reporting entities (IRC Title 26). The tool adapts — SEC registrants trigger Reg S-K and SOX validation; private companies focus on ASC compliance and footnote completeness; nonprofits require net asset classification checks. Specify the entity type in the 'regulatoryContext' field.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/financial-audit-prover](https://vinkius.com/mcp/financial-audit-prover)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Financial Audit Prover** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `financial-audit-prover` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Financial Audit Prover** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "financial-audit-prover": {
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
