# Temu Seller Hub MCP Server

Automate cross-border e-commerce ops via Temu — manage orders, track fulfillment, sync inventory, and process returns natively from any AI agent.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/temu-seller-hub)

## Overview
**Category:** industry-titans
**Tools Count:** 12

## Description
Bridge your AI agents directly into the **Temu Open Platform**, Pinduoduo's global cross-border marketplace processing millions of orders daily. Automate the complete supply-chain lifecycle without navigating complex seller consoles.

### What you can do

- **Order Management** — List incoming orders from global buyers, retrieve full line-item details, and monitor payment status dynamically
- **Fulfillment & Logistics** — Query valid shipping carriers, mark orders as shipped with tracking numbers, and monitor delivery milestones
- **Inventory Sync** — Automate stock quantity updates across SKUs preventing overselling and stockout situations
- **Product Catalog** — Pull published product listings and detailed goods specifications for auditing and optimization
- **Returns Handling** — Track incoming RMA requests, query refund states, and manage reverse logistics efficiently

### How it works

1. Register as a developer on the [Temu Open Platform](https://seller.kuajingmaihuo.com/)
2. Create an application and obtain your **App Key** and **App Secret**
3. Generate an **Access Token** via the seller OAuth flow
4. Paste these credentials below — the engine handles all MD5 signature generation automatically per request

Eliminate the daily grind of refreshing seller dashboards. Your AI agent now processes orders, updates inventory, and tracks shipments automatically — letting you scale operations without scaling headcount.

### Who is this for?

- **Cross-Border Sellers** — automate order processing and inventory management across multiple regions without switching between seller portals
- **Supply Chain Coordinators** — track fulfillment pipelines and carrier assignments in real-time through natural language queries
- **E-commerce Analysts** — pull product performance data and return rates for optimization decisions directly from the AI workspace


## Available Tools
- **create_ship_order**: Uses the v2 ship order creation API.

Create a shipping order to fulfill a delivery
- **get_aftersale_list**: List after-sale / return requests
- **get_goods_detail**: Get full product details for a specific item
- **get_goods_list**: List published products on Temu store
- **get_goods_sku**: Get SKU-level details for a product
- **get_inventory**: List inventory levels across all SKUs
- **get_logistics_companies**: Get supported shipping carriers on Temu
- **get_order_detail**: Get full details for a specific Temu order
- **get_order_list**: Supports pagination and optional status filter. Uses create_after/create_before timestamps.

Get a list of Temu orders by creation date range
- **get_purchase_orders**: Used to track incoming stock requests from the platform.

Get restocking / purchase orders from Temu
- **get_ship_order_list**: List existing shipping orders
- **sync_inventory**: Update inventory stock quantity for a specific SKU


## Installation & Usage

To install and use the **Temu Seller Hub** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/temu-seller-hub](https://vinkius.com/mcp/temu-seller-hub)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
