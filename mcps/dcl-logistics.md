# DCL Logistics MCP Server

Equip your AI agent to manage order fulfillment, track shipments, and monitor warehouse inventory via the DCL Logistics API.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/dcl-logistics)

## Overview
**Category:** ecommerce
**Tools Count:** 10

## Description
Integrate **DCL Logistics**, the leader in third-party logistics (3PL) and fulfillment, directly into your AI workflow. Manage your fulfillment orders, track shipments in real-time, and monitor warehouse inventory levels using natural language.

### What you can do

- **Order Oversight** — List and retrieve detailed statuses for all your fulfillment orders across DCL facilities.
- **Shipment Tracking** — Track recent shipments, access carrier details, and monitor delivery progress.
- **Inventory Management** — Check real-time stock levels for your SKUs and identify low-stock items.
- **Return Processing** — Monitor customer returns (RMAs) and their processing status directly via chat.

### How it works

1. Connect the DCL Logistics integration to your AI assistant.
2. Authorize using your DCL API Key and Account ID (found in your eFactory portal).
3. Orchestrate your supply chain and fulfillment operations through intuitive conversation.

### Who is this for?

- **E-commerce Brands** — Quickly check order statuses and stock levels during peak seasons.
- **Operations Managers** — Monitor shipment delays and warehouse inventory via chat.
- **Customer Support Teams** — Gather tracking information and return statuses for customer inquiries.


## Available Tools
- **get_account_details**: Returns account-level metadata such as company name, service tier, and active warehouse assignments.

Retrieve metadata for your DCL Logistics account
- **get_sku_inventory_status**: Provides a detailed breakdown of inventory status, including warehouse locations and any pending stock movements.

Get current stock level and status for a specific SKU
- **get_order_details**: Resolves line item details, recipient addresses, and the complete audit trail of order processing events.

Get detailed information for a specific order
- **get_shipment_details**: Resolves carrier-level status updates, estimated delivery dates, and proof of delivery (if available).

Get tracking and shipping details for a specific shipment ID
- **list_warehouse_inventory**: Returns a list of SKUs with their total on-hand, available, and reserved quantities.

List current inventory levels across all items
- **list_low_stock_items**: Identifies SKUs where the available quantity has fallen below the defined reorder point (e.g., < 10 units).

Identify items with inventory levels below a threshold (mock logic)
- **list_fulfillment_orders**: Returns order metadata including system IDs, current fulfillment status, and customer identifiers.

List all fulfillment orders in your DCL account
- **list_customer_returns**: Returns a list of Return Merchandise Authorizations (RMAs) including return reason, status of the returned goods, and credit processing info.

List all processed and pending customer returns (RMAs)
- **list_recent_shipments**: Returns a collection of shipment objects with associated carrier info, tracking numbers, and departure timestamps.

List all shipments processed by DCL
- **search_orders_by_keyword**: Matches keywords against order references, customer names, and shipping addresses to isolate specific fulfillment records.

Search for orders using a keyword or customer name


## Installation & Usage

To install and use the **DCL Logistics** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/dcl-logistics](https://vinkius.com/mcp/dcl-logistics)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
