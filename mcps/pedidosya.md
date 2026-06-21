# PedidosYa MCP Server

Automate restaurant operations on PedidosYa — manage orders, update menus, request couriers, and track deliveries across Latin America from any AI agent.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/pedidosya)

## Overview
**Category:** ecommerce
**Tools Count:** 14

## Description
Connect your **PedidosYa** partner account to any AI agent and manage the full delivery lifecycle across Latin America's leading food delivery platform.

### What you can do

- **Order Management** — Receive, accept, reject, and mark orders as ready for pickup, all through natural conversation without touching the partner tablet
- **Menu Control** — Toggle products on/off (sold out) and update prices in real-time on your live PedidosYa listing
- **Courier Logistics** — Request on-demand PedidosYa couriers for B2B deliveries and track their GPS position in real-time
- **Venue Management** — Query all your registered restaurants, their operating hours, preparation times, and marketplace performance
- **Webhook Automation** — Configure event-driven webhooks for new orders, cancellations, and courier assignments

### How it works

1. Subscribe to this server
2. Enter your PedidosYa Partner Client ID and Secret
3. Start managing your delivery operations from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Restaurant Owners** — accept orders and manage sold-out items without touching the POS tablet
- **Dark Kitchen Operators** — orchestrate multi-brand virtual kitchens across venues programmatically
- **Logistics Managers** — request on-demand courier pickups and track deliveries in real-time


## Available Tools
- **accept_order**: Once accepted, the restaurant commits to preparing the items within the estimated preparation time. The PedidosYa system will begin assigning a delivery courier.

Accept a pending order
- **create_webhook**: g., new_order, order_cancelled, courier_assigned, order_delivered).

Create a new webhook subscription
- **get_order**: Get full details of a specific order
- **get_restaurant**: Get details of a specific restaurant
- **list_menu_sections**: g., Entradas, Platos Principales, Bebidas, Postres). Each section contains its products with prices, descriptions, and availability status.

List menu sections and products for a restaurant
- **list_orders**: Filter by status to find pending orders requiring acceptance, orders being prepared, orders ready for pickup, or completed deliveries.

List incoming orders
- **list_restaurants**: Each venue includes its operating status, delivery radius, and current open/closed state.

List your partner restaurants
- **list_webhooks**: ).

List configured webhooks
- **mark_order_ready**: This triggers the courier dispatch if one hasn't already arrived.

Mark an order as ready for courier pickup
- **reject_order**: Valid rejection reasons include: out_of_stock, closing_soon, too_busy, item_unavailable. Frequent rejections may affect your venue's ranking on the platform.

Reject a pending order
- **request_courier**: Used for scheduling on-demand courier pickups, ideal for B2B deliveries outside the regular order flow. Specify the pickup and dropoff addresses and package details.

Request a PedidosYa courier for a delivery
- **track_shipment**: Track a courier shipment in real-time
- **update_product_price**: Price changes take effect immediately on the marketplace listing. The price should be in the local currency of the venue's country.

Update the price of a menu product
- **update_product_status**: Use this to mark items as temporarily unavailable (sold out) or to bring them back online without editing the full menu.

Toggle a menu product on or off


## Installation & Usage

To install and use the **PedidosYa** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/pedidosya](https://vinkius.com/mcp/pedidosya)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
