# Cornershop MCP Server

Automate LatAm grocery deliveries via Cornershop (by Uber) — search products, manage carts, track orders, and monitor shoppers from any AI agent.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/cornershop)

## Overview
**Category:** industry-titans
**Tools Count:** 14

## Description
Connect your **Cornershop by Uber** B2B account to any AI agent and manage your last-mile grocery delivery operations through natural conversation.

### What you can do

- **Store & Product Discovery** — Search through connected retail partners (Jumbo, Lider, pharmacies), browse their aisles, and find specific SKUs with real-time pricing and availability
- **Order Creation** — Construct shopping carts dynamically and place delivery orders directly through your AI agent
- **Live Tracking** — Monitor the real-time status of your orders, from picking to delivery, including GPS tracking of the assigned Shopper
- **Order Modification** — Add or remove items from the cart while the Shopper is still in the store, without opening the mobile app
- **Shopper Communication** — Retrieve contact details for assigned Shoppers to resolve delivery issues instantly

### How it works

1. Subscribe to this server
2. Enter your Cornershop Client ID and Secret (via the B2B portal or Uber Eats Direct)
3. Start managing your grocery logistics from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Corporate Office Managers** — automate office grocery and supply runs
- **B2B Resellers** — programmatically place orders for fulfillment
- **Personal Assistants** — manage client grocery lists and track deliveries efficiently


## Available Tools
- **cancel_order**: Note: Orders can only be cancelled without penalty if the shopper hasn't started picking.

Cancel a pending order
- **create_order**: Requires a JSON string defining the cart (product IDs, quantities) and delivery address details.

Place a new delivery order
- **create_webhook**: g., shopper_assigned, order_delivered).

Create a new explicit webhook
- **get_order**: Get full details of a specific order
- **get_product**: Get details of a specific product
- **get_store**: Get details of a specific store branch
- **list_store_aisles**: List categories and aisles of a store
- **list_orders**: List your delivery orders
- **list_shoppers**: Get information about the assigned Shopper
- **list_stores**: g. Jumbo, Lider, pharmacies). Can be geographically filtered by latitude and longitude.

List available grocery stores and partners
- **list_webhooks**: List configured order webhooks
- **search_products**: Returns matching SKUs, names, current pricing, and availability.

Search for specific groceries and products
- **track_order**: Get real-time tracking for a delivery
- **update_order**: Useful for last-minute replacements or additions.

Update an active order (e.g. add/remove items)


## Installation & Usage

To install and use the **Cornershop** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/cornershop](https://vinkius.com/mcp/cornershop)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
