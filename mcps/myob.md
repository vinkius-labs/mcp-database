# MYOB MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/myob)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/myob-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/myob-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [erp-operations](../categories/erp-operations.md)

Automate accounting and sales management via MYOB — list GL accounts, journal transactions, invoices, and customer payments directly from any AI agent.

## Description
Connect your **MYOB** business account to any AI agent and take full control of your accounting and sales workflows through natural conversation.

### What you can do

- **General Ledger** — List accounts, journal transactions, tax codes, and categories for any company file.
- **Sales & Invoicing** — Query sale invoices, customer payments, and sale orders to track revenue in real-time.
- **Job Tracking** — Retrieve and manage jobs to monitor project-specific financial performance.
- **Data Filtering** — Use OData expressions to filter, skip, and order financial records for precise reporting.
- **Company File Management** — Access specific company files using their unique URIs to maintain multi-entity oversight.

### How it works

1. Subscribe to this server
2. Enter your MYOB API Key, Access Token, and Company File Token
3. Start managing your finances from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Accountants & Bookkeepers** — quickly audit ledgers and tax codes without manual exports
- **Sales Managers** — track invoice statuses and customer payments directly from your workflow
- **Business Owners** — get instant snapshots of financial health and job progress through simple queries


## Available Tools
- **list_banking_bank_accounts**: List Banking Bank Accounts
- **list_banking_receive_money_txns**: List Banking Receive Money Transactions
- **list_banking_spend_money_txns**: List Banking Spend Money Transactions
- **list_banking_transfer_money_txns**: List Banking Transfer Money Transactions
- **list_gl_accounts**: List General Ledger Accounts
- **list_gl_categories**: List General Ledger Categories
- **list_gl_jobs**: List General Ledger Jobs
- **list_gl_journal_transactions**: List General Ledger Journal Transactions
- **list_gl_tax_codes**: List General Ledger Tax Codes
- **list_inventory_adjustments**: List Inventory Adjustments
- **list_inventory_item_price_matrices**: List Inventory Item Price Matrices
- **list_inventory_items**: List Inventory Items
- **list_inventory_locations**: List Inventory Locations
- **list_payroll_categories**: List Payroll Categories
- **list_payroll_superannuation_funds**: List Payroll Superannuation Funds
- **list_payroll_timesheets**: List Payroll Timesheets
- **list_purchase_bills**: List Purchase Bills
- **list_purchase_orders**: List Purchase Orders
- **list_purchase_supplier_payments**: List Purchase Supplier Payments
- **list_sale_customer_payments**: List Sale Customer Payments
- **list_sale_invoices**: List Sale Invoices
- **list_sale_orders**: List Sale Orders
- **list_sale_quotes**: List Sale Quotes


## 💬 Prompt Examples

Here are some examples of how you can interact with the **MYOB** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all general ledger accounts for the company file at URI 'https://ar1.api.myob.com/accountright/guid'."

**🤖 AI Agent:**
> I've retrieved the accounts for that company file. You have 45 active accounts, including 'General Checking' (Code: 1-1100) and 'Trade Debtors' (Code: 1-1200). Would you like to see the full list or filter by a specific account type?

---

**👤 You:**
> "Show me the sale invoices for the company file 'https://ar1.api.myob.com/accountright/guid' with a limit of 5."

**🤖 AI Agent:**
> Fetching the latest invoices... I found 5 recent invoices. The most recent is Invoice #INV-001 for $1,200.00, currently marked as 'Open'. Would you like details on the customer payments associated with these?

---

**👤 You:**
> "Retrieve the customer payments from the company file URI 'https://ar1.api.myob.com/accountright/guid'."

**🤖 AI Agent:**
> Querying customer payments... I've listed the recent transactions. There was a significant payment of $5,000.00 received yesterday from 'Global Industries'. Should I check which invoices this payment cleared?


## Installation & Usage

To install and use the **MYOB** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/myob](https://vinkius.com/mcp/myob)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
