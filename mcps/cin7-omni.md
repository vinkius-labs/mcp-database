# Cin7 Omni MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/cin7-omni)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/cin7-omni-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/cin7-omni-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [ecommerce](../categories/ecommerce.md)

Manage inventory and multi-channel orders via Cin7 Omni — track stock, monitor sales, and manage contacts directly from any AI agent.

## Description
Connect your **Cin7 Omni** account to any AI agent and take full control of your inventory management and order fulfillment through natural conversation. Streamline how you manage stock across multiple warehouses and sales channels.

### What you can do

- **Inventory Oversight** — List and retrieve details for all products in your catalog natively
- **Stock Intelligence** — Access real-time stock levels across all locations and for specific SKUs flawlessly
- **Order Management** — List and retrieve details for sales orders and purchase orders flawlessly
- **Contact Logistics** — Access customer and supplier information to maintain seamless relationships securely
- **Distribution Tracking** — Monitor inbound and outbound shipments to ensure timely delivery flawlessly
- **Commerce Insights** — Retrieve detailed product metadata and order statuses directly within your workspace

### How it works

1. Subscribe to this server
2. Enter your Cin7 API Username and API Key (obtained from Settings > API v1)
3. Start managing your inventory from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Inventory Managers** — monitor stock levels and inbound shipments using natural language
- **Warehouse Operations** — verify product locations and order statuses without opening the complex ERP
- **Purchasing Teams** — quickly look up supplier info and purchase order history straight from their chat interface
- **E-commerce Teams** — verify product details and multi-channel sales status


## Available Tools
- **get_sku_stock_level**: Get current stock level for a specific product ID
- **get_product_details**: Get detailed information for a specific product
- **get_sales_order_details**: Get detailed information for a specific sales order
- **list_cin7_contacts**: List customer and supplier contacts
- **list_cin7_products**: List products in the inventory
- **list_purchase_orders**: List purchase orders and inbound shipments
- **list_sales_orders**: List sales orders and their status
- **list_stock_levels**: List current stock levels for all products


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Cin7 Omni** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List my last 5 sales orders in Cin7."

**🤖 AI Agent:**
> Retrieving your recent sales orders... I found 5 items: Order #SO-100 (Dispatched), #SO-101 (Fully Invoiced), and 3 others. Would you like the full details for any of these?

---

**👤 You:**
> "What is the stock level for product ID 12345?"

**🤖 AI Agent:**
> Checking stock for product 12345... You have 150 units available across all locations. 100 in Main Warehouse and 50 in West Coast DC.

---

**👤 You:**
> "Search for products with 'Shirt' in their name."

**🤖 AI Agent:**
> Searching for 'Shirt'... I found 3 products: 'Blue Cotton Shirt', 'Red Polo Shirt', and 'White Formal Shirt'. Which one would you like more information on?


## Installation & Usage

To install and use the **Cin7 Omni** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/cin7-omni](https://vinkius.com/mcp/cin7-omni)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
