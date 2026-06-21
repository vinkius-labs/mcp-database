# Zoho Inventory MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/zoho-inventory)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/zoho-inventory-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/zoho-inventory-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [ecommerce](../categories/ecommerce.md)

Manage inventory items, sales orders, and stock levels via the Zoho Inventory API.

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


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Zoho Inventory** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all organizations in my Zoho Inventory account."

**🤖 AI Agent:**
> I've retrieved your organizations. You have 2 entities: 'Main Store (ID: 123456)' and 'Secondary Warehouse (ID: 789012)'. Which one would you like to access?

---

**👤 You:**
> "Show the stock level for 'Professional Camera'."

**🤖 AI Agent:**
> For 'Professional Camera' (ID: 101) in organization 123456, there are currently 45 units available in stock.

---

**👤 You:**
> "List my 5 most recent sales orders in organization '123456'."

**🤖 AI Agent:**
> I've fetched your latest sales orders. Recent transactions include Order #SO-001 for 'Alice Smith' ($1,500.00) and Order #SO-002 for 'Bob Jones' ($850.50).


## Installation & Usage

To install and use the **Zoho Inventory** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/zoho-inventory](https://vinkius.com/mcp/zoho-inventory)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
