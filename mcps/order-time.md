# Order Time MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/order-time)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [inventory-management](../categories/inventory-management.md)

Inventory and order management — manage items, customers, and sales orders via Order Time.

## Description
Connect your **Order Time** account to empower your AI agents with advanced inventory and order management capabilities. This server provides programmatic access to the Order Time REST API for seamless tracking of products, customers, and fulfillment workflows.

### What you can do

- **Inventory Visibility** — List and inspect complete product catalogs and part items
- **Customer Management** — Access detailed customer profiles and historical records
- **Sales & Purchase Tracking** — Monitor the status of sales orders and purchase orders in real-time
- **Custom Field Access** — Retrieve specialized metadata through custom field definitions
- **Operational Efficiency** — Automate inventory queries and order status checks through simple natural language commands

### How it works

1. Subscribe to this server
2. Enter your **Order Time API Key**, **User Email**, and **Password**
3. Start managing your inventory from Claude, Cursor, or any MCP client


## Available Tools (9)
- **get_customer**: Get customer details
- **get_item**: Get item details
- **get_purchase_order**: Get purchase order details
- **get_sales_order**: Get sales order details
- **list_custom_fields**: List custom field definitions
- **list_customers**: List all customers
- **list_items**: List inventory items
- **list_purchase_orders**: List purchase orders
- **list_sales_orders**: List sales orders


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Order Time** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List my inventory items."

**🤖 AI Agent:**
> Fetching items... I've found 150 items in your catalog. Here are the most recent ones...


## ❓ FAQ

**Q: How do I generate an API Key?**
The Master Admin can generate an API Key within the Order Time application settings.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/order-time](https://vinkius.com/mcp/order-time)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Order Time** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `order-time` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Order Time** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "order-time": {
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
