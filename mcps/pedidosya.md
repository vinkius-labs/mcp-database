# PedidosYa MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/pedidosya)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [ecommerce](../categories/ecommerce.md)

Automate restaurant operations on PedidosYa — manage orders, update menus, request couriers, and track deliveries across Latin America from any AI agent.

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


## Available Tools (14)
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


## 💬 Prompt Examples

Here are some examples of how you can interact with the **PedidosYa** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Show me all pending orders for my restaurant."

**🤖 AI Agent:**
> You have 3 pending orders: 1. Order #PY-88412 — 2x Burger Clásica + 1x Papas Fritas ($345 UYU, 5 min ago). 2. Order #PY-88415 — 1x Pizza Margherita + 2x Coca-Cola ($520 UYU, 2 min ago). 3. Order #PY-88418 — 3x Empanadas + 1x Flan ($280 UYU, just now). Would you like me to accept all three?

---

**👤 You:**
> "Mark the Chocotorta as sold out on restaurant ID R-4421."

**🤖 AI Agent:**
> Done! Product 'Chocotorta' (ID: P-9922) has been marked as unavailable on restaurant R-4421's PedidosYa menu. Customers will see it greyed out until you re-enable it. Would you like to update any other products?

---

**👤 You:**
> "Request a courier to pick up a package from Av. 18 de Julio 1234, Montevideo and deliver to Rambla Wilson 500."

**🤖 AI Agent:**
> Courier requested! Shipment #SH-77201 has been created. Pickup: Av. 18 de Julio 1234, Montevideo. Dropoff: Rambla Wilson 500, Montevideo. Estimated pickup in 12 minutes. A courier will be assigned shortly. Use `track_shipment` with ID SH-77201 to monitor real-time GPS location.


## ❓ FAQ

**Q: Can my AI agent accept or reject incoming orders automatically?**
Yes! Use `accept_order` to confirm an incoming order or `reject_order` with a reason (out_of_stock, closing_soon, too_busy, item_unavailable). Once accepted, the PedidosYa system begins assigning a delivery courier. When ready, use `mark_order_ready` to signal the courier for pickup.

**Q: How do I mark items as sold out on my live menu?**
Use the `update_product_status` tool with the restaurant ID, product ID, and set `available` to false. The product will immediately show as unavailable on PedidosYa. To bring it back, call the same tool with `available` set to true.

**Q: Can I request a courier for deliveries outside of food orders?**
Yes! Use the `request_courier` tool to create a shipment request with pickup and dropoff addresses. This leverages PedidosYa's logistics network for B2B courier services, independent of restaurant orders. Track the courier in real-time with `track_shipment`.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/pedidosya](https://vinkius.com/mcp/pedidosya)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **PedidosYa** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `pedidosya` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **PedidosYa** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "pedidosya": {
      "url": "https://edge.vinkius.com/[TOKEN]/mcp"
    }
  }
}
```

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
