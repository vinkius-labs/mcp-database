# ShipHero MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/shiphero)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/shiphero-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/shiphero-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [ecommerce](../categories/ecommerce.md)

Manage e-commerce logistics via ShipHero — track orders, monitor inventory levels, and handle warehouse movements directly from your AI agent.

## Description
Connect your **ShipHero** account to any AI agent to streamline your warehouse and fulfillment operations through natural language.

### What you can do

- **Order Management** — List recent orders and create new ones with full shipping and line item details.
- **Inventory Control** — Check real-time stock levels by SKU, track history of inventory changes, and add or remove stock instantly.
- **Bulk Operations** — Sync inventory levels in bulk using CSV URLs for rapid warehouse updates.
- **Product Insights** — Retrieve deep metadata for products, including warehouse-specific availability and legacy ID conversion.
- **Automation** — Register webhooks to stay updated on inventory changes or order statuses.

### How it works

1. Subscribe to this server
2. Enter your ShipHero Access Token
3. Start managing your logistics from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **E-commerce Managers** — monitor fulfillment health and stock levels without leaving your workspace
- **Operations Teams** — quickly adjust inventory and track movement history during audits
- **Developers** — integrate warehouse data into your workflow and test webhooks via simple prompts


## Available Tools
- **add_inventory**: Add or remove inventory for a SKU
- **create_order**: Create a new order in ShipHero
- **create_webhook**: Register a new webhook
- **get_uuid**: Get UUID from a legacy numeric ID
- **list_inventory_changes**: List inventory changes for a SKU
- **list_orders**: List ShipHero orders
- **get_product**: Get product details by SKU
- **sync_inventory**: Bulk sync inventory via CSV URL


## 💬 Prompt Examples

Here are some examples of how you can interact with the **ShipHero** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List the 10 most recent orders from my primary warehouse."

**🤖 AI Agent:**
> I've retrieved the latest orders. You have 10 recent records, including Order #SH-1029 (Status: Pending) and Order #SH-1030 (Status: Fulfilled). Would you like details on a specific one?

---

**👤 You:**
> "Check the current inventory level and warehouse details for SKU 'BLUE-SHIRT-L'."

**🤖 AI Agent:**
> For SKU 'BLUE-SHIRT-L', I found 45 units available in Warehouse A and 12 units in Warehouse B. The total on-hand inventory is 57 units.

---

**👤 You:**
> "Add 25 units to SKU 'GIFT-WRAP' in warehouse 'WH-99' because of a new shipment."

**🤖 AI Agent:**
> Successfully updated inventory for 'GIFT-WRAP'. Added 25 units to warehouse 'WH-99'. The new balance has been synchronized.


## Installation & Usage

To install and use the **ShipHero** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/shiphero](https://vinkius.com/mcp/shiphero)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
