# ManoMano (Home Improvement Marketplace) MCP Server

Manage your ManoMano seller account — update offer prices, track orders, and audit fulfillment stock.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/manomano-home-improvement-marketplace)

## Overview
**Category:** supply-chain
**Tools Count:** 11

## Description
Connect your **ManoMano Seller** account to any AI agent and take full control of your marketplace operations and home improvement catalog through natural conversation.

### What you can do

- **Offer Orchestration** — List all published offers and retrieve detailed metadata including current stock, VAT-included pricing, and SKUs directly from your agent
- **Live Catalog Updates** — Safely modify VAT-included prices and update available inventory quantities for specific offers to maintain competitive market positioning
- **Order Management** — List all received orders and retrieve complete representations including customer details, delivery addresses, and individual line items securely
- **Logistical Control** — Acknowledge and accept pending orders or transition them to 'Shipped' status by supplying carrier-specific tracking numbers and carrier names
- **Fulfillment Visibility** — Monitor stock levels maintained through ManoFulfillment (ManoMano warehouse) to ensure logistical accuracy and product availability
- **Taxonomy Discovery** — Enumerate root category lists and registered brands to guide product mapping and architectural catalog taxonomy natively

### How it works

1. Subscribe to this server
2. Enter your ManoMano API Key
3. Start managing your marketplace presence from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Marketplace Sellers** — manage pricing and stock levels through natural conversation without manual Seller Central exports
- **E-commerce Managers** — monitor order flow and retrieve customer delivery data directly from your workspace for rapid auditing
- **Logistics Teams** — update shipping statuses and audit ManoFulfillment stock levels efficiently to maintain high fulfillment standards


## Available Tools
- **list_offers**: List all published offers on ManoMano
- **get_offer**: Get details for a specific ManoMano offer (price, stock, SKU)
- **update_offer_price**: This is a reversible operation.

Change the price of a specific offer
- **update_offer_stock**: This is a reversible operation.

Update the available stock count for a specific offer
- **list_orders**: List all received ManoMano orders
- **get_order**: Get full order details including customer, addresses, and order lines
- **accept_order**: Accept a pending ManoMano order
- **ship_order**: Ship an order by supplying a valid tracking number and carrier
- **list_categories**: List ManoMano catalog categories
- **list_brands**: List available brands on ManoMano
- **list_fulfillment_stock**: Check stock maintained through ManoFulfillment (ManoMano warehouse)


## Installation & Usage

To install and use the **ManoMano (Home Improvement Marketplace)** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/manomano-home-improvement-marketplace](https://vinkius.com/mcp/manomano-home-improvement-marketplace)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
