# Youzan / 有赞 MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/youzan)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [ecommerce](../categories/ecommerce.md)

Leading E-commerce and retail SaaS platform — manage products, orders, and customers via AI.

## Description
Empower your AI agent to orchestrate your retail business with **Youzan** (有赞), the dominant E-commerce and retail SaaS platform in China. By connecting Youzan to your agent, you transform complex store management and order tracking into a natural conversation. Your agent can instantly list products, retrieve order details, manage customer profiles, and even provide sales statistics without you ever needing to navigate the comprehensive Youzan Backend. Whether you are managing an online shop or a large-scale retail operation, your agent acts as a real-time retail assistant, keeping your data accurate and your sales moving.

### What you can do

- **Product Orchestration** — List all items on sale, get detailed product information, and browse store categories.
- **Order Management** — List sold trades and retrieve detailed order information to track fulfillment and delivery.
- **Customer CRM Control** — Search and manage customer profiles, including contact details and purchase history.
- **Inventory Monitoring** — Retrieve stock levels and SKU information for any item in your shop.
- **Sales Insights** — Get high-level summaries of sales performance and product rankings.

### How it works

1. Subscribe to this server
2. Enter your Youzan Client ID, Client Secret, and Shop ID (kdt_id)
3. Start managing your retail operations through Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **E-commerce Managers** — monitor store performance, audit orders, and manage products through natural language queries.
- **Store Owners** — track sales progress and update inventory details directly from your AI-powered workspace.
- **Customer Success Teams** — retrieve customer profiles and order histories via a unified AI interface.
- **Youzan Power Users** — integrate your existing retail workflows into your AI-driven daily routines.


## Available Tools
- **get_customer**: Get customer details
- **get_inventory**: Get item SKU inventory
- **get_item**: Get item details
- **get_order**: Get order details
- **get_sales_stats**: Get sales performance stats
- **get_shop**: Get shop information
- **list_categories**: List item categories
- **list_customers**: Search SCRM customers
- **list_items**: List on-sale items
- **list_orders**: List sold trades


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Youzan / 有赞** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all products currently on sale in my shop."

**🤖 AI Agent:**
> I've retrieved your on-sale items. You have 25 active products, including 'Spring Collection T-Shirt' and 'Organic Tea Set'. Would you like more details or stock levels for any of them?

---

**👤 You:**
> "Show me the last 5 orders from today."

**🤖 AI Agent:**
> I've listed the last 5 orders. They include transactions for 'Wireless Headphones' and 'Designer Watch'. Total revenue from these orders is approximately ¥3,500. Should I check the shipping status for any of them?

---

**👤 You:**
> "Check the inventory for item ID 12345678."

**🤖 AI Agent:**
> I've retrieved the inventory for item 12345678. You have 3 variants: Small (10 in stock), Medium (5 in stock), and Large (Out of stock). Would you like me to notify you when the Large variant is replenished?


## ❓ FAQ

**Q: How do I find my Youzan Client ID and Secret?**
Log in to the [Youzan Cloud Console](https://console.youzanyun.com/), create an application, and you will find your Client ID (App Key) and Client Secret in the app settings.

**Q: Where is my Shop ID (kdt_id)?**
Your Shop ID (kdt_id) can be found in the bottom left corner of your Youzan store administration backend.

**Q: Can I check stock levels for specific product variants?**
Yes. Use the `get_inventory` tool with the product's item ID. It will return a list of all SKUs (variants) along with their current stock levels and pricing.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/youzan](https://vinkius.com/mcp/youzan)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Youzan / 有赞** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `youzan` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Youzan / 有赞** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "youzan": {
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
