# LawPay MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/lawpay)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/lawpay-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/lawpay-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [money-moves](../categories/money-moves.md)

Accept legal payments online with trust and operating account compliance that meets bar association requirements for law firms.

## Description
Connect your **LawPay** account to any AI agent and manage legal payments through natural conversation.

### What you can do

- **Transaction Management** — Browse payments, refunds, and charges with status tracking
- **Invoice Tracking** — List invoices with amounts, due dates, and payment status
- **Trust Accounts** — Monitor trust (IOLTA) account balances and transactions
- **Payment Processing** — Create charges and process payments
- **Financial Reports** — Access revenue summaries, payment trends, and aging reports
- **Client Billing** — Track client payment history and outstanding balances

### How it works

1. Subscribe to this server
2. Enter your LawPay Secret Key and Merchant ID
3. Start managing payments from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Law Firms** — manage client payments and trust accounts
- **Legal Billing** — track invoices and outstanding balances
- **Finance Teams** — access payment reports and reconciliation


## Available Tools
- **create_invoice**: Create a new invoice
- **create_refund**: Refund a transaction
- **get_account_info**: Get merchant profile info
- **get_account**: Get account details
- **get_payment_method**: Get payment method details
- **get_account_stats**: Get payment statistics
- **get_transaction**: Get transaction details
- **list_accounts**: ).

List merchant accounts
- **list_invoices**: List payment invoices
- **list_payment_methods**: List saved payment methods
- **list_settlements**: List bank settlements
- **list_transactions**: List all payment transactions


## 💬 Prompt Examples

Here are some examples of how you can interact with the **LawPay** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Show payment summary for this month and trust account balances."

**🤖 AI Agent:**
> This month: 45 payments received, $128,400 total. Credit card: 38 ($98,200). ACH/eCheck: 7 ($30,200). Refunds: 2 ($1,500). Average payment: $2,853. Trust accounts: Operating ($45,200), IOLTA Trust ($234,500, 12 client matters). Largest trust balance: Matter #1045 — Smith v. Jones ($45,000).

---

**👤 You:**
> "Show outstanding invoices and the aging report."

**🤖 AI Agent:**
> Outstanding: 18 invoices, $67,800 total. Current (0-30 days): 10 invoices, $38,200. 31-60 days: 5, $18,400. 61-90 days: 2, $8,200. 90+ days: 1, $3,000 ⚠️ (Matter #892 — Johnson Estate). Top outstanding: 'Corporate Merger — TechCo' ($12,500, 15 days). Collection rate: 94%.

---

**👤 You:**
> "List recent transactions for Matter #1045 and create a charge."

**🤖 AI Agent:**
> Matter #1045 — Smith v. Jones. Trust balance: $45,000. Transactions (30 days): 3. Deposit: $20,000 (retainer, Apr 5). Disbursement: -$5,000 (filing fees, Apr 12). Disbursement: -$2,500 (expert witness, Apr 20). Charge created! $3,500 — 'Legal services, April billing'. Method: Credit card. Status: Approved ✅.


## Installation & Usage

To install and use the **LawPay** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/lawpay](https://vinkius.com/mcp/lawpay)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
