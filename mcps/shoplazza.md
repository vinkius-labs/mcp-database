# Shoplazza / 店匠 MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/shoplazza)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [ecommerce](../categories/ecommerce.md)

Global E-commerce platform — manage products, orders, and inventory via AI.

## Description
Empower your AI agent to orchestrate your global retail business with **Shoplazza** (店匠), the premier E-commerce platform for international brands. By connecting Shoplazza to your agent, you transform complex store management and order tracking into a natural conversation. Your agent can instantly list your products, retrieve detailed order information, monitor inventory levels, and even browse store collections without you ever needing to navigate the Shoplazza Admin interface. Whether you are managing a single boutique or a large-scale international operation, your agent acts as a real-time retail assistant, keeping your data accurate and your global sales moving.

### What you can do

- **Product Orchestration** — List all items in your store, get detailed product metadata, and browse collections.
- **Order Management** — List and retrieve detailed order information to track fulfillment, payments, and delivery.
- **Inventory Monitoring** — Retrieve real-time inventory levels for your products to ensure stock availability.
- **Customer Insights** — Search and manage customer profiles and their purchase history.
- **Store Configuration** — Access general shop information and monitor configured webhooks.

### How it works

1. Subscribe to this server
2. Enter your Shoplazza Shop Domain and Admin API Access Token
3. Start managing your retail operations through Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Global E-commerce Managers** — monitor store performance, audit orders, and manage products across regions through natural language queries.
- **Retail Operations Teams** — track inventory levels and coordinate order fulfillment directly from your AI-powered workspace.
- **Business Analysts** — retrieve store data for sales performance analysis and inventory forecasting.
- **Shoplazza Power Users** — integrate your existing retail workflows into your AI-driven daily routines.


## Available Tools (10)
- **list_collections**: List product collections
- **list_customers**: List shop customers
- **list_orders**: List shop orders
- **list_products**: List shop products
- **list_webhooks**: List store webhooks
- **get_customer**: Get customer details
- **get_inventory_levels**: Get inventory levels
- **get_order**: Get order details
- **get_product**: Get product details
- **get_shop_info**: Get shop information


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Shoplazza / 店匠** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all products in my Shoplazza store."

**🤖 AI Agent:**
> I've retrieved your Shoplazza products. You have 30 active items, including 'Classic Leather Boots' and 'Waterproof Jacket'. Would you like to see the details or current stock for any of them?

---

**👤 You:**
> "Show me the last 5 orders from my Shoplazza shop."

**🤖 AI Agent:**
> I've listed the last 5 orders from Shoplazza. They include recent transactions for 'Silk Scarf' and 'Silver Watch'. Total value for these orders is $450. Would you like to check the shipping status?

---

**👤 You:**
> "Check the inventory level for item ID 'inv-123456'."

**🤖 AI Agent:**
> I've retrieved the inventory data for item 'inv-123456'. Current stock level is 15 units. Would you like me to notify you if it falls below a certain threshold?


## ❓ FAQ

**Q: How do I find my Shoplazza Access Token?**
Log in to the [Shoplazza Partner Platform](https://partners.shoplazza.com/), create an application, and follow the OAuth 2.0 flow to obtain your Admin API Access Token.

**Q: What is the 'shop_domain' format?**
Your shop domain should be the full URL of your Shoplazza admin instance, typically in the format: `your-store.myshoplazza.com`.

**Q: Can I check inventory for specific items?**
Yes. Use the `get_inventory_levels` tool. You can optionally provide a comma-separated list of `inventory_item_ids` to retrieve the stock levels for those specific items.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/shoplazza](https://vinkius.com/mcp/shoplazza)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Shoplazza / 店匠** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `shoplazza` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Shoplazza / 店匠** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "shoplazza": {
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
