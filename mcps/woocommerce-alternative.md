# WooCommerce MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/woocommerce-alternative)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [ecommerce](../categories/ecommerce.md)

Manage your WooCommerce store — audit products, orders, and reports via AI.

## Description
Empower your AI agent to orchestrate your entire e-commerce ecosystem with **WooCommerce**, the world's most customizable open-source platform. By connecting WooCommerce to your agent, you transform complex store management into a natural conversation. Your agent can instantly list your products, audit recent orders, and retrieve sales reports without you ever touching a dashboard. Whether you are running a boutique shop or a high-volume enterprise store, your agent acts as a real-time store operator, ensuring your business is always healthy and efficient.

### What you can do

- **Order Auditing** — List all recent and historical orders, and retrieve detailed metadata for each, including status and customer info.
- **Product Oversight** — List all products and categories in your account to maintain a structured catalog.
- **Customer Administration** — Query customer profiles and monitor their purchase history to understand your audience.
- **Sales Intelligence** — List store reports and system status to stay on top of your performance metrics in real-time.
- **Coupon Governance** — List all active coupons to ensure your promotional strategy is correctly applied.

### How it works

1. Subscribe to this server
2. Enter your Store URL, Consumer Key, and Consumer Secret
3. Start managing your store data through Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Store Owners** — monitor daily sales and order fulfillment straight from your workflow.
- **Marketing Leads** — verify if new products have been correctly published and coupons are active.
- **Support Teams** — perform rapid order audits and check customer details without manual dashboard logins.
- **Operations Managers** — automate store querying to orchestrate cross-functional e-commerce teams smoothly.


## Available Tools (10)
- **get_order**: Get details for a specific order
- **get_product**: Get details for a specific product
- **get_system_status**: Get WooCommerce system status
- **list_coupons**: List all coupons
- **list_customers**: List WooCommerce customers
- **list_orders**: List WooCommerce orders
- **list_categories**: List product categories
- **list_products**: List WooCommerce products
- **list_reports**: List WooCommerce reports
- **update_order**: Update an order status


## 💬 Prompt Examples

Here are some examples of how you can interact with the **WooCommerce** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List my last 5 orders in WooCommerce."

**🤖 AI Agent:**
> I've retrieved your recent orders. You have 5 new transactions, including order #1234 for $45.00 by John Smith. Would you like the full details for any of them?

---

**👤 You:**
> "Show me all my draft products."

**🤖 AI Agent:**
> I've found 3 products in draft status: 'New Hoodie', 'Limited Poster', and 'Demo Shirt'. I can provide category and pricing info for each if you like.

---

**👤 You:**
> "What is the system status of my store?"

**🤖 AI Agent:**
> Your WooCommerce system status is healthy. Environment: Production, WooCommerce version: 8.5.0, Database status: OK. Is there anything specific you'd like to check?


## ❓ FAQ

**Q: How do I find my WooCommerce API keys?**
In your WordPress dashboard, go to **WooCommerce** > **Settings** > **Advanced** > **REST API** and click 'Add key'. Copy the Consumer Key and Secret and paste them below.

**Q: Can the agent update order statuses?**
Yes. Use the `update_order` tool providing the Order ID and the new status (e.g., 'completed', 'processing'). Your agent will confirm the update instantly.

**Q: Is it possible to see sales reports via the agent?**
Yes. The `list_reports` tool allows your agent to retrieve high-level sales data and performance reports directly from your store.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/woocommerce-alternative](https://vinkius.com/mcp/woocommerce-alternative)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **WooCommerce** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `woocommerce-alternative` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **WooCommerce** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "woocommerce-alternative": {
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
