# FreeAgent MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/freeagent)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Manage accounting, track invoices, and oversee bank transactions via AI agents with FreeAgent.

## Description
Connect your **FreeAgent** account to any AI agent to automate your accounting and financial oversight through the Model Context Protocol (MCP). FreeAgent is an award-winning accounting software designed for freelancers and small businesses. This MCP server enables you to manage your invoices, track bank transactions, and retrieve real-time Profit and Loss summaries directly through natural conversation.

### Key Features

- **Invoice Management** — List all sales invoices, fetch detailed metadata, and monitor overdue payments instantly.
- **Contact Oversight** — Access your database of customers and suppliers to maintain full context of your business relationships.
- **Banking Integration** — List configured bank accounts and retrieve transaction history for reconciliation and auditing.
- **Expense & Bill Tracking** — Monitor employee out-of-pocket expenses and supplier bills to keep your costs under control.
- **Project Coordination** — Access and list projects managed in FreeAgent to see how they impact your finances.
- **Financial Reporting** — Retrieve high-level Profit and Loss summaries to understand your business performance in real-time.
- **Organization Metadata** — Access company settings and chart of accounts categories for consistent financial reporting.

### How it works

1. Subscribe to this server through the Vinkius Marketplace
2. Authorize your FreeAgent account via OAuth 2.0
3. Start managing your accounting data from Claude, Cursor, or any MCP client

### Who is this for?

- **Freelancers & Contractors** — quickly check if an invoice has been paid or list recent expenses while working on a project.
- **Small Business Owners** — get a real-time overview of your company's P&L and bank balances via simple AI commands.
- **Accountants & Bookkeepers** — automate the retrieval of transaction history and contact metadata for faster reconciliation.


## Available Tools (12)
- **get_contact_details**: Get contact metadata
- **get_invoice_details**: Get invoice metadata
- **get_profit_and_loss**: Get P&L summary
- **list_bank_transactions**: List transactions for an account
- **list_purchase_bills**: List purchase invoices (bills)
- **list_chart_of_accounts**: List accounting categories
- **list_contacts**: List customers and suppliers
- **list_out_of_pocket_expenses**: List employee expenses
- **list_invoices**: List sales invoices
- **list_projects**: List active projects
- **get_company_details**: Get company metadata
- **list_bank_accounts**: List bank accounts


## 💬 Prompt Examples

Here are some examples of how you can interact with the **FreeAgent** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Show me my 5 most recent sales invoices and their status."

**🤖 AI Agent:**
> Retrieving invoices... I found your 5 most recent invoices, including 'INV-001' (Status: Paid) and 'INV-002' (Status: Open). Would you like the details for the open ones?

---

**👤 You:**
> "List all bank accounts and their current balances."

**🤖 AI Agent:**
> Fetching bank accounts... You have 2 accounts: 'Business Current Account' (£12,450.00) and 'Tax Reserve' (£5,200.00). Would you like to see recent transactions for either?

---

**👤 You:**
> "Get my Profit and Loss summary for the last month."

**🤖 AI Agent:**
> Retrieving P&L data... For the last month, your total income was £8,500.00 and total expenses were £3,200.00, resulting in a net profit of £5,300.00.


## ❓ FAQ

**Q: How do I connect my FreeAgent account?**
This server uses OAuth 2.0. Simply click 'Connect' in the Vinkius interface, and you will be redirected to FreeAgent to authorize the integration.

**Q: Can I see my actual bank transactions using the agent?**
Yes! The 'list_bank_transactions' tool allows you to retrieve the history for any configured bank account in your FreeAgent profile.

**Q: How do I filter for overdue invoices?**
Use the 'list_invoices' tool and set the 'nested_state' parameter to 'Overdue'. The agent will return a list of all clients with outstanding payments.

**Q: Is Profit and Loss data available?**
Yes, the 'get_profit_and_loss' tool provides a summary report for any specified date range, helping you track your business health.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/freeagent](https://vinkius.com/mcp/freeagent)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **FreeAgent** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `freeagent` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **FreeAgent** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "freeagent": {
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
