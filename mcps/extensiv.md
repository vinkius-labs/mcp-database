# Extensiv MCP Server

Manage omnichannel operations via Extensiv — track orders and shipments, monitor inventory and warehouses, and manage vendors directly from any AI agent.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/extensiv)

## Overview
**Category:** ecommerce
**Tools Count:** 10

## Description
Connect your **Extensiv** (formerly Skubana) account to any AI agent and take full control of your omnichannel e-commerce operations and inventory management through natural conversation.

### What you can do

- **Order Orchestration** — List and filter omnichannel orders to retrieve order numbers, statuses, channel mappings, and line items natively
- **Inventory Auditing** — Monitor current stock levels across all warehouses, including available, committed, on-order, and in-transit quantities
- **Warehouse Management** — Retrieve configurations for 3PL and in-house warehouses, identifying addresses and capability settings flawlessly
- **Supply Chain Oversight** — List purchase orders (POs) and track vendor shipments, expected delivery dates, and receiving statuses securely
- **Product Master Data** — Access core product details including SKUs, dimensions, weights, and costs to manage your catalog metadata
- **Vendor & Brand Control** — Manage supplier contact details, lead times, and payment terms, and list all product brands configured in the system
- **Return & RMA Tracking** — Monitor return merchandise authorizations with reason codes, status updates, and linked refund amounts in real-time
- **Customer Intelligence** — Retrieve customer profiles with shipping addresses and order history summaries to resolve inquiries limitlessly

### How it works

1. Subscribe to this server
2. Enter your Extensiv API Access Token (obtained via OAuth or from your App details)
3. Start managing your omnichannel operations from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **E-commerce Ops Managers** — monitor inventory levels and track shipments across multiple channels using natural language
- **Inventory Coordinators** — audit warehouse stock and manage purchase orders without opening the Extensiv dashboard
- **Customer Support Teams** — quickly look up order statuses and customer histories to resolve inquiries in real-time
- **Supply Chain Analysts** — track vendor performance and monitor lead times through natural conversation


## Available Tools
- **list_orders**: 1/orders with pagination. Returns orders with order number, status, channel, shipping address, line items, and fulfillment tracking. Pass limit to control page size (default 100).

List Extensiv/Skubana orders
- **list_products**: 1/products with pagination. Returns product master data including SKU, name, dimensions, weight, cost, and linked vendor information.

List Extensiv products
- **list_inventory**: 1/inventory with pagination. Returns current stock levels by warehouse and product, including available, committed, on-order, and in-transit quantities.

List Extensiv inventory levels
- **list_warehouses**: 1/warehouses. Returns all configured 3PL and in-house warehouses with name, address, type, and capability settings. No parameters required.

List Extensiv warehouses
- **list_pos**: 1/purchaseorders with pagination. Returns PO number, vendor, expected date, line items with SKU and quantity, and receiving status.

List Extensiv purchase orders
- **list_vendors**: 1/vendors. Returns all configured vendors with name, contact details, lead time, currency, and payment terms. No parameters required.

List Extensiv vendors/suppliers
- **list_shipments**: 1/shipments with pagination. Returns shipment tracking details including carrier, tracking number, ship date, delivery status, and linked order references.

List Extensiv shipments
- **list_rmas**: 1/rmas with pagination. Returns return merchandise authorizations with reason code, status, linked order, refund amount, and items being returned.

List Extensiv returns (RMAs)
- **list_brands**: 1/brands. Returns all product brands configured in the system with brand name and description. No parameters required.

List Extensiv brands
- **list_customers**: 1/customers with pagination. Returns customer profiles with name, email, phone, shipping address, and order history summary.

List Extensiv customers


## Installation & Usage

To install and use the **Extensiv** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/extensiv](https://vinkius.com/mcp/extensiv)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
