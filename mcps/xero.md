# Xero MCP Server

Manage invoices, bank transactions, and financial reports on Xero — the beautiful accounting software for small business.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/xero)

## Overview
**Category:** money-moves
**Tools Count:** 9

## Description
Connect your **Xero** account to any AI agent and manage your business finances through natural conversation.

### What you can do

- **Invoicing Lifecycle** — List all sales and purchase invoices, retrieve comprehensive details including line items and taxes, and track payment statuses
- **Contact Management** — Browse your entire database of customers and suppliers to retrieve contact IDs for accurate invoicing and reporting
- **Bank Reconciliation** — Monitor cash flow by listing bank transactions and applied payments to stay on top of your accounts receivable and payable
- **Financial Reporting** — Retrieve real-time Balance Sheet and Profit and Loss (PnL) reports for any specific date or period through simple commands
- **Chart of Accounts** — Browse your general ledger accounts to verify codes and types (Bank, Expense, Revenue) before recording transactions
- **Organization Audit** — Retrieve legal registration details, base currency, and high-level tenant information for compliance purposes
- **Business Insights** — Quickly find unique invoice, transaction, and contact IDs required for automated accounting workflows

### How it works

1. Subscribe to this server
2. Enter your Xero Access Token and Tenant ID
3. Start monitoring your financial health through Claude, Cursor, or any MCP-compatible client

No more manual navigation through complex accounting dashboards to check if a bill was paid. Your AI agent becomes your financial operations assistant.

### Who is this for?

- **Business Owners** — monitor real-time PnL and check bank transaction history through simple chat commands
- **Accountants & Bookkeepers** — audit invoice details and browse chart of accounts without manual data entry
- **Operations Teams** — verify payment statuses and retrieve customer contact details for billing coordination
- **Finance Analysts** — quickly surface balance sheet data and reconcile payments through conversation


## Available Tools
- **get_organisation_info**: Retrieves details about the Xero organization
- **get_balance_sheet**: Returns assets, liabilities, and equity totals.

Retrieves the balance sheet report for a specific date
- **get_invoice_details**: Retrieves comprehensive details for a specific Xero invoice
- **get_profit_and_loss**: Provide from_date and to_date.

Retrieves the profit and loss (PnL) report for a specific date range
- **list_chart_of_accounts**: Lists all accounts in the Xero chart of accounts
- **list_bank_transactions**: Lists all transactions recorded in bank accounts
- **list_xero_contacts**: Lists all customers and suppliers registered in Xero
- **list_xero_invoices**: Lists all sales and purchase invoices in the Xero organization
- **list_xero_payments**: Lists all payments applied to invoices


## Installation & Usage

To install and use the **Xero** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/xero](https://vinkius.com/mcp/xero)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
