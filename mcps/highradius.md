# HighRadius MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/highradius)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [finance-payments](../categories/finance-payments.md)

Manage invoices, payments, disputes, and deductions via HighRadius API.

## Description
Connect **HighRadius** to any AI agent and automate your Order-to-Cash operations -- manage invoices, reconcile payments, handle disputes, and track deductions through natural conversation.

### What you can do
- **Invoice Management** -- List and inspect all invoices with amounts and due dates
- **Payment Tracking** -- View all payments received and their reconciliation status
- **Payment Reconciliation** -- Match payments to invoices automatically
- **Customer Management** -- View customer profiles and outstanding balances
- **Dispute Handling** -- Create and track disputes for invoice discrepancies
- **Deduction Tracking** -- Monitor short payments and adjustments

### How it works
1. Subscribe to this server
2. Enter your HighRadius Access Token
3. Start managing receivables from Claude, Cursor, or any MCP-compatible client

HighRadius is a leading Order-to-Cash automation platform used by enterprises to streamline accounts receivable, cash application, and collections.

### Who is this for?
- **AR Teams** -- Monitor invoices and reconcile payments without logging into the platform
- **Finance Managers** -- Track disputes, deductions, and cash application status
- **Collections Agents** -- View customer balances and outstanding invoices quickly


## Available Tools
- **get_cash_application_status**: Get the current status of the cash application process
- **create_dispute**: Body should include invoice_id, reason, and amount.

Create a new dispute record
- **list_customers**: List all customers in the system
- **list_deductions**: List all deductions in the system
- **list_disputes**: List all disputes in the system
- **get_customer**: Get details of a specific customer
- **get_invoice**: Get details of a specific invoice
- **get_payment**: Get details of a specific payment
- **list_invoices**: Use this to get an overview of outstanding receivables.

List all invoices in the system
- **list_payments**: List all payment records
- **reconcile_payment**: Provide the payment ID and an array of invoice IDs to reconcile.

Reconcile a payment against one or more invoices


## 💬 Prompt Examples

Here are some examples of how you can interact with the **HighRadius** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Show me all outstanding invoices."

**🤖 AI Agent:**
> Found 5 invoices: 1. INV-001 ($15,000 - Due: 2025-04-01). 2. INV-002 ($8,500 - Due: 2025-04-15).

---

**👤 You:**
> "Reconcile payment PAY-123 against invoices INV-001 and INV-002."

**🤖 AI Agent:**
> Payment PAY-123 reconciled successfully against 2 invoices.

---

**👤 You:**
> "Create a dispute for invoice INV-003 with reason 'Incorrect pricing' and amount $2,000."

**🤖 AI Agent:**
> Dispute created successfully! Dispute ID: DISP-456.


## ❓ FAQ

**Q: How do I get my HighRadius Access Token?**
Log in to your HighRadius account, navigate to Settings > API Access, and generate a new token.

**Q: Can I reconcile payments automatically?**
Yes! Use the reconcile_payment action with the payment ID and an array of invoice IDs to match payments to invoices.

**Q: Can I create disputes for invoice discrepancies?**
Yes! Use the create_dispute action with a JSON body including the invoice ID, reason, and disputed amount.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/highradius](https://vinkius.com/mcp/highradius)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **HighRadius** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `highradius` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **HighRadius** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "highradius": {
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
