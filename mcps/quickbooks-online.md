# QuickBooks Online MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/quickbooks-online)
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


## Available Tools (10)
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


## ❓ FAQ

**Q: Can I run Profit & Loss reports?**
Yes! Use the `profit_and_loss` tool with start and end dates in YYYY-MM-DD format.

**Q: How do I create an invoice?**
Use `create_invoice` with a JSON payload containing the CustomerRef and Line items.

**Q: Can I run custom queries?**
Yes! The `query` tool accepts any QuickBooks query. Example: SELECT * FROM Invoice WHERE TotalAmt > 500.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/quickbooks-online](https://vinkius.com/mcp/quickbooks-online)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **QuickBooks Online** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `quickbooks-online` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **QuickBooks Online** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "quickbooks-online": {
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
