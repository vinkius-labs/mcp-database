# Boloo (Bol.com Retailer) MCP Server

Manage your bol.com store via the Retailer API — track orders, update stock, and manage offers directly from any AI agent.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/boloo-bolcom-retailer)

## Overview
**Category:** ecommerce
**Tools Count:** 10

## Description
Connect your **bol.com Retailer** account to any AI agent and orchestrate your e-commerce operations through natural conversation.

### What you can do

- **Order Oversight** — List open and handled orders, and retrieve detailed metadata for individual order items.
- **Inventory Management** — Update stock levels and prices for your offers in real-time to maintain accuracy.
- **Offer Coordination** — List and inspect all active product offers in your Boloo catalog.
- **Logistics Control** — Confirm shipments for order items and manage cancellations with valid reason codes.
- **Product Intelligence** — Retrieve global product details using EAN codes from the bol.com public catalog.
- **Integration Monitoring** — List configured webhook subscriptions to verify your event-driven data flow.

### How it works

1. Subscribe to this server
2. Enter your bol.com Client ID and Client Secret
3. Start managing your Dutch e-commerce business from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Retailers & Sellers** — quickly check for new orders and update inventory without logging into the seller dashboard.
- **Operations Managers** — monitor shipment statuses and offer performance straight from their workflow tools.
- **Developers** — verify API interactions and stock syncs using natural language.


## Available Tools
- **cancel_order_item**: Requires a valid reason code.

Cancel an order item
- **get_offer**: Get details of a specific offer
- **get_order**: Get details of a specific order
- **get_product_details**: com catalog.

Get global product info by EAN
- **list_offers**: List all product offers
- **list_orders**: Default is OPEN.

List all open or handled orders
- **list_subscriptions**: List event subscriptions (webhooks)
- **ship_order_item**: Confirm shipment of an order item
- **update_offer_price**: Update the price for an offer
- **update_offer_stock**: Update the stock level for an offer


## Installation & Usage

To install and use the **Boloo (Bol.com Retailer)** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/boloo-bolcom-retailer](https://vinkius.com/mcp/boloo-bolcom-retailer)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
