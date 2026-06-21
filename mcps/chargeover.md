# ChargeOver MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/chargeover)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [finance-accounting](../categories/finance-accounting.md)

Manage recurring billing and invoicing via ChargeOver — track customers, monitor subscriptions, and analyze transactions directly from any AI agent.

## Description
Connect your **ChargeOver** account to any AI agent and take full control of your recurring billing and invoicing operations through natural conversation. Streamline how you manage subscriptions and customer payments.

### What you can do

- **Customer Oversight** — List and retrieve details for all customer profiles and their contact information natively
- **Invoice Management** — Monitor generated invoices and their current payment status flawlessly
- **Subscription Tracking** — List and retrieve details for active and inactive customer packages securely
- **Transaction Auditing** — Access and monitor all billing transactions and payment history flawlessly
- **Quote Control** — List and review sales quotes to manage your revenue pipeline securely
- **Account Visibility** — Retrieve core account and user information directly within your workspace

### How it works

1. Subscribe to this server
2. Enter your ChargeOver Public Key, Private Key, and Subdomain
3. Start managing your recurring billing from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Billing Managers** — monitor subscription health and review invoice statuses using natural language
- **Accounts Receivable Teams** — audit transaction history and customer balances without opening the dashboard
- **Sales Ops** — quickly look up quote details and customer profiles straight from their chat interface
- **Business Owners** — verify total recurring revenue and transaction volumes


## Available Tools
- **get_chargeover_account**: Retrieve core account and user information
- **get_customer_details**: Get detailed information for a specific customer
- **get_invoice_details**: Get detailed information for a specific invoice
- **list_chargeover_customers**: List all customers
- **list_chargeover_invoices**: List all invoices
- **list_billing_quotes**: List all sales quotes
- **list_billing_subscriptions**: List all customer subscriptions (packages)
- **list_billing_transactions**: List all billing transactions


## 💬 Prompt Examples

Here are some examples of how you can interact with the **ChargeOver** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Show me the last 5 invoices in ChargeOver."

**🤖 AI Agent:**
> Retrieving your recent invoices... I found 5 items totaling $2,100.00. 4 are 'Paid' and 1 is 'Overdue'. Would you like to see the details for the overdue invoice?

---

**👤 You:**
> "List all customers with active subscriptions."

**🤖 AI Agent:**
> Checking subscriptions... I found 12 customers with active packages, including 'Acme Corp' and 'Global Industries'. I can list their contact details for you.

---

**👤 You:**
> "What was my total transaction volume today?"

**🤖 AI Agent:**
> Retrieving today's transactions... You had 8 successful transactions totaling $1,245.50. There were no failed attempts recorded today.


## ❓ FAQ

**Q: Can I check the status of a specific invoice?**
Yes! Use the `get_invoice_details` tool with the unique invoice ID. The agent will return the full record, including the current balance and payment status.

**Q: How do I see all active subscriptions?**
Use the `list_billing_subscriptions` tool. Your agent will fetch all customer packages, allowing you to filter for those that are currently in an active state.

**Q: Where do I find my API Public and Private keys?**
Log in to your ChargeOver account and navigate to **Settings > Developer > REST API**. You can generate and copy your keys from that section.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/chargeover](https://vinkius.com/mcp/chargeover)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **ChargeOver** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `chargeover` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **ChargeOver** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "chargeover": {
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
