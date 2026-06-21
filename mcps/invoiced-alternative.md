# Invoiced MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/invoiced-alternative)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [erp-operations](../categories/erp-operations.md)

Get paid faster with automated invoicing, smart payment reminders, and accounts receivable workflows that reduce DSO.

## Description
Connect your **Invoiced** account to any AI agent and take full control of your accounts receivable orchestration and automated billing workflows through natural conversation.

### What you can do

- **Invoice Portfolio Orchestration** â€” List and manage all issued invoices programmatically, retrieving detailed payment metadata and aging statuses
- **Customer & Payment Intelligence** â€” Programmatically retrieve directories of customers and access complete credit profiles and payment history in real-time
- **A/R Workflow Architecture** â€” Access your complete directory of payment plans and auto-pay settings to coordinate your organizational revenue
- **Operational Monitoring** â€” Access real-time status updates for paid invoices and track collection metrics directly through your agent for instant reporting
- **Infrastructure Verification** â€” Verify account-level API connectivity and monitor transaction volume directly through your agent for perfectly coordinated service scaling

### How it works

1. Subscribe to this server
2. Retrieve your **API Key** from your Invoiced dashboard (Settings > API)
3. Start orchestrating your revenue growth from Claude, Cursor, or any MCP client

No more manual following up on overdue payments or missing billing updates. Your AI acts as your dedicated finance coordinator and accounts receivable architect.

### Who is this for?

- **Finance Managers** â€” instantly retrieve invoice summaries and monitor collection goals using natural language commands
- **Accounts Receivable Leads** â€” verify individual customer metadata and track payment history without leaving your creative workspace
- **Developers** â€” integrate high-speed Invoiced billing data into custom ERP and accounting pipelines through simple AI queries


## Available Tools (10)
- **check_invoiced_status**: Verify Invoiced API connectivity
- **create_customer**: Create a customer
- **create_invoice**: Pass line items as JSON array with name, quantity, and unit_cost.

Create an invoice
- **get_customer**: Get customer details
- **get_invoice**: Get invoice details
- **list_credit_notes**: List all credit notes
- **list_customers**: List all customers
- **list_estimates**: List all estimates
- **list_invoices**: List all invoices
- **list_payments**: List all payments


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Invoiced** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Show all unpaid invoices in my Invoiced account."

**🤖 AI Agent:**
> You have 7 unpaid invoices totaling ,450. The largest is INV-1042 for ,200 (due in 3 days). Would you like to see the customer details or send a payment reminder?

---

**👤 You:**
> "Create an invoice for customer 5001 with 2 items."

**🤖 AI Agent:**
> Invoice INV-1098 created for customer 5001. Total:  (Web Design: , SEO Audit: ). The invoice is ready to send. Would you like to add a due date?

---

**👤 You:**
> "List all estimates waiting for approval."

**🤖 AI Agent:**
> You have 4 pending estimates totaling ,000. The oldest is EST-0034 (,500) sent 12 days ago. Would you like to follow up with the customer?


## ❓ FAQ

**Q: Can I create invoices directly from my AI agent?**
Yes. Use the `create_invoice` tool with a customer ID and line items. The invoice is created instantly in your Invoiced account.

**Q: How do I track outstanding payments?**
Use `list_payments` to see all payment transactions or `list_invoices` to review invoices with their payment status and outstanding balances.

**Q: Can I manage customers and credit notes?**
Absolutely. Use `create_customer` to add new accounts, `list_customers` to browse, and `list_credit_notes` to review all issued credits.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/invoiced-alternative](https://vinkius.com/mcp/invoiced-alternative)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Invoiced** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `invoiced-alternative` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Invoiced** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "invoiced-alternative": {
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
