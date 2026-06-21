# Linnworks (E-commerce Ops) MCP Server

Manage e-commerce operations via Linnworks — audit open orders, track inventory SKUs, and monitor multi-location stock levels.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/linnworks-e-commerce-ops)

## Overview
**Category:** ecommerce
**Tools Count:** 10

## Description
Connect your **Linnworks** account to any AI agent and take full control of your multi-channel e-commerce inventory and order management through natural conversation.

### What you can do

- **Order Orchestration** — List all open orders across your integrated marketplaces (Amazon, Shopify, eBay) and retrieve detailed line items and shipping info directly from your agent
- **Inventory Intelligence** — Query specific product details by exact SKU, including weights, categories, and extended property mappings required for accurate listings
- **Multi-Location Stock** — Retrieve real-time stock levels across all your physical warehouses and virtual locations to identify shortages or surplus inventory
- **Logistics Audit** — List configured postal services, shipping methods, and carriers to understand your fulfillment network and cost structures
- **Sales Channel Monitoring** — Enumerate active sales channels and their integration statuses to ensure your multichannel synchronization is healthy
- **Supplier & PO Management** — List configured suppliers and monitor recent returns and refunds from the last 30 days to maintain supply chain visibility

### How it works

1. Subscribe to this server
2. Enter your Linnworks Server URL and API Token
3. Start managing your e-commerce ops from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **E-commerce Managers** — monitor order volumes and inventory health across multiple marketplaces through natural conversation without manual report exports
- **Warehouse Leads** — check stock levels and verified warehouse locations to optimize pick-and-pack operations directly from your workspace
- **Operations Teams** — audit supplier data and sales channel integrations to ensure seamless multichannel growth and logistics compliance


## Available Tools
- **list_open_orders**: Pass limit to control pagination. Returns order details including order IDs, customer info, shipping, and item lines.

Get Linnworks open orders including lines and customer info
- **get_inventory_item**: Use this to check product details, pricing, weight, and category assignment for a specific product.

Get Linnworks inventory item details by exact SKU
- **get_stock_level**: Returns available, in-order, due, and minimum quantities per location.

Get Linnworks stock levels across all locations by Item ID
- **list_locations**: Returns location ID, name, address, and configuration settings for each warehouse.

Get Linnworks explicitly configured inventory locations/warehouses
- **list_postal_services**: Returns service names, carriers, tracking capabilities, and cost configuration.

Get Linnworks explicitly configured postal services
- **list_categories**: Returns category IDs, names, and parent-child hierarchy. Use to understand product organization and filter inventory.

Get Linnworks active product grouping categories
- **list_channels**: ) and their properties via /api/Inventory/GetChannels. Returns channel ID, source name, subchannel info, and integration status.

Get Linnworks active sales channel properties (Amazon, Shopify, etc)
- **list_suppliers**: Returns supplier names, codes, contact details, and currency settings.

Get Linnworks configured purchase order suppliers
- **list_returns**: Returns return IDs, reason codes, refund amounts, order references, and processing status.

Get Linnworks recent returns from the last 30 days
- **execute_custom_rpc**: Example path: /api/Inventory/GetInventoryItemTitles. All Linnworks APIs are POST-based RPC. Refer to apps.linnworks.net/Api for the full endpoint list.

Execute any custom fallback POST RPC method exposed by Linnworks API


## Installation & Usage

To install and use the **Linnworks (E-commerce Ops)** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/linnworks-e-commerce-ops](https://vinkius.com/mcp/linnworks-e-commerce-ops)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
