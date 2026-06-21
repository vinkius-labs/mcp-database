# Order Desk MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/order-desk-alternative)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/order-desk-alternative-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/order-desk-alternative-mcp)
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


## Installation & Usage

To install and use the **Order Desk** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/order-desk-alternative](https://vinkius.com/mcp/order-desk-alternative)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
