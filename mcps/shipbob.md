# ShipBob MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/shipbob)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/shipbob-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/shipbob-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [ecommerce](../categories/ecommerce.md)

Automate your e-commerce fulfillment with ShipBob — manage products, track orders, and monitor inventory levels directly from your AI agent.

## Description
Connect your **ShipBob** account to any AI agent and take full control of your e-commerce fulfillment and supply chain through natural conversation.

### What you can do

- **Order Management** — List, retrieve, and create fulfillment orders. Check real-time statuses and cancel orders when necessary.
- **Product Catalog** — Manage your virtual product records, list variants, and convert items into bundles directly from the chat.
- **Inventory Tracking** — Monitor inventory levels across different locations, check lot-specific data, and query historical inventory movements.
- **Shipment Visibility** — Get detailed tracking information and update shipment addresses to ensure successful deliveries.
- **Returns & Receiving** — Create and manage return orders and Warehouse Receiving Orders (WRO) to keep your supply chain moving.

### How it works

1. Subscribe to this server
2. Enter your ShipBob API Token
3. Start managing your logistics from Claude, Cursor, or any MCP-compatible client

No more switching between your store backend and ShipBob dashboard to check if an order has shipped. Your AI acts as a dedicated logistics coordinator.

### Who is this for?

- **E-commerce Owners** — quickly check stock levels and order statuses without digging through complex dashboards
- **Customer Support Teams** — retrieve tracking numbers and update shipping addresses instantly to resolve customer inquiries
- **Operations Managers** — monitor warehouse receiving and inventory history to optimize supply chain workflows


## Available Tools
- **batch_cancel_shipments**: Cancel multiple shipments at once
- **batch_update_tracking**: Mark tracking as synced to your system
- **cancel_order**: Cancel an order and its shipments
- **list_channels**: g., a Shopify store).

List all channels the user has access to
- **convert_variant_to_bundle**: Convert a variant into a bundle
- **create_order**: Create a new fulfillment order
- **create_product**: Create a new product with variants
- **create_receiving**: Create a new Warehouse Receiving Order (WRO)
- **create_return**: Create a return order (RMA)
- **get_inventory_levels_by_location**: Get inventory levels grouped by fulfillment center
- **get_inventory_levels_by_lot**: Get inventory levels grouped by lot/expiration
- **get_inventory_levels**: Get aggregated inventory levels across all locations
- **get_order**: Get order details and shipment status
- **get_product**: Get details for a specific product
- **get_receiving_labels**: Get PDF box labels for a WRO
- **get_shipment**: Get specific shipment details
- **list_inventory**: List all inventory items
- **list_invoices**: List invoices by date range
- **list_orders**: List orders with status/tracking filters
- **list_products**: List products with filtering
- **list_receiving**: List Warehouse Receiving Orders (WROs)
- **list_returns**: List return orders
- **list_transaction_fees**: List available fee types
- **list_product_variants**: List all variants for a product
- **query_inventory_history**: Query inventory movement events
- **query_transactions**: Search transactions (charges, credits)
- **set_external_sync_receiving**: Mark WROs as synced to your system
- **update_product**: Update product details
- **update_return**: Update an existing return
- **update_shipment_address**: Update the shipping address for a shipment


## 💬 Prompt Examples

Here are some examples of how you can interact with the **ShipBob** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all my active ShipBob sales channels."

**🤖 AI Agent:**
> I've retrieved your channels. You have 2 active installations: 'Shopify Store Front' (ID: 4567) and 'Amazon Integration' (ID: 8910).

---

**👤 You:**
> "What is the current status and tracking for order 123456?"

**🤖 AI Agent:**
> Order 123456 is currently 'Shipped'. The tracking number is 1Z999AA10123456789 via UPS. It was dispatched from the Chicago fulfillment center.

---

**👤 You:**
> "Show me the inventory levels for SKU 'SUMMER-HAT-01'."

**🤖 AI Agent:**
> For SKU 'SUMMER-HAT-01', you have 150 units fulfillable across all locations, with 25 units currently committed to open orders.


## Installation & Usage

To install and use the **ShipBob** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/shipbob](https://vinkius.com/mcp/shipbob)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
