# Zoho Inventory MCP Server

Manage inventory items, sales orders, and stock levels via the Zoho Inventory API.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/zoho-inventory)

## Overview
**Category:** ecommerce
**Tools Count:** 9

## Description
Connect your **Zoho Inventory** account to any AI agent to automate your order management and stock control. This MCP server enables your agent to interact with products, sales orders, and purchase orders directly through natural language interfaces.

### What you can do

- **Inventory Oversight** — List all items in your inventory and retrieve real-time stock levels and metadata
- **Order Management** — List, retrieve, and create sales orders and purchase orders across your organizations
- **Stock Tracking** — Monitor item availability and identify stockouts before they happen
- **Bundle Visibility** — List composite items and bundles to understand your product kits and assemblies
- **Multi-Org Support** — Manage multiple business entities by providing the required organization ID for all operations

### How it works

1. Subscribe to this server
2. Enter your Zoho Client ID, Client Secret, and Data Center Domain
3. Start managing your inventory from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Inventory Managers** — Quickly check item availability and update stock notes via natural language commands
- **Warehouse Operations** — Monitor incoming and outgoing orders without opening the administrative panel
- **Developers** — Integrate real-time inventory data and order automation into your daily development workflow


## Available Tools
- **list_composite_items**: List all composite items (bundles)
- **create_new_item**: Requires a JSON body with item details (name, rate, etc.).

Add a new item to the inventory
- **create_sales_order**: Requires a JSON body with customer and line item details.

Create a new sales order
- **get_item_details**: Get details for a specific item
- **get_sales_order_details**: Get details for a specific sales order
- **list_inventory_items**: List all items in the inventory
- **list_organizations**: Use this to identify the organization ID for other calls.

List all Zoho Inventory organizations
- **list_purchase_orders**: List all purchase orders
- **list_sales_orders**: List all sales orders


## Installation & Usage

To install and use the **Zoho Inventory** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/zoho-inventory](https://vinkius.com/mcp/zoho-inventory)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
