# Fieldfolio MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/fieldfolio)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/fieldfolio-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/fieldfolio-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [e-commerce](../categories/e-commerce.md)

Connect Fieldfolio to automate wholesale management — manage products, orders, and inventory directly from your AI agent.

## Description
Fieldfolio is a leading B2B wholesale marketplace. This MCP server allows your AI agent to interact with your Fieldfolio seller account flawlessly.

### Key Features
- **Product Orchestration** — List all items in your wholesale catalog and fetch detailed metadata for specific products natively.
- **Order Management** — Retrieve and inspect wholesale orders to stay updated on fulfillment and sales flawlessly.
- **Inventory Intelligence** — Query real-time stock levels and update inventory quantities directly from the agent flawlessy.
- **Customer CRM** — Access retail customer profiles and order history to personalize business relationships flawlessly.
- **Catalog Search** — Search your entire wholesale catalog by keyword to quickly find specific items flawlessly.
- **Webhook Auditing** — List active webhooks to ensure your third-party integrations are synchronized flawlessly.

### How it works
1. Subscribe to this server
2. Enter your Fieldfolio API Token (found in Settings > Integrations)
3. Start managing your wholesale business from Claude, Cursor, or any MCP-compatible client

### Who is this for?
- **Wholesale Managers** — monitor sales trends and order statuses without manual dashboard exports
- **Operations Teams** — sync product data and inventory levels directly from your chat workflow
- **Sales Reps** — quickly look up product availability and customer history through simple natural language queries


## Available Tools
- **get_customer**: Get details for a specific retail customer
- **get_me**: Get details for the authorized seller account
- **get_order**: Get details for a specific wholesale order
- **get_product**: Get details for a specific product
- **list_categories**: List all product categories
- **list_customers**: List all retail customers
- **list_inventory**: List inventory levels for all products
- **list_orders**: List all wholesale orders
- **list_products**: List all products in your wholesale catalog
- **list_webhooks**: List all configured webhooks
- **search_catalog**: Search the wholesale catalog by keyword
- **update_inventory**: Update inventory quantity for a specific product


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Fieldfolio** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List my active wholesale orders."

**🤖 AI Agent:**
> I've retrieved your recent orders. You have 12 orders currently pending, including 'Retailer A' (Order #1025) and 'Store B' (Order #1026). Would you like to see the item breakdown for any of these?

---

**👤 You:**
> "Check the inventory level for 'Summer T-Shirt'."

**🤖 AI Agent:**
> Inspecting inventory... 'Summer T-Shirt' (SKU: ST-101) currently has 45 units in stock. Shall I alert you if it drops below 10?

---

**👤 You:**
> "Search the catalog for 'Ceramic Vases'."

**🤖 AI Agent:**
> Searching catalog... I found 3 matching items: 'Minimalist Ceramic Vase', 'Blue Glazed Vase', and 'Rustic Pot'. Which one would you like more details on?


## Installation & Usage

To install and use the **Fieldfolio** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/fieldfolio](https://vinkius.com/mcp/fieldfolio)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
