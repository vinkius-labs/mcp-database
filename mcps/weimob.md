# Weimob / 微盟 MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/weimob)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [ecommerce](../categories/ecommerce.md)

Leading E-commerce and marketing SaaS platform in China — manage products, orders, and members via AI.

## Description
Empower your AI agent to orchestrate your retail business with **Weimob** (微盟), the dominant E-commerce and marketing SaaS platform in China. By connecting Weimob to your agent, you transform complex shop management and order tracking into a natural conversation. Your agent can instantly list your goods, retrieve detailed order information, manage customer profiles, and even provide sales statistics without you needing to navigate the comprehensive Weimob Cloud interface. Whether you are managing a WeChat mini-program shop or a large-scale retail operation, your agent acts as a real-time retail assistant, keeping your data accurate and your sales moving.

### What you can do

- **Product Orchestration** — List all items on sale, get detailed product information, and browse store categories.
- **Order Management** — List sold trades and retrieve detailed order information to track fulfillment and delivery.
- **Customer CRM Control** — Search and manage member profiles, including contact details and purchase history.
- **Inventory Monitoring** — Retrieve stock levels for any SKU in your shop to ensure product availability.
- **Sales Insights** — Get high-level summaries of sales performance and performance statistics.

### How it works

1. Subscribe to this server
2. Enter your Weimob Client ID and Client Secret
3. Start managing your retail operations through Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **E-commerce Managers** — monitor store performance, audit orders, and manage products through natural language queries.
- **Marketing Leads** — track member engagement and coordinate between different promotional activities via a unified AI interface.
- **Operations Teams** — oversee multiple shops and inventory levels without manual technical overhead.
- **Weimob Users** — integrate your existing retail workflows into your AI-driven daily routines.


## Available Tools (10)
- **get_order**: Get order details
- **get_sales_stats**: Get sales statistics
- **get_shop_info**: Get Weimob shop information
- **list_categories**: List product categories
- **list_customers**: List shop customers
- **list_goods**: List shop products
- **list_orders**: List shop orders
- **get_customer**: Get customer details
- **get_goods_detail**: Get product details
- **get_inventory**: Get SKU inventory


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Weimob / 微盟** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all products currently on sale in my Weimob shop."

**🤖 AI Agent:**
> I've retrieved your on-sale goods. You have 25 active products, including 'Summer Dress' and 'Smart Watch'. Would you like more details or stock levels for any of them?

---

**👤 You:**
> "Show me the last 5 orders from today."

**🤖 AI Agent:**
> I've listed the last 5 orders. They include transactions for 'Organic Coffee' and 'Wireless Earbuds'. Total revenue from these orders is approximately ¥2,800. Should I check the fulfillment status for any of them?

---

**👤 You:**
> "Get sales statistics for the last 7 days."

**🤖 AI Agent:**
> Across the last 7 days, your shop generated ¥150,000 in revenue from 450 orders. Your top-selling category is 'Electronics'. Would you like a more detailed breakdown by product?


## ❓ FAQ

**Q: How do I find my Weimob Client ID and Secret?**
Log in to the [Weimob Cloud Console](https://cloud.weimob.com/), create an application, and you will find your Client ID (App Key) and Client Secret in the application management section.

**Q: Can I check stock levels for specific SKUs?**
Yes. Use the `get_inventory` tool with the SKU ID. It will return the current stock level for that specific product variant.

**Q: Does this server support multi-shop management?**
Yes, as long as your Client ID and Secret have authorized access to multiple shops within your Weimob organization, your agent can manage them through the unified API interface.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/weimob](https://vinkius.com/mcp/weimob)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Weimob / 微盟** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `weimob` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Weimob / 微盟** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "weimob": {
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
