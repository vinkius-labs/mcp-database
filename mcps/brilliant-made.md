# Brilliant Made MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/brilliant-made)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/brilliant-made-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/brilliant-made-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Manage your corporate swag via Brilliant Made — track orders, browse products, and monitor inventory directly from any AI agent.

## Description
Connect your **Brilliant Made** account to any AI agent and orchestrate your corporate swag, gifting campaigns, and inventory management through natural conversation.

### What you can do

- **Order Oversight** — List and retrieve detailed metadata for all swag orders and monitor fulfillment progress.
- **Product Discovery** — Browse your custom storefront catalog and retrieve specifications for individual product variants.
- **Inventory Tracking** — Monitor real-time stock levels across your entire product range to ensure availability for campaigns.
- **Gift Card Management** — List, create, and assign storefront gift cards to reward employees or clients.
- **Operational Control** — Cancel pending orders directly from your workspace if needed.

### How it works

1. Subscribe to this server
2. Enter your Brilliant Made API Key
3. Start managing your corporate swag from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Office Managers & HR** — quickly order swag for new hires or check stock for upcoming events without manual dashboard work.
- **Marketing Teams** — monitor gifting campaign fulfillment and product availability straight from their workflow tools.
- **Ops Leads** — verify order statuses and inventory levels using natural language.


## Available Tools
- **cancel_order**: Cancel an existing swag order
- **create_gift_card**: Create a new storefront gift card
- **create_order**: Place a new swag order
- **get_inventory_status**: Retrieve real-time inventory status for all products
- **get_order**: Get details of a specific order
- **get_product_variant**: Get details of a specific product variant
- **list_fulfillment_orders**: List all fulfillment orders
- **list_gift_cards**: List all storefront gift cards
- **list_orders**: List all swag orders
- **list_products**: List all available products in the store


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Brilliant Made** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all my recent swag orders in Brilliant Made."

**🤖 AI Agent:**
> I've retrieved your orders. You have 3 recent orders, including Order #1001 (Status: Shipped) and Order #1005 (Status: Processing). Would you like to see the tracking info for any of them?

---

**👤 You:**
> "Show the current inventory status for all products."

**🤖 AI Agent:**
> Retrieving inventory... You have 'Branded Hoodie' (Stock: 150), 'Custom Mug' (Stock: 80), and 'Logo Sticker Pack' (Stock: 500) available.

---

**👤 You:**
> "Get details for product variant var_123."

**🤖 AI Agent:**
> Variant var_123 is the 'Blue / Large' version of the Branded Hoodie. Its current price is $45.00 and it is in stock.


## Installation & Usage

To install and use the **Brilliant Made** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/brilliant-made](https://vinkius.com/mcp/brilliant-made)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
