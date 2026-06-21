# Plaid Enterprise Banking MCP Server

Ultimate Open Banking: balances, transactions, ML fraud logic, payroll, and asset verification.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/plaid-enterprise-banking)

## Overview
**Category:** money-moves
**Tools Count:** 10

## Description
Connect your natural language AI directly to the **Plaid Enterprise** API ecosystem. Unlock Wall-Street grade financial intelligence by turning any compatible agent into a professional underwriter, forensic accountant, and wealth advisor.

### What you can do

- **Core Treasury** — Read available balances, credit limits, and sync L2/L3 enriched itemized transactions (merchants/geolocation).
- **Predictive ML (Signal & Network)** — Evaluate the fraud return risk of ACH wires before they happen via the Plaid Signal AI network.
- **Wealth & Liabilities** — Pull real-time brokerage investment holdings, asset reports, and audit credit card APR and student loan balances.
- **Payroll & Employment** — Parse and extract raw data from W2 payroll stubs and auto-verify active global employers.
- **AML & Watchlist Screening** — Check the account holder against the Interpol list, OFAC sanctions, and Global PEP for identity compliance.
- **Routing & ACH Wiring** — Safely extract account and 9-digit routing numbers securely for banking transfers.

### How it works

1. Subscribe to this server
2. Enter your Plaid Client ID and Secret in the setup
3. Pass your specific `access_token` into the LLM prompts to analyze isolated ledgers instantly

### Security Notice
This MCP instance is strictly hardcoded to **Read-Only**. While it can inspect mass volumes of wealth and ML data, it cannot programmatically execute ACH debits, Wires, or Payments on your behalf, ensuring production-grade safety.


## Available Tools
- **create_link_token**: Required to connect bank accounts.

Create a Plaid Link token for account connection
- **exchange_public_token**: Exchange a public token for an access token
- **get_accounts**: List connected bank accounts
- **get_balances**: Get real-time account balances
- **get_categories**: List transaction categories
- **get_identity**: Get account holder identity
- **get_institution**: Get bank institution details
- **get_item_info**: Get connected item status
- **get_transactions**: Get transaction history
- **search_institutions**: Returns matching institutions with supported products.

Search financial institutions


## Installation & Usage

To install and use the **Plaid Enterprise Banking** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/plaid-enterprise-banking](https://vinkius.com/mcp/plaid-enterprise-banking)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
