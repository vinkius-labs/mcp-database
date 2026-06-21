# LeafLink MCP Server

Manage cannabis wholesale orders, products, and inventory via the LeafLink API.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/leaflink)

## Overview
**Category:** ecommerce
**Tools Count:** 9

## Description
Connect your **LeafLink** account to any AI agent to automate your cannabis wholesale operations. This MCP server enables your agent to manage product listings, monitor real-time inventory, and track received orders directly from natural language.

### What you can do

- **Order Oversight** — List and retrieve detailed information for all wholesale orders received from buyers
- **Inventory Visibility** — Get real-time stock levels and availability for your entire product catalog
- **Catalog Management** — List, retrieve, create, and update products including pricing and metadata
- **Status Transitions** — Move orders through their lifecycle (accept, fulfill, cancel) via simple commands
- **Partner Tracking** — List registered brands and buyers to maintain clear visibility of your wholesale network

### How it works

1. Subscribe to this server
2. Enter your LeafLink API Key (JWT Bearer Token)
3. Start managing your wholesale business from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Wholesale Managers** — Monitor incoming orders and update product availability without opening the dashboard
- **Operations Teams** — Automate inventory updates and order fulfillment workflows via natural language
- **Sales Directors** — Quickly query brand catalogs and buyer information during planning sessions


## Available Tools
- **list_wholesale_brands**: List all brands in your account
- **create_new_product**: Requires a JSON body with product details.

Add a new product to your wholesale catalog
- **list_wholesale_customers**: List all buyers and customers
- **get_order_details**: Get details for a specific order
- **get_product_details**: Get details for a specific product
- **list_received_orders**: List all wholesale orders received
- **list_wholesale_products**: List all products available in your inventory
- **update_order_status**: g., accept, fulfill, cancel, reject).

Transition an order through its lifecycle
- **update_product_inventory**: Update inventory level for a specific product


## Installation & Usage

To install and use the **LeafLink** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/leaflink](https://vinkius.com/mcp/leaflink)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
