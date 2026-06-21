# Nuvemshop MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/nuvemshop)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/nuvemshop-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/nuvemshop-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [money-moves](../categories/money-moves.md)

Manage your Nuvemshop e-commerce via API — list products, orders, customers, coupons, and webhooks directly from any AI agent.

## Description
Connect your **Nuvemshop** store to any AI agent and take full control of your e-commerce operations through natural conversation.

### What you can do

- **Product Management** — List, create, update, and delete products with full catalog details including variants, SKUs, and stock levels
- **Order Processing** — Monitor orders, track fulfillment status, create manual orders, and update order states through the sales pipeline
- **Customer Management** — Browse customer database, view order history, create and update customer records with addresses
- **Discount Coupons** — Create, manage, and delete promotional coupons with percentage, absolute, or shipping discounts
- **Category Organization** — List product categories to understand your store's organization structure
- **Variant Management** — Inspect product variants (size, color, material) with individual SKUs, prices, and stock
- **Store Configuration** — View store details including plan, currency, domain, and settings
- **Webhook Integration** — List, create, and delete webhooks for real-time event notifications

### How it works

1. Subscribe to this server
2. Enter your Nuvemshop Access Token and Store ID
3. Start managing your e-commerce from Claude, Cursor, or any MCP-compatible client

No more navigating the Nuvemshop dashboard for every catalog or order action. Your AI acts as a dedicated store manager.

### Who is this for?

- **Store Owners** — instantly check product inventory, review new orders, and manage customer records without opening the dashboard
- **Operations Teams** — monitor order fulfillment, update order statuses, and track shipping progress
- **Marketing Teams** — create and manage discount campaigns, review coupon usage, and analyze customer segments
- **Developers** — configure webhooks for integrations, manage product variants programmatically, and automate catalog operations


## Available Tools
- **create_coupon**: You must provide the coupon code
and type (percentage, absolute, or shipping). Optional fields include value, validity dates,
minimum purchase amount, and applicable products/categories.
Example: { "code": "SUMMER20", "type": "percentage", "value": 20, "min_price": 100, "start_date": "2026-06-01", "end_date": "2026-06-30" }

Create a new discount coupon in your Nuvemshop store
- **create_customer**: You must provide at minimum 
the customer name and email. Optional fields include phone, addresses, and tags.
Example: { "first_name": "João", "last_name": "Silva", "email": "joao@example.com", "phone": "11999999999" }

Create a new customer record in your Nuvemshop store
- **create_order**: Useful for phone orders, 
in-person sales, or bulk order imports. You must provide customer information and at least 
one order item with product ID or variant ID and quantity.
Example: { "email": "customer@example.com", "items": [{ "product_id": 123, "quantity": 2 }] }

Create a new order manually in your Nuvemshop store
- **create_product**: You must provide at minimum 
the product name and price. Optional fields include description, SKU, stock quantity, 
categories, images, and variants.
Example: { "name": "T-Shirt Blue", "price": 49.90, "sku": "TSH-BLU-001", "stock": 100, "description": "Comfortable cotton t-shirt" }

Create a new product in your Nuvemshop store
- **create_webhook**: You must provide the URL to receive notifications and the events to subscribe to.
Available events include: orders/create, orders/update, products/create, products/update,
products/delete, customers/create, customers/update.
Example: { "url": "https://your-app.com/webhooks/nuvemshop", "event": "orders/create" }

Create a new webhook for real-time event notifications
- **delete_coupon**: You must provide the coupon_id.
This action cannot be undone. Use this to deactivate expired or discontinued promotions.
Be careful as this will prevent customers from using this coupon code.

Delete a discount coupon from your Nuvemshop store
- **delete_product**: You must provide the product_id.
This action cannot be undone. Use this to remove discontinued products, test products,
or items that are no longer available. Be careful as this will also remove all associated
variants and images for that product.

Delete a product from your Nuvemshop store
- **delete_webhook**: You must provide the webhook_id.
This action cannot be undone. Use this to remove webhook endpoints that are no longer needed
or to stop receiving notifications for specific events.

Delete a webhook from your Nuvemshop store
- **get_coupon**: Use the coupon_id obtained from list_coupons to inspect full coupon details.

Get detailed information about a specific coupon
- **get_customer**: Use the customer_id obtained from list_customers to inspect full customer details.
This is useful for customer support, order management, or analyzing purchase history.

Get detailed information about a specific customer
- **get_order**: Use the order_id obtained from list_orders to inspect full order details.
This is useful for verifying order status, preparing shipments, or reviewing customer purchases.

Get detailed information about a specific order
- **get_product**: Use the product_id obtained from list_products to inspect full product details.
This is useful for verifying product data before updating or checking stock levels.

Get detailed information about a specific product
- **get_store**: Use this to verify your store
setup and understand available features.

Get details about your Nuvemshop store
- **list_categories**: Each category includes name, description, and number of assigned products.
Use this to understand your store's product organization and category structure.

List all product categories in your Nuvemshop store
- **list_coupons**: Each coupon includes code, type (percentage, absolute, shipping), value, validity dates,
usage count, and minimum purchase requirements. Use this to review active promotions
and analyze coupon performance.

List all discount coupons in your Nuvemshop store
- **list_customers**: Each customer 
includes name, email, phone number, total orders, total spent, and registration date.
You can optionally specify page number and records per page. Use this to browse your 
customer database, analyze purchase patterns, or find specific customers by name or email.

List all customers in your Nuvemshop store
- **list_orders**: Each order includes
order number, customer name, total value, status (pending, paid, fulfilled, cancelled), 
payment status, and creation date. You can optionally filter by status, specify page number, 
and set records per page. Use this to monitor sales, track order fulfillment, and review revenue.

List all orders in your Nuvemshop store
- **list_products**: Each product includes 
name, description, price, SKU, stock quantity, status (active, draft, archived), and images.
You can optionally filter by status, specify page number, and set records per page (max: 200).
Use this to browse your product catalog or find a specific product by name or SKU.

List all products in your Nuvemshop store
- **list_variants**: Each variant includes SKU, price, stock quantity, and option values.
Use the product_id from list_products to see all variants of that product.
This is useful for managing inventory of products with multiple options.

List all variants for a specific product
- **list_webhooks**: ).
Each webhook includes URL, events subscribed, and creation date.
Use this to verify your integration endpoints are properly configured.

List all webhooks configured in your Nuvemshop store
- **update_coupon**: Common updates include changing discount value,
extending validity dates, or modifying minimum purchase requirements. You must provide 
the coupon_id and the fields to update as JSON.

Update an existing discount coupon
- **update_customer**: Common updates include 
changing contact information, updating addresses, or adding tags. You must provide 
the customer_id and the fields to update as JSON. Only provide the fields you want to change.

Update an existing customer record
- **update_order**: Common updates include changing order status
(e.g., from pending to paid, or from paid to fulfilled), updating shipping information,
or modifying order items. You must provide the order_id and the fields to update as JSON.

Update an existing order in your Nuvemshop store
- **update_product**: You must provide the product_id
and the fields to update as JSON. Only the fields provided will be updated.
Common updates include: changing price, updating stock quantity, modifying description,
or changing product status. The product_id must exist in your store.

Update an existing product in your Nuvemshop store


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Nuvemshop** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Show me all pending orders and their total values."

**🤖 AI Agent:**
> I found 5 pending orders:
1. **Order #10234** — João Silva — R$ 249.90 — Created: 2026-04-06
2. **Order #10235** — Maria Santos — R$ 89.90 — Created: 2026-04-06
3. **Order #10236** — Carlos Oliveira — R$ 459.00 — Created: 2026-04-07
4. **Order #10237** — Ana Costa — R$ 129.90 — Created: 2026-04-07
5. **Order #10238** — Pedro Lima — R$ 319.90 — Created: 2026-04-07

Total pending revenue: R$ 1,248.60. Would you like to update the status of any order?

---

**👤 You:**
> "Create a new coupon SUMMER20 with 20% discount, minimum purchase of R$ 100, valid until June 30th."

**🤖 AI Agent:**
> I've successfully created the coupon:
- **Code**: SUMMER20
- **Type**: Percentage discount
- **Value**: 20%
- **Minimum Purchase**: R$ 100.00
- **Valid Until**: June 30, 2026
- **Uses**: 0 / Unlimited

The coupon is now active and ready for customers to use at checkout.

---

**👤 You:**
> "List all products with stock below 10 units so I can reorder."

**🤖 AI Agent:**
> I found 8 products with stock below 10 units:
1. **T-Shirt Blue M** — SKU: TSH-BLU-M — Stock: 3 — Price: R$ 49.90
2. **T-Shirt Blue L** — SKU: TSH-BLU-L — Stock: 7 — Price: R$ 49.90
3. **Sneaker White 42** — SKU: SNK-WHT-42 — Stock: 2 — Price: R$ 199.90
4. **Cap Black** — SKU: CAP-BLK-001 — Stock: 5 — Price: R$ 39.90
5. **Backpack Gray** — SKU: BPK-GRY-001 — Stock: 1 — Price: R$ 159.90
6. **Socks Pack** — SKU: SCK-PCK-001 — Stock: 8 — Price: R$ 29.90
7. **Belt Brown** — SKU: BLT-BRN-001 — Stock: 4 — Price: R$ 79.90
8. **Wallet Black** — SKU: WLT-BLK-001 — Stock: 6 — Price: R$ 89.90

Would you like to update stock quantities for any of these products?


## Installation & Usage

To install and use the **Nuvemshop** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/nuvemshop](https://vinkius.com/mcp/nuvemshop)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
