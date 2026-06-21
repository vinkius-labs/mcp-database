# BigCommerce MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/bigcommerce-alternative)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/bigcommerce-alternative-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/bigcommerce-alternative-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [industry-titans](../categories/industry-titans.md)

Manage your online store with product catalogs, order fulfillment, and customer data for high-volume e-commerce operations.

## Description
Connect your **BigCommerce** store to any AI agent and take full control of your enterprise e-commerce operations and storefront management through natural conversation.

### What you can do

- **Catalog Orchestration** — List and manage your entire product directory programmatically, retrieving detailed high-fidelity metadata for items, variants, and stock levels
- **Order Lifecycle Management** — Monitor real-time transaction history and retrieve detailed order profiles (V2 API), including billing and fulfillment status directly through your agent
- **Customer Intelligence** — Access your complete directory of shoppers and retrieve high-fidelity profile metadata to maintain perfectly coordinated relationship ecosystems
- **Storefront Architecture** — Manage product categories and brands programmatically to ensure your digital catalog is perfectly organized and up-to-date
- **Infrastructure Monitoring** — Access store-level configuration including currency settings, language preferences, and account status for instant operational reporting

### How it works

1. Subscribe to this server
2. Retrieve your **Access Token**, **Store Hash**, and **Client ID** from your BigCommerce dashboard (Settings > API Accounts)
3. Start orchestrating your digital commerce from Claude, Cursor, or any MCP client

No more manual toggling between storefront tabs or digging through complex order tables. Your AI acts as your dedicated store manager and commerce architect.

### Who is this for?

- **Store Managers** — instantly retrieve product summaries and monitor order statuses using natural language commands
- **Inventory Coordinators** — track stock levels and manage product variants without leaving your creative workspace
- **Marketing Leads** — automate the analysis of customer purchase patterns and catalog growth through simple AI queries


## Available Tools
- **get_customer_details**: Get details for a customer
- **get_order_details**: Get details for an order
- **get_product_details**: Get metadata for a product
- **get_store_info**: Get store configuration
- **list_catalog_brands**: List product brands
- **list_catalog_categories**: List product categories
- **list_customers**: List store customers
- **list_orders**: List recent store orders
- **list_products**: Supports filtering by name or brand.

List your BigCommerce products


## 💬 Prompt Examples

Here are some examples of how you can interact with the **BigCommerce** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all products in my BigCommerce store and their current stock levels."

**🤖 AI Agent:**
> I've retrieved your catalog. You currently have 150 products, including 'Enterprise Laptop' (Stock: 45) and 'Ergonomic Chair'. Would you like the detailed variant metadata for any of these?

---

**👤 You:**
> "Show the last 5 orders and their fulfillment status."

**🤖 AI Agent:**
> Fetching transactions... Your last 5 orders include 3 'Shipped' status and 2 'Pending' (Order IDs: 1024, 1025). Shall I retrieve the high-fidelity billing info for the pending ones?

---

**👤 You:**
> "Get the full profile for customer ID '123'."

**🤖 AI Agent:**
> Retrieving profile... John Doe (ID: 123) is a registered shopper since 2024 with 15 total orders. He belongs to the 'VIP' customer group. Need help checking his historical transaction metadata?


## Installation & Usage

To install and use the **BigCommerce** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/bigcommerce-alternative](https://vinkius.com/mcp/bigcommerce-alternative)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
