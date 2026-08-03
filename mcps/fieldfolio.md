# Fieldfolio MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/fieldfolio)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [e-commerce](../categories/e-commerce.md)

Connect Fieldfolio to automate wholesale management — manage products, orders, and inventory directly from your AI agent.

## Description
Fieldfolio is a leading B2B wholesale marketplace. This MCP server allows your AI agent to interact with your Fieldfolio seller account flawlessly.

### Key Features
- **Product Orchestration** — List all items in your wholesale catalog and fetch detailed metadata for specific products natively.
- **Order Management** — Retrieve and inspect wholesale orders to stay updated on fulfillment and sales flawlessly.
- **Inventory Intelligence** — Query real-time stock levels and update inventory quantities directly from the agent flawlessy.
- **Customer CRM** — Access retail customer profiles and order history to personalize business relationships flawlessly.
- **Catalog Search** — Search your entire wholesale catalog by keyword to quickly find specific items flawlessly.
- **Webhook Auditing** — List active webhooks to ensure your third-party integrations are synchronized flawlessly.

### How it works
1. Subscribe to this server
2. Enter your Fieldfolio API Token (found in Settings > Integrations)
3. Start managing your wholesale business from Claude, Cursor, or any MCP-compatible client

### Who is this for?
- **Wholesale Managers** — monitor sales trends and order statuses without manual dashboard exports
- **Operations Teams** — sync product data and inventory levels directly from your chat workflow
- **Sales Reps** — quickly look up product availability and customer history through simple natural language queries


## Available Tools (12)
- **get_customer**: Get details for a specific retail customer
- **get_me**: Get details for the authorized seller account
- **get_order**: Get details for a specific wholesale order
- **get_product**: Get details for a specific product
- **list_categories**: List all product categories
- **list_customers**: List all retail customers
- **list_inventory**: List inventory levels for all products
- **list_orders**: List all wholesale orders
- **list_products**: List all products in your wholesale catalog
- **list_webhooks**: List all configured webhooks
- **search_catalog**: Search the wholesale catalog by keyword
- **update_inventory**: Update inventory quantity for a specific product


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Fieldfolio** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List my active wholesale orders."

**🤖 AI Agent:**
> I've retrieved your recent orders. You have 12 orders currently pending, including 'Retailer A' (Order #1025) and 'Store B' (Order #1026). Would you like to see the item breakdown for any of these?

---

**👤 You:**
> "Check the inventory level for 'Summer T-Shirt'."

**🤖 AI Agent:**
> Inspecting inventory... 'Summer T-Shirt' (SKU: ST-101) currently has 45 units in stock. Shall I alert you if it drops below 10?

---

**👤 You:**
> "Search the catalog for 'Ceramic Vases'."

**🤖 AI Agent:**
> Searching catalog... I found 3 matching items: 'Minimalist Ceramic Vase', 'Blue Glazed Vase', and 'Rustic Pot'. Which one would you like more details on?


## ❓ FAQ

**Q: How do I obtain my Fieldfolio API Token?**
Log in to your Fieldfolio Seller account, go to **Settings > Integrations**, and click on **Generate API Key**. Note that you must be on a qualifying paid plan to see this option.

**Q: Which plans include API access?**
API access is available on Fieldfolio's Startup, Business, and Enterprise plans.

**Q: Can I update stock levels via this integration?**
Yes! The `update_inventory` tool allows you to set new stock quantities for specific products in your catalog flawlessy.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/fieldfolio](https://vinkius.com/mcp/fieldfolio)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Fieldfolio** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `fieldfolio` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Fieldfolio** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "fieldfolio": {
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
