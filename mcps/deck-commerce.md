# Deck Commerce MCP Server

Equip your AI agent to manage order fulfillment, track shipments, and monitor inventory via the Deck Commerce API.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/deck-commerce)

## Overview
**Category:** ecommerce
**Tools Count:** 10

## Description
Integrate **Deck Commerce**, the leading order management system (OMS) for direct-to-consumer retailers, directly into your AI workflow. Manage your customer orders, track real-time inventory levels across facilities, and monitor shipments and returns using natural language.

### What you can do

- **Order Oversight** — List and retrieve detailed information for all customer orders and their current processing status.
- **Inventory Intelligence** — Access real-time stock levels for your SKUs and monitor backordered items.
- **Shipment Tracking** — Track processed shipments, access tracking numbers, and monitor delivery progress.
- **Return Management** — List customer returns and monitor their status directly via chat.

### How it works

1. Connect the Deck Commerce integration to your AI assistant.
2. Authorize using your Deck Commerce API Key and Site ID (found in your admin portal).
3. Optimize your omnichannel operations and fulfillment through intuitive conversation.

### Who is this for?

- **E-commerce Operations** — Quickly check order statuses and stock availability across multiple nodes.
- **Logistics Managers** — Monitor shipment progress and identify fulfillment bottlenecks via chat.
- **Customer Service Teams** — Gather tracking info and return details for customer inquiries instantly.


## Available Tools
- **get_account_metadata**: Returns account-level metadata such as organization name, active integrations, and system configuration.

Retrieve settings and metadata for your Deck Commerce account
- **get_sku_stock_level**: Provides a detailed breakdown of quantities at individual fulfillment nodes and identifies current inventory status.

Get current stock level and status for a specific SKU
- **get_order_details**: Resolves line item details, shipping addresses, tax information, and the full order history trail.

Get detailed information for a specific order
- **get_shipment_tracking**: Resolves carrier status updates, delivery estimates, and current shipment location.

Get tracking and shipping details for a specific shipment
- **list_backordered_items**: Identifies products where demand exceeds current on-hand availability.

List all items currently on backorder (mock logic)
- **list_available_inventory**: Returns a list of SKUs with their total available-to-sell, on-hand, and reserved quantities across all nodes.

List current inventory levels across all items
- **list_oms_orders**: Returns order metadata including order numbers, current status, and customer identifiers.

List all customer orders in your Deck Commerce OMS
- **list_order_returns**: Returns a list of return requests including return reasons, RMA numbers, and current processing state.

List all customer returns and their processing status
- **list_processed_shipments**: Returns shipment metadata including carrier information, tracking numbers, and fulfillment timestamps.

List all shipments processed by Deck Commerce
- **search_orders_by_number**: Matches keywords against order numbers, customer names, and email addresses to isolate specific OMS records.

Search for orders using an order number or customer info


## Installation & Usage

To install and use the **Deck Commerce** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/deck-commerce](https://vinkius.com/mcp/deck-commerce)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
