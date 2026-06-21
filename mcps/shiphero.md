# ShipHero MCP Server

Manage e-commerce logistics via ShipHero — track orders, monitor inventory levels, and handle warehouse movements directly from your AI agent.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/shiphero)

## Overview
**Category:** ecommerce
**Tools Count:** 8

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


## Installation & Usage

To install and use the **ShipHero** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/shiphero](https://vinkius.com/mcp/shiphero)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
