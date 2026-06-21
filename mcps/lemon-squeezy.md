# Lemon Squeezy MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/lemon-squeezy)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [ecommerce](../categories/ecommerce.md)

Manage e-commerce stores, products, orders, and subscriptions via the Lemon Squeezy API.

## Description
Connect your **Lemon Squeezy** account to any AI agent to automate your software sales and subscription management. This MCP server enables your agent to interact with stores, products, orders, and customer subscriptions directly from natural language interfaces using the JSON:API standard.

### What you can do

- **Store Oversight** — List all your Lemon Squeezy stores and retrieve detailed configurations and metadata
- **Product Management** — Query your entire product catalog, including pricing, status, and purchase URLs
- **Order Tracking** — List and retrieve detailed information for customer orders, including financial totals and payment status
- **Subscription Lifecycle** — Monitor active subscriptions, retrieve renewal dates, and cancel plans when necessary
- **Customer CRM** — Manage customer profiles and retrieve their complete purchase and subscription history

### How it works

1. Subscribe to this server
2. Enter your Lemon Squeezy API Key
3. Start managing your digital business from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **SaaS Founders** — Monitor sales performance and subscription health via natural language commands
- **Operations Teams** — Quickly check order details and manage customer cancellations without opening the dashboard
- **Developers** — Integrate e-commerce data and subscription management into your daily development workflow


## Available Tools (11)
- **cancel_subscription**: The customer will retain access until the end of the current billing cycle.

Cancel an active subscription
- **list_all_customers**: List all customers
- **get_customer_details**: Get details for a specific customer
- **get_order_details**: Get details for a specific order
- **get_product_details**: Get details for a specific product
- **get_store_details**: Get details for a specific store
- **get_subscription_details**: Get details for a specific subscription
- **list_all_orders**: List all orders
- **list_all_products**: List all products available in your account
- **list_stores**: List all stores in your Lemon Squeezy account
- **list_all_subscriptions**: List all active and historical subscriptions


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Lemon Squeezy** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all products in my Lemon Squeezy account."

**🤖 AI Agent:**
> I've retrieved your products. You have 5 products, including 'SaaS Pro Plan ($49.00)', 'E-book: Mastering AI ($19.00)', and 3 others. Would you like to see the purchase URLs for any of them?

---

**👤 You:**
> "Show my 5 most recent orders."

**🤖 AI Agent:**
> I found 5 recent orders. Notable ones include Order #12345 from 'John Smith' ($49.00) and Order #12344 from 'Alice Doe' ($19.00). Both are currently marked as 'paid'.

---

**👤 You:**
> "Get details for subscription ID '98765'."

**🤖 AI Agent:**
> I've fetched the details for subscription 98765. The status is 'active', and the next renewal is scheduled for July 15th. The associated customer is 'jane@example.com'.


## ❓ FAQ

**Q: How do I find my Lemon Squeezy API Key?**
Log in to your Lemon Squeezy dashboard and navigate to Settings > API to generate and copy your unique API Key.

**Q: Can I cancel a customer subscription using the agent?**
Yes, use the `cancel_subscription` tool with the unique subscription ID. The subscription will remain active until the end of the current billing cycle.

**Q: Is it possible to see the formatted price of a product?**
Yes, the tools retrieve the `total_formatted` or `price_formatted` attributes directly from the Lemon Squeezy API for easy reading.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/lemon-squeezy](https://vinkius.com/mcp/lemon-squeezy)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Lemon Squeezy** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `lemon-squeezy` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Lemon Squeezy** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "lemon-squeezy": {
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
