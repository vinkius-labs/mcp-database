# Xero MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/xero)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [money-moves](../categories/money-moves.md)

Manage invoices, bank transactions, and financial reports on Xero — the beautiful accounting software for small business.

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


## Available Tools (9)
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


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Xero** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all my unpaid invoices in Xero."

**🤖 AI Agent:**
> I found 5 invoices with outstanding balances: 1. INV-001 ($1,200.00), 2. INV-005 ($450.00), 3. INV-012 ($890.00), and 2 others. Would you like the details for the largest one?

---

**👤 You:**
> "What is our Profit and Loss for March 2026?"

**🤖 AI Agent:**
> PnL Report for March 2026: Total Revenue: $42,500.00, Total Expenses: $28,150.00, Net Profit: $14,350.00. This is a 12% improvement compared to February. Would you like a breakdown by category?

---

**👤 You:**
> "Find the contact ID for 'Global Tech' and show their last 3 payments."

**🤖 AI Agent:**
> Contact 'Global Tech' (ID: 550e8400-e29b...) found. Their last 3 payments were: 1. $1,200.00 (2026-03-15), 2. $1,200.00 (2026-02-15), and 3. $1,200.00 (2026-01-15). All applied to recurring service invoices.


## ❓ FAQ

**Q: Can I retrieve my profit and loss report for a specific period via chat?**
Yes. The `get_profit_and_loss` tool allows your AI agent to retrieve a PnL report by providing a start and end date. This provides an instant summary of your revenue and expenses without manual reporting.

**Q: How do I find out the outstanding amount on a specific invoice?**
You can use the `get_invoice_details` tool. Provide the unique invoice ID, and your agent will return the full metadata, including the original amount, any applied payments, and the current balance due.

**Q: Is it possible to see my bank transactions through the agent?**
Absolutely. Use the `list_bank_transactions` tool to retrieve a list of all transactions recorded in your Xero bank accounts, helping you monitor cash flow directly through your conversation.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/xero](https://vinkius.com/mcp/xero)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Xero** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `xero` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Xero** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "xero": {
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
