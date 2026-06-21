# Fizzpa MCP Server

Market your restaurant or food business with digital menus, online ordering integration, and customer engagement tools.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/fizzpa)

## Overview
**Category:** ecommerce
**Tools Count:** 12

## Description
Connect your **Fizzpa** account to any AI agent and take full control of your e-commerce fulfillment, order management, and warehouse workflows through natural conversation.

### What you can do

- **Order Orchestration** — List and manage customer orders programmatically, including retrieving detailed line items and updating fulfillment statuses
- **Label & Logistics** — Programmatically generate shipping labels and retrieve direct print URLs (PDF/Image) to streamline your shipping operations
- **Inventory Intelligence** — Monitor real-time stock levels across your product catalog and retrieve granular warehouse location metadata
- **Catalog Oversight** — Access complete SKU and product variant details directly through your agent to maintain high-fidelity inventory data
- **Operational Monitoring** — Check API connectivity and manage outbound webhooks for real-time tracking of order and inventory events

### How it works

1. Subscribe to this server
2. Retrieve your **API Key** (Bearer token) from your Fizzpa dashboard (Account Settings > API)
3. Start managing your logistics and fulfillment from Claude, Cursor, or any MCP client

No more manual scrubbing through shipping logs or complex warehouse tables. Your AI acts as your dedicated logistics and operations coordinator.

### Who is this for?

- **E-commerce Ops Managers** — instantly check order statuses and monitor site-wide output using natural language commands
- **Warehouse Supervisors** — retrieve shipping labels and track real-time inventory levels without leaving your workspace
- **Customer Support Teams** — quickly verify shipping details and provide delivery updates through automated AI queries


## Available Tools
- **check_api_health**: Verify Fizzpa API connectivity
- **create_new_order**: Requires customer name and line items.

Add a new order to the system
- **cancel_order**: Delete/Cancel an order
- **get_shipping_label**: Generate shipping label for an order
- **get_account_profile**: Get authenticated account info
- **get_order_details**: Get details for a specific order
- **list_inventory_levels**: List stock levels for items
- **list_warehouse_locations**: List warehouse storage locations
- **list_fizzpa_orders**: Supports filtering by status or date.

List all customer orders
- **list_catalog_products**: List all products in the catalog
- **list_configured_webhooks**: List active webhooks
- **update_order_info**: Modify an existing order


## Installation & Usage

To install and use the **Fizzpa** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/fizzpa](https://vinkius.com/mcp/fizzpa)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
