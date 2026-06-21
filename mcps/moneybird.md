# Moneybird MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/moneybird)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [erp-operations](../categories/erp-operations.md)

Manage your accounting via Moneybird — list invoices, track contacts, and oversee estimates directly from your AI agent.

## Description
Connect your **Moneybird** administration to your AI agent and take full control of your business accounting and invoicing through natural conversation.

### What you can do

- **Invoicing & Sales** — List all sales invoices and get detailed info on specific ones, including amounts and due dates.
- **Purchase Tracking** — Access your incoming purchase invoices from suppliers to keep track of expenses.
- **Financial Mutations** — Monitor bank mutations and all financial transactions within your administration.
- **Recurring Billing** — List and manage your recurring sales invoice templates for automated billing.
- **Ledger & Bookkeeping** — View your chart of accounts (ledger accounts) and defined accounting workflows.
- **Contact Management** — View and create customer or supplier contacts to keep your CRM updated.
- **Estimates Oversight** — Access and list your business estimates to track potential sales.

### How it works

1. Subscribe to this server
2. Enter your Moneybird Access Token and Administration ID
3. Start managing your finances from Claude, Cursor, or any MCP client

### Who is this for?

- **Entrepreneurs** — quickly check for overdue invoices or bank mutations without opening the Moneybird app.
- **Accountants** — automate the retrieval of transaction, invoice, and ledger lists for reporting.
- **Sales Teams** — verify estimate statuses and customer information during the sales cycle.


## Available Tools
- **create_contact**: Create a new contact in Moneybird
- **get_invoice**: Get specific invoice details
- **list_contacts**: List Moneybird contacts
- **list_estimates**: List business estimates
- **list_financial_mutations**: List financial transactions
- **list_invoices**: List sales invoices
- **list_ledger_accounts**: List ledger accounts
- **list_purchase_invoices**: List purchase invoices
- **list_recurring_invoices**: List recurring invoices
- **list_workflows**: List accounting workflows


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Moneybird** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all my sales invoices from the last month."

**🤖 AI Agent:**
> I've fetched your sales invoices. You have 12 invoices for the last month, including 'INV-2024-001' (€1,200.00) and 'INV-2024-002' (€850.00). 3 invoices are still marked as 'unpaid'. Would you like to see the details for the unpaid ones?

---

**👤 You:**
> "Check my recent bank mutations."

**🤖 AI Agent:**
> Retrieving financial mutations... I found 5 recent movements, including a payout from Mollie (+€1,500.00) and an automated rent payment (-€900.00). Shall I show you the remaining 3 transactions?

---

**👤 You:**
> "List my purchase invoices from suppliers."

**🤖 AI Agent:**
> I've retrieved your purchase invoices. You have 8 incoming invoices this month, including 'Adobe Subscription' ($20.99) and 'AWS Cloud Services' ($145.50). 2 are currently awaiting payment. Shall I provide the due dates for those?


## ❓ FAQ

**Q: How do I find my Moneybird Administration ID?**
Log in to Moneybird via your browser. The ID is the numeric string in the URL immediately following 'moneybird.com/' (e.g., in moneybird.com/123456789/..., the ID is 123456789).

**Q: Can I see my bank transactions through this server?**
Yes! Use the `list_financial_mutations` tool to retrieve all bank mutations and financial movements recorded in your Moneybird administration.

**Q: Does this support purchase invoices (expenses)?**
Yes. The `list_purchase_invoices` tool allows you to see all incoming invoices from your suppliers and track your business expenses.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/moneybird](https://vinkius.com/mcp/moneybird)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Moneybird** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `moneybird` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Moneybird** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "moneybird": {
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
