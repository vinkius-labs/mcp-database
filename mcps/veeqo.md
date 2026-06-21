# Veeqo MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/veeqo)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [ecommerce](../categories/ecommerce.md)

Manage multi-channel e-commerce inventory, shipping, and order fulfillment from one platform that syncs with Amazon and beyond.

## Description
Connect your **Veeqo** account to any AI agent and simplify how you manage your multi-channel retail, inventory levels, and shipping workflows through natural conversation.

### What you can do

- **Order Management** — List all sales orders, retrieve line-item details, and create manual orders for specific customers.
- **Inventory Control** — Query your product catalog and monitor real-time stock levels across all your channels.
- **Customer Directory** — List and inspect customer data associated with your orders to maintain your CRM.
- **Shipping Monitoring** — Track shipments and list fulfillment history to stay on top of your logistics.
- **SKU Insights** — Fetch detailed metadata and variant status for any product in your inventory.

### How it works

1. Subscribe to this server
2. Enter your Veeqo API Key (found in your user profile settings)
3. Start managing your e-commerce operations from Claude, Cursor, or any MCP client

### Who is this for?

- **E-commerce Managers** — quickly check stock levels and monitor order statuses via simple AI queries.
- **Operations Teams** — track shipments and manage the product catalog directly from the workspace.
- **Retail Business Owners** — get instant bird's-eye views of sales history and inventory health via the AI assistant.


## Available Tools
- **create_manual_order**: Create a new order
- **get_order_details**: Get details for a specific order
- **get_product_details**: Get details for a specific product
- **list_customers**: List Veeqo customers
- **list_orders**: List Veeqo orders
- **list_inventory_products**: List products
- **list_shipments**: List shipments


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Veeqo** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all active orders in my Veeqo account."

**🤖 AI Agent:**
> I've retrieved your orders. You have 5 active sales orders including #10293, #10294, and #10295. Their statuses range from 'Awaiting Shipment' to 'Picking'. Which one should we inspect?

---

**👤 You:**
> "Check the current stock for 'Blue T-Shirt' in the inventory."

**🤖 AI Agent:**
> Fetching product details... The 'Blue T-Shirt' (SKU: TS-BLUE-01) has 42 units remaining in your main warehouse and 15 units in the secondary location. Shall I set a low-stock alert?

---

**👤 You:**
> "Show me the last 3 shipments and their tracking numbers."

**🤖 AI Agent:**
> I've retrieved the latest shipments: #SH-8823 (Track: 1Z99...), #SH-8824 (Track: 1Z88...), and #SH-8825 (Track: 1Z77...). All have been dispatched successfully via UPS.


## ❓ FAQ

**Q: Can I check the stock level of a specific SKU via AI?**
Yes! Use the `list_inventory_products` tool to see your catalog, or `get_product_details` with a specific Product ID to see variant stock levels.

**Q: How do I see the latest shipping updates?**
Run the `list_shipments` query. The agent will retrieve a history of recent shipments, allowing you to monitor fulfillment progress directly from the conversation.

**Q: Is it possible to create a manual order via AI?**
Absolutely. Use the `create_manual_order` action. You'll need to provide the customer details and an array of line items in JSON format to initiate the order.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/veeqo](https://vinkius.com/mcp/veeqo)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Veeqo** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `veeqo` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Veeqo** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "veeqo": {
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
