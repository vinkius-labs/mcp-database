# OpenCart MCP Server

Connect your OpenCart store to AI agents — browse products, manage orders, track customers, and update fulfillment status through natural conversation.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/opencart)

## Overview
**Category:** business-operations
**Tools Count:** 10

## Description
Turn your **OpenCart** e-commerce backend into an AI-powered command center. Browse your product catalog, check order details, look up customers, and push status updates — without logging into the admin panel.

### What you can do

- **Product Catalog** — List all products or fetch a specific product with pricing, stock status, SEO tags, and linked categories
- **Order Management** — Browse orders with totals, payment methods, and shipping addresses. Get detailed line-items for any order by ID
- **Order Status Updates** — Push status transitions (Processing, Shipped, Complete, Cancelled) with comments via the order history endpoint
- **Customer Profiles** — List registered customers or fetch full details including addresses, custom fields, and newsletter status
- **Categories** — View your product category hierarchy and navigation structure
- **Cart Inspection** — Check the current API session cart contents for programmatic checkout workflows

### How it works

1. Subscribe to this server
2. Enter your OpenCart Store URL, API Username, and API Key
3. Start managing your store from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Store owners** — check daily orders and revenue without opening the admin panel
- **Support teams** — look up customer orders instantly during live chat support
- **Fulfillment ops** — update order statuses in bulk by talking to your AI agent instead of clicking through forms


## Available Tools
- **list_products**: Fetches active products, retrieving metadata such as prices, stock status, and basic SEO tags mapped inside the OpenCart product repository.

List OpenCart products using the native OpenCart API
- **get_product**: Get OpenCart product by ID. Returns full details
- **list_orders**: List OpenCart orders using the native API
- **get_order**: Get OpenCart order details by explicit ID
- **get_order_history**: g., Pending, Processing, Shipped). Use to verify tracking logic or administrative fulfillment changes.

Get OpenCart order status history by ID
- **list_customers**: List OpenCart registered customers
- **get_customer**: Get OpenCart customer full details by explicit ID
- **list_categories**: List OpenCart product category schemas
- **add_order_history**: Push updates like marking a shipment Complete or Canceled.

Add OpenCart order history / mutate order active status
- **get_cart**: Primarily used to verify product mapping prior to custom order creation logic.

Get current API session cart contents in OpenCart


## Installation & Usage

To install and use the **OpenCart** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/opencart](https://vinkius.com/mcp/opencart)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
