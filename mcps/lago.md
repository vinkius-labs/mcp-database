# Lago MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/lago)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [money-moves](../categories/money-moves.md)

Manage your metering and usage-based billing with Lago — handle customers, subscriptions, plans, and events directly from your AI agent.

## Description
Connect **Lago** to your AI agent to automate your metering and billing infrastructure. Lago is the open-source alternative to Stripe Billing, designed for complex usage-based pricing models.

### What you can do

- **Customer Management** — Create and update customer profiles with `upsert_customer` and retrieve details with `get_customer`.
- **Subscription Lifecycle** — Assign plans to customers using `create_subscription` and monitor them with `get_subscription`.
- **Billing Infrastructure** — Define billing plans with `create_plan` and set up `create_billable_metric` to track consumption.
- **Usage Tracking** — Send real-time usage data with `send_event` or `batch_events` to trigger accurate billing.
- **Financial Operations** — Manage wallets, apply coupons, and list invoices to keep your revenue operations running smoothly.

### How it works

1. Subscribe to this server
2. Enter your Lago API Key
3. Start managing your billing logic from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **SaaS Founders** — quickly check customer subscription status or update plans without leaving the chat.
- **Growth Engineers** — automate the creation of coupons and wallets for promotional campaigns.
- **Finance Teams** — list invoices and verify billable metrics through natural language queries.


## Available Tools (12)
- **create_coupon**: Create a coupon
- **create_plan**: Create a new billing plan
- **create_subscription**: Assign a plan to a customer (create subscription)
- **create_wallet**: Create a wallet for prepaid credits
- **get_customer**: Retrieve a customer by external ID
- **get_subscription**: Retrieve a subscription by external ID
- **list_invoices**: List all invoices
- **send_event**: Send a usage event
- **upsert_customer**: Requires an external_id.

Create or update a customer in Lago
- **apply_coupon**: Apply a coupon to a customer
- **batch_events**: Send a batch of usage events
- **create_billable_metric**: Create a billable metric


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Lago** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Create a new customer in Lago with external ID 'user_123' and email 'dev@example.com'."

**🤖 AI Agent:**
> I've successfully created the customer record for 'user_123'. Their profile is now active in Lago and ready for subscriptions.

---

**👤 You:**
> "Show me the subscription details for ID 'sub_98765'."

**🤖 AI Agent:**
> Fetching subscription 'sub_98765'... It is currently active on the 'Premium' plan, started on 2023-10-01, and is set for monthly billing.

---

**👤 You:**
> "List all invoices for my Lago account."

**🤖 AI Agent:**
> I've retrieved the latest invoices. You have 3 pending invoices for this month and 12 paid invoices from the previous quarter. Would you like to see the details for a specific one?


## ❓ FAQ

**Q: How do I track a new usage event for a customer?**
Use the `send_event` tool. You'll need to provide the customer's external ID and the metric code to record the consumption in real-time.

**Q: Can I create a new billing plan with specific charges?**
Yes, use the `create_plan` tool. You can define the name, interval, and base amount, as well as pass a JSON object for specific charges.

**Q: Is it possible to apply a discount to a customer?**
Absolutely. First, create a coupon using `create_coupon`, then use the `apply_coupon` tool to link it to a specific customer's external ID.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/lago](https://vinkius.com/mcp/lago)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Lago** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `lago` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Lago** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "lago": {
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
