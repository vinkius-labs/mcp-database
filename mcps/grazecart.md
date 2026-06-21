# GrazeCart MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/grazecart)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/grazecart-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/grazecart-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [ecommerce](../categories/ecommerce.md)

Manage your GrazeCart store — track orders, update inventory, and manage customers directly via AI.

## Description
Connect your **GrazeCart** ecommerce account to any AI agent and take control of your perishable food business operations through natural conversation.

### What you can do

- **Order Management** — List recent orders and resolve specific order details including status and totals natively
- **Fulfillment Operations** — Update order statuses and trigger payment charges for pending orders flawlessly
- **Inventory Control** — Browse your product catalog and update inventory counts for variants to prevent overselling synchronously
- **Customer Oversight** — Search and retrieve customer profiles, including their order history and contact information natively
- **Logistics & Pickup** — List active pickup locations and delivery zones to assist with logistics planning securely

### How it works

1. Subscribe to this server
2. Enter your GrazeCart Store URL and API Token (found in your Admin Panel under Profile > API Token)
3. Start managing your farm-to-table business from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Farm Owners & Managers** — quickly check daily orders and update stock levels for fresh products without manual dashboard navigation
- **Operations Teams** — manage pickup logistics and verify customer details during the fulfillment process
- **Customer Support** — look up order histories and update customer information through simple conversational queries


## Available Tools
- **charge_order**: Trigger a payment charge for an order
- **create_customer**: Create a new customer profile
- **get_customer**: Get profile details for a specific customer
- **get_order**: Get details for a specific order
- **get_product**: Get details for a specific product
- **list_customers**: List all customers registered in the store
- **list_delivery_zones**: List configured delivery zones
- **list_orders**: List all orders from the GrazeCart store
- **list_pickup_locations**: List all active pickup locations for the store
- **list_products**: List all products in the catalog
- **update_inventory**: Update inventory counts for a product
- **update_order**: Update an existing order


## 💬 Prompt Examples

Here are some examples of how you can interact with the **GrazeCart** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List my recent orders in GrazeCart"

**🤖 AI Agent:**
> Retrieving your orders... I found 3 recent orders: #1001 ($145.00), #1002 ($82.50), and #1003 ($210.00). Would you like to see the details for the latest order?

---

**👤 You:**
> "Check the inventory for 'Grass-fed Ribeye'"

**🤖 AI Agent:**
> Checking products... 'Grass-fed Ribeye' (ID: 452) has 12 units currently available in stock. There are also 5 units reserved for pending orders.

---

**👤 You:**
> "Process the payment for order #1001"

**🤖 AI Agent:**
> Processing payment... Success! I've triggered the payment charge for Order #1001. The transaction status is now 'Success'.


## Installation & Usage

To install and use the **GrazeCart** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/grazecart](https://vinkius.com/mcp/grazecart)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
