# QuickBooks Online MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/quickbooks-online)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/quickbooks-online-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/quickbooks-online-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [industry-titans](../categories/industry-titans.md)

Connect QuickBooks to AI — query invoices, manage customers, run financial reports, and automate accounting workflows.

## Description
Connect **QuickBooks Online** to any AI agent and manage your entire accounting operation through natural conversation.

### What you can do

- **Invoice Management** — List, view, and create invoices with line items and taxes
- **Customer Management** — Browse customers, view profiles, create new accounts
- **Payment Tracking** — View payment records with amounts and linked invoices
- **Financial Reports** — Run Profit & Loss reports for any date range
- **Company Info** — View company details, fiscal year, and subscription info
- **Custom Queries** — Execute any QuickBooks query language statement


## Available Tools
- **profit_and_loss**: Provide dates in YYYY-MM-DD format.

Run Profit & Loss report
- **list_invoices**: List all invoices
- **get_invoice**: Get invoice details
- **create_invoice**: Provide customer ref and line items as JSON.

Create a new invoice
- **get_customer**: Get customer details
- **query**: Example: SELECT * FROM Invoice WHERE TotalAmt > 100 MAXRESULTS 50

Execute a QuickBooks query
- **create_customer**: Provide DisplayName and optional email/phone as JSON.

Create a new customer
- **list_customers**: List all customers
- **get_payment**: Get payment details
- **get_company_info**: Get company information


## 💬 Prompt Examples

Here are some examples of how you can interact with the **QuickBooks Online** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Show me all unpaid invoices."

**🤖 AI Agent:**
> Found 12 unpaid invoices:

| # | Customer | Amount | Due Date |
|---|----------|--------|----------|
| 1042 | Acme Corp | $3,500 | Apr 15 |
| 1041 | TechStart | $1,200 | Apr 10 |
...

Total outstanding: $18,750

---

**👤 You:**
> "Run the P&L report for Q1 2026."

**🤖 AI Agent:**
> 📊 Profit & Loss — Q1 2026

| Category | Amount |
|----------|--------|
| Revenue | $245,000 |
| COGS | -$89,000 |
| Gross Profit | $156,000 |
| Operating Expenses | -$67,000 |
| Net Income | $89,000 |

---

**👤 You:**
> "Create a customer for John Smith, john@acme.com."

**🤖 AI Agent:**
> ✅ Customer created!

- **Name**: John Smith
- **Email**: john@acme.com
- **ID**: 145


## Installation & Usage

To install and use the **QuickBooks Online** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/quickbooks-online](https://vinkius.com/mcp/quickbooks-online)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
