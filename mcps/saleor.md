# Saleor MCP Server

Connect your AI to your headless Saleor e-commerce store. Seamlessly manage products, audit recent orders, and assist customers natively through your chat.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/saleor)

## Overview
**Category:** loved-by-devs
**Tools Count:** 10

## Description
Empower your conversational AI with deep access to **Saleor**, the highly scalable, headless GraphQL-first e-commerce engine designed around high performance experiences. Connect your environment to actively manage your daily retail store operations, inspect products, or troubleshoot customer inquiries natively from chat.

### What you can do

- **Inventory & Catalogs** — Quickly inspect your store's entire directory (`list_products`). Retrieve detailed specifics such as available variants, pricing, and precise stock configurations per individual product ID (`get_product`).
- **Category Orchestration** — Browse how your catalog is organized internally by fetching collections (`list_collections`) and sub-categories (`list_categories`) without toggling through web dashboards.
- **Order Fulfillment Auditing** — Easily review a list of the latest purchases happening on your platform (`list_orders`) and quickly grab comprehensive snapshots of individual receipts, line items, or billing addresses (`get_order`).
- **Customer Assistance** — Query your database to find registered profiles globally (`list_customers`) or drill down into specific shopper's order details and status natively (`get_customer`).
- **Architecture Inspection** — Inspect high-level configuration such as default currencies and active regions by utilizing `list_channels` or retrieving global details via `get_shop_info`.

### How it works

1. Authorize the Saleor mapping tools within your workspace integrations.
2. Access your main Saleor backend dashboard.
3. Generate a dedicated internal App Token containing adequate reading/managing authorizations.
4. Enter the Saleor Cloud GraphQL API Endpoint and the generated access token simultaneously into the connection securely.
5. Ask the AI: "Find out order specifics and shipping details for order number '334'."


## Available Tools
- **get_customer**: Retrieves profile information and order history for a specific customer
- **get_order**: Retrieves details for a specific order
- **get_product**: Retrieves details for a specific product by ID
- **get_shop_info**: Retrieves global shop configuration
- **list_categories**: Lists all product categories
- **list_channels**: Lists all configured sales channels
- **list_collections**: Lists all product collections
- **list_customers**: Lists all customers/users registered in the shop
- **list_orders**: Lists recent customer orders
- **list_products**: Lists all products in the Saleor store


## Installation & Usage

To install and use the **Saleor** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/saleor](https://vinkius.com/mcp/saleor)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
