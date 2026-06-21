# Megaventory MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/megaventory)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/megaventory-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/megaventory-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [supply-chain](../categories/supply-chain.md)

Inventory and order management via Megaventory — track products, stock levels, and orders.

## Description
Connect your **Megaventory** account to any AI agent and take full control of your inventory management and order fulfillment through natural conversation.

### What you can do

- **Inventory Management** — List all products, search by description, and fetch detailed SKU metadata
- **Stock Tracking** — Retrieve real-time stock levels across all configured inventory locations
- **Order Orchestration** — List and inspect sales orders and purchase orders with full status visibility
- **Entity Management** — Manage your directory of suppliers and clients directly from your agent
- **Warehouse Oversight** — Enumerate active inventory locations and their specific configurations

### How it works

1. Subscribe to this server
2. Enter your Megaventory API Key
3. Start managing your inventory from Claude, Cursor, or any MCP-compatible client


## Available Tools
- **get_product**: Get details for a specific product SKU
- **get_purchase_order**: Get details for a specific purchase order
- **get_sales_order**: Get details for a specific sales order
- **get_product_stock**: Get stock levels for a product SKU
- **list_suppliers_clients**: List all suppliers and clients
- **list_inventory_locations**: List all inventory locations
- **list_products**: List all products
- **list_purchase_orders**: List all purchase orders
- **list_sales_orders**: List all sales orders
- **search_products**: Search for products by description


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Megaventory** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all products in my Megaventory account."

**🤖 AI Agent:**
> Retrieving products... I found several items including 'Standard Widget' (SKU: WID-001) and 'Premium Gadget' (SKU: GAD-999).

---

**👤 You:**
> "What is the stock level for SKU 'WID-001'?"

**🤖 AI Agent:**
> Checking stock levels... SKU 'WID-001' has 150 units available across your 3 inventory locations.

---

**👤 You:**
> "Show the last 5 sales orders."

**🤖 AI Agent:**
> Querying sales orders... I found your most recent orders, including SO-12345 for Client 'TechCorp' and SO-12344 for 'Global Solutions'.


## Installation & Usage

To install and use the **Megaventory** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/megaventory](https://vinkius.com/mcp/megaventory)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
