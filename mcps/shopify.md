# Shopify MCP Server

Manage your Shopify store via AI — list products, process orders, search customers, track inventory, and manage discounts from any agent.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/shopify)

## Overview
**Category:** industry-titans
**Tools Count:** 23

## Description
Connect your **Shopify** store to any AI agent and run your entire ecommerce operation through natural conversation.

### What you can do

- **Product Management** — List, search, and create products with variants, images, and pricing
- **Order Processing** — View all orders, inspect details with line items and shipping, close fulfilled orders
- **Customer Intelligence** — Browse customers, view profiles with purchase history, search by name or email
- **Inventory Tracking** — Check stock levels per location and variant
- **Collections & Discounts** — Browse product collections and active price rules

### How it works

1. Subscribe to this server
2. Enter your Shopify store name and Admin API access token
3. Start managing your store from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Ecommerce Managers** — instant access to orders and inventory without the dashboard
- **Customer Support** — look up orders and customer profiles in seconds
- **Marketing Teams** — manage products and discounts through AI workflows


## Available Tools
- **list_products**: Use limit to control results.

List all products in the Shopify store
- **list_inventory_levels**: Get inventory levels for a location
- **list_collections**: List product collections
- **list_price_rules**: List discount price rules
- **get_product**: Get detailed product information
- **create_product**: Returns the created product with its ID.

Create a new product in the store
- **list_orders**: Filter by status: open, closed, cancelled, any.

List orders from the store
- **get_order**: Get detailed order information
- **close_order**: Useful after manual fulfillment or resolution.

Close an existing order
- **list_customers**: List all customers
- **get_customer**: Get detailed customer profile
- **search_customers**: Use queries like "email:john@example.com" or plain text.

Search customers by name, email, or other fields
- **update_product**: Pass only the fields you want to change.

Update an existing product
- **delete_product**: This action is irreversible — the product and all its variants are permanently deleted.

Permanently delete a product
- **count_products**: Useful for inventory audits and dashboard metrics.

Get total product count
- **cancel_order**: Cannot be undone after cancellation processing.

Cancel an existing order
- **count_orders**: Filter by status: open, closed, cancelled, or any.

Get total order count
- **create_customer**: Returns the created customer record with its unique ID.

Create a new customer profile
- **list_locations**: Location IDs are required for inventory queries.

List all store locations
- **list_smart_collections**: List automated smart collections
- **list_fulfillments**: List fulfillments for an order
- **list_themes**: List store themes
- **list_pages**: ) with titles, content, and publication status.

List store pages


## Installation & Usage

To install and use the **Shopify** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/shopify](https://vinkius.com/mcp/shopify)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
