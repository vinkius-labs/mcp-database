# Commerce.js MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/commercejs)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/commercejs-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/commercejs-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [ecommerce](../categories/ecommerce.md)

Manage your e-commerce store via Commerce.js — list products, manage carts, and handle orders directly from any AI agent.

## Description
Connect your **Commerce.js** (Chec) account to any AI agent and take full control of your e-commerce operations through natural conversation.

### What you can do

- **Product Catalog** — List all products, filter by category, and fetch detailed metadata for specific items using IDs.
- **Cart Management** — Create new carts, add products with specific quantities, and update line items seamlessly.
- **Checkout Flow** — Generate checkout tokens from carts to prepare for secure transactions and capture orders with customer details.
- **Order Processing** — List recent orders, retrieve specific order details, and manage fulfillment data.
- **Category Organization** — Browse store categories to understand your product hierarchy and improve navigation.

### How it works

1. Subscribe to this server
2. Enter your Chec Public Key and Secret Key
3. Start managing your store from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Store Managers** — quickly check inventory levels and order statuses without logging into the dashboard
- **Developers** — test cart and checkout logic directly from the terminal or code editor
- **Support Teams** — look up customer order details instantly to provide faster assistance


## Available Tools
- **add_to_cart**: Add an item to a cart
- **capture_order**: Capture an order
- **create_cart**: Create or retrieve a cart
- **generate_checkout_token**: Generate a checkout token
- **get_order**: Requires Secret Key.

Retrieve a specific order
- **get_product**: Retrieve a specific product
- **list_categories**: List categories
- **list_orders**: Requires Secret Key.

List orders
- **list_products**: Can be filtered by category or paginated.

List products in the store
- **update_cart_item**: Update a cart item


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Commerce.js** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List the first 5 products in my store."

**🤖 AI Agent:**
> I've retrieved your products. Your top items include 'Wireless Headphones' (prod_123) and 'Smart Watch' (prod_456). Would you like more details on any of these?

---

**👤 You:**
> "Create a cart and add 2 units of product prod_Q123."

**🤖 AI Agent:**
> Cart created successfully (ID: cart_abc123). I have added 2 units of 'Organic Coffee Beans' to it. The current subtotal is $30.00.

---

**👤 You:**
> "Show me the details for order ord_987."

**🤖 AI Agent:**
> Order ord_987 was placed by John Doe. It contains 1x 'Gaming Mouse' and is currently marked as 'Fulfilled'. Shipping was handled via Standard Delivery.


## Installation & Usage

To install and use the **Commerce.js** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/commercejs](https://vinkius.com/mcp/commercejs)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
