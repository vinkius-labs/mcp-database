# Financial Audit Prover MCP Server

Forces AI to ground every financial conclusion in ASC codification, trace numbers to source documents, reconcile statements, and identify required disclosures instead of generating plausible numbers without audit trails.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/financial-audit-prover)

## Overview
**Category:** productivity
**Tools Count:** 1

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


## Available Tools
- **validate_financial_audit**: Financial reporting is not opinion — it is codified standards, traceable evidence, and mathematical reconciliation. You must: (1) cite the specific US GAAP basis — ASC topic-subtopic-section-paragraph. "GAAP requires" is not a citation. "ASC 606-10-25-27 point-in-time recognition criteria" is, (2) provide an AUDIT TRAIL — trace every material number to source documents. GL account, journal entry reference, invoice/contract/confirmation reference, reconciliation to trial balance, financial statement line item, (3) demonstrate CROSS-CHECKS — the financial statements must reconcile internally. Total assets = total liabilities + equity. Net income flows to retained earnings. Cash flow statement reconciles to cash change. Show actual numbers, (4) assess MATERIALITY — quantitative threshold (5% pre-tax income per SAB 99 benchmark) AND qualitative factors (trend masking, covenant impact, compensation effect, unlawful activity concealment). Both dimensions are mandatory, (5) identify all required DISCLOSURES — specific ASC footnote topics, Reg S-K narrative items, Reg S-X presentation rules, SOX certifications. If rejected, your financial analysis has a structural deficiency.

Structured reflection tool for US financial reasoning — forces audit-grade analysis grounded in US GAAP (FASB ASC codification), PCAOB standards, SEC regulations, and SOX requirements. Catches GAAP Violation (applying revenue recognition without citing ASC 606-10-25-27 vs 25-31 — "per GAAP" is not a reference. The specific ASC paragraph that governs your treatment is the reference. IFRS is not US GAAP), Trail Broken ("per the records" without tracing to source documents — GL entry, invoice number, bank confirmation, contract date. Per PCAOB AS 2810, every material assertion requires sufficient appropriate audit evidence), Crosscheck Failed (financial statements that do not reconcile internally — assets ≠ liabilities + equity, net income does not flow to retained earnings, cash flow does not reconcile to cash balance change. If the B/S does not balance, nothing is reliable), Materiality Ignored ("immaterial" without quantitative threshold per SAB 99 (5% pre-tax income is the benchmark, not a rule) AND qualitative assessment — does it mask a trend? Affect covenant compliance? Involve management compensation?), and Disclosure Missing (accounting treatment without identifying required footnotes — ASC 235 policies, ASC 275 risks, ASC 450 contingencies, ASC 855 subsequent events, Reg S-K Item 303 MD&A, SOX 302/404 certifications). Call once per financial analysis or audit issue


## Installation & Usage

To install and use the **Financial Audit Prover** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/financial-audit-prover](https://vinkius.com/mcp/financial-audit-prover)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
