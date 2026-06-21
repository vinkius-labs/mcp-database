# Order Desk MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/order-desk-alternative)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [industry-titans](../categories/industry-titans.md)

Route and manage orders from multiple sales channels to fulfillment providers with automation rules that handle the complexity.

## Description
Connect your **Order Desk** account to any AI agent and take full control of your e-commerce orchestration and order fulfillment through natural conversation. Order Desk is a multi-channel order management system that connects with hundreds of shopping carts and shipping providers, and this integration allows you to retrieve order metadata, manage inventory items, and track shipments directly from your chat interface.

### What you can do

- **Order & Fulfillment Orchestration** — List and filter store orders in real-time and retrieve detailed metadata programmatically across all your connected channels.
- **Inventory Lifecycle Management** — Access and monitor your centralized inventory database and create or update stock levels directly from the AI interface to ensure product availability.
- **Shipment Tracking Intelligence** — Add shipment records and tracking numbers to existing orders via natural language to keep your customers informed.
- **Custom Field Control** — Access and manage order-level custom data and checkout metadata using simple AI commands.
- **Operational Monitoring** — Track system responses and verify connection health to ensure your e-commerce workflows are always optimized.

### How it works

1. Subscribe to this server
2. Enter your Order Desk Store ID and API Key from your store settings
3. Start managing your orders and inventory from Claude, Cursor, or any MCP-compatible client

No more manual logging into the dashboard to check order status or inventory levels. Your AI acts as a dedicated operations manager or fulfillment coordinator.

### Who is this for?

- **E-commerce Merchants** — quickly retrieve order summaries and monitor inventory health without switching apps.
- **Operations Leads** — automate the management of shipments and track warehouse activity via natural conversation.
- **Developers** — integrate real-time order data and store configuration directly within the chat.


## Available Tools
- **create_store_order**: Create a new order
- **create_order_shipment**: ) to an existing order.

Add a shipment to an order
- **delete_store_order**: Delete an order from the store
- **get_inventory_item**: Get details for a specific inventory item
- **get_order_details**: Get details for a specific order
- **list_inventory_items**: List inventory items
- **list_order_items**: List line items within an order
- **list_store_orders**: List orders from the store
- **list_order_shipments**: List shipments for an order
- **test_orderdesk_connection**: Verify API connection
- **update_store_order**: Update an existing order


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Order Desk** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all active orders in Order Desk."

**🤖 AI Agent:**
> I've retrieved your orders. You have 15 active shipments across your channels. Notable recent orders include #1234 from Shopify and #5678 from Amazon. Which one would you like to see details for?

---

**👤 You:**
> "Show me all orders placed today and their current fulfillment status."

**🤖 AI Agent:**
> You have 23 orders placed today. 8 are in Processing status, 11 have been Shipped (tracking numbers available), 2 are On Hold awaiting payment confirmation, and 2 are in Partial Fulfillment. Total revenue today: $4,287.50. The largest order is #ORD-9847 for $892 containing 6 line items.

---

**👤 You:**
> "Check the inventory levels for SKU WIDGET-PRO-BLK and update the stock count to 250."

**🤖 AI Agent:**
> SKU WIDGET-PRO-BLK ("Widget Pro Black Edition") found. Previous stock: 47 units. I have updated the inventory count to 250 units. The item is mapped to 3 active sales channels and has a reorder point set at 25 units. Last shipment received: May 5th (200 units from supplier Acme Widgets).


## ❓ FAQ

**Q: Can my AI automatically find the details for a specific order by its ID?**
Yes! Use the `get_order` tool with the Order ID. Your agent will respond with complete metadata for the record, including customer information, items, and status in seconds.

**Q: How do I find my Order Desk Store ID and API Key?**
Log in to your Order Desk store, navigate to **Store Settings** > **API**, and you will find your unique Store ID and generate your secret API key there.

**Q: Can I update inventory levels using the AI?**
Absolutely. Use the `update_inventory` tool. Provide the Inventory Item ID and the new stock quantity, and the agent will sync the update to Order Desk immediately.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/order-desk-alternative](https://vinkius.com/mcp/order-desk-alternative)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Order Desk** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `order-desk-alternative` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Order Desk** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "order-desk-alternative": {
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
