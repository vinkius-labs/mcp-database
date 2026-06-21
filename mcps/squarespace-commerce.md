# Squarespace Commerce MCP Server

Bring your Squarespace Commerce backend into your AI. Manipulate inventory, track orders, and fulfill shipments programmatically.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/squarespace-commerce)

## Overview
**Category:** industry-titans
**Tools Count:** 10

## Description
Connect your **Squarespace Commerce** backend operations exclusively to your localized artificial intelligence companion. Sever the need to log into visual CMS dashboards repetitively just to verify if an order processed successfully or if a variant sold out. Unveil inventory metrics, customer logs, and complex catalog hierarchies natively, commanding AI responses to adjust stock instantly via natural language.

### What you can do

- **Order Logistics** — Read pending commercial shipments scanning `list_orders`, pinpoint specific buyer details using `get_order_details` and finalize dispatch procedures securely invoking `fulfill_order`
- **Inventory Scaling** — Audit remaining physical store stock actively running `list_inventory`, and inject stock resupplies or debits commanding `adjust_inventory` instantly
- **Product Catalog** — Pull deep merchandising arrays gathering everything your shop sells utilizing `list_products` and breaking down SKU variants natively requesting `get_product_details`
- **CRM & Books** — Download shopper histories calling `list_customer_profiles` while tracking absolute bank flow via pure data streams with `list_transactions`

### How it works

1. Enable the MCP bridge natively on your computing environment
2. Provide your overarching Squarespace Developer API Key securely
3. Engage your language model internally telling it to flag all unfulfilled orders older than 48 hours automatically

### Who is this for?

- **E-Commerce Operations** — automate repetitive dispatch approvals by commanding LLMs to process `fulfill_order` based on simple logic parameters over chat
- **Back-End Developers** — build specialized headless checkout flows investigating exact endpoint limits or structures blindly without consulting postman 
- **Shop Managers & Owners** — pull markdown tables highlighting "Low Stock Items" instantly right inside Cursor to orchestrate purchasing cycles quickly


## Available Tools
- **adjust_inventory**: Provide a variant_id and a quantity delta (e.g. 5 to add, -2 to subtract).

Adjusts the inventory quantity for a product variant
- **fulfill_order**: Requires order_id, tracking_number, and carrier name.

Marks an order as fulfilled and adds tracking information
- **get_order_details**: Retrieves details for a specific order
- **get_product_details**: Retrieves details for a specific product
- **list_inventory**: Lists inventory levels for product variants
- **list_orders**: Supports pagination via cursor.

Lists Squarespace Commerce orders
- **list_products**: Returns product names and IDs. Use the cursor from the previous response for pagination.

Lists Squarespace Commerce products
- **list_customer_profiles**: Lists Squarespace customer profiles
- **list_transactions**: Lists financial transactions
- **list_webhooks**: Lists configured webhook subscriptions


## Installation & Usage

To install and use the **Squarespace Commerce** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/squarespace-commerce](https://vinkius.com/mcp/squarespace-commerce)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
