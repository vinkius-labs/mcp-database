# Veeqo MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/veeqo)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/veeqo-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/veeqo-mcp)
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


## Installation & Usage

To install and use the **Veeqo** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/veeqo](https://vinkius.com/mcp/veeqo)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
