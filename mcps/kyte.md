# Kyte MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/kyte)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/kyte-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/kyte-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [ecommerce](../categories/ecommerce.md)

Manage your POS store — list products, track orders, and audit inventory.

## Description
Connect your AI agent to **Kyte**, the mobile-first POS system designed for small businesses to manage inventory and sales anywhere.

### Key Features

- **Catalog Auditing** — List all products and categories to maintain your digital storefront
- **Order Tracking** — Access and monitor sales orders, status updates, and customer history
- **Inventory Management** — Check stock levels in real-time to prevent sell-outs
- **Customer CRM** — View profiles and transaction history for your store's buyers
- **Financial Visibility** — List transactions and casher logs to monitor store performance

### Simple Setup

1. Subscribe to this server
2. Log in to Kyte, go to **Settings** > **API**, and generate an API Key
3. Enter your key in the configuration panel
4. Start managing your store via natural language


## Available Tools
- **list_kyte_products**: Returns product IDs, names, and current prices.

List all products in the store
- **get_product_details**: Get details for a specific product
- **list_kyte_orders**: Use this to audit recent transactions and delivery statuses.

List recent store orders
- **get_order_details**: Get details for a specific order
- **list_kyte_customers**: List store customers
- **get_customer_profile**: Get details for a specific customer
- **list_product_categories**: List product categories
- **get_inventory_status**: Check current inventory levels
- **list_financial_transactions**: List financial transactions
- **get_kyte_store_status**: Get current store operational status


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Kyte** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all products in my Kyte store"

**🤖 AI Agent:**
> I've retrieved your product catalog. You have 25 items across 3 categories. Notable products include 'Organic Coffee' ($15.00) and 'Ceramic Mug' ($12.50). Would you like to check inventory levels for these?

---

**👤 You:**
> "Show the last 5 orders"

**🤖 AI Agent:**
> Retrieving recent sales… The last 5 orders total $350.50. 3 are 'Completed', 1 is 'Pending Payment', and 1 is 'Cancelled'. Would you like the details for the pending order?

---

**👤 You:**
> "Which products are low on stock?"

**🤖 AI Agent:**
> Checking inventory… 2 products are below your warning level: 'Artisanal Honey' (2 left) and 'Handmade Soap' (0 left). Should I list these for your next supplier order?


## Installation & Usage

To install and use the **Kyte** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/kyte](https://vinkius.com/mcp/kyte)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
