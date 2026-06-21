# Invoiced MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/invoiced)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [finance-accounting](../categories/finance-accounting.md)

Manage accounts receivable, invoices, and payments via Invoiced API.

## Description
Empower your AI agents to manage your billing and payments lifecycle with Invoiced. This MCP server allows you to list customers, retrieve invoice details, track payments, and view subscription plans directly through the Invoiced API. Ideal for automating accounts receivable and financial operations.


## Available Tools
- **get_customer**: Returns contact info, balance data, and payment settings. Use for deep intelligence on a customer before billing interactions.

Retrieves details for a specific customer
- **get_invoice**: Essential for auditing specific billings or providing customer support.

Retrieves details for a specific invoice
- **list_coupons**: Useful for auditing marketing incentives.

Lists all active discount coupons
- **list_customers**: Returns customer names, account numbers, and IDs. Use this as the main starting point for managing receivables or identifying specific clients.

Lists all customers in Invoiced
- **list_invoices**: Includes invoice numbers, amounts, and statuses. Essential for monitoring accounts receivable and overall revenue flow.

Lists all invoices
- **list_items**: Includes item codes, descriptions, and unit prices. Useful for auditing the available billing inventory.

Lists all items in your catalog
- **list_payments**: Returns payment methods, amounts, and transaction IDs. Use this to audit revenue collection and reconcile bank statements.

Lists all payments received
- **list_plans**: g., Monthly SaaS, Annual Support). Useful for auditing subscription-based business models.

Lists all defined subscription plans
- **list_subscriptions**: Essential for monitoring long-term customer commitments and MRR (Monthly Recurring Revenue).

Lists all active customer subscriptions
- **list_tax_rates**: Essential for auditing compliance and understanding how taxes are applied to invoices.

Lists all defined tax rates


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Invoiced** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all active customers in Invoiced."

**🤖 AI Agent:**
> I'll fetch the list of your Invoiced customers for you.

---

**👤 You:**
> "Show me the last 5 invoices generated."

**🤖 AI Agent:**
> I'll retrieve the most recent invoices from your account.

---

**👤 You:**
> "Check the status of invoice number 'INV-789'."

**🤖 AI Agent:**
> I'll look up the details and current payment status for that specific invoice.


## ❓ FAQ

**Q: How do I get Invoiced API credentials?**
Log in to your Invoiced dashboard, navigate to Settings > Developers > API Keys, and copy your API Key.

**Q: Does it support Sandbox mode?**
Yes, you can use your Invoiced sandbox API key to test all functionality without moving real money.

**Q: Can I see real-time payments?**
Yes, the list_payments tool provides access to all payment transactions recorded in your Invoiced account.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/invoiced](https://vinkius.com/mcp/invoiced)
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
3. Set Type to "SSE", enter `invoiced` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Invoiced** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "invoiced": {
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
