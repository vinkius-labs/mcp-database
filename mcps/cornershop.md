# Cornershop MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/cornershop)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [industry-titans](../categories/industry-titans.md)

Automate LatAm grocery deliveries via Cornershop (by Uber) — search products, manage carts, track orders, and monitor shoppers from any AI agent.

## Description
Connect your **Cornershop by Uber** B2B account to any AI agent and manage your last-mile grocery delivery operations through natural conversation.

### What you can do

- **Store & Product Discovery** — Search through connected retail partners (Jumbo, Lider, pharmacies), browse their aisles, and find specific SKUs with real-time pricing and availability
- **Order Creation** — Construct shopping carts dynamically and place delivery orders directly through your AI agent
- **Live Tracking** — Monitor the real-time status of your orders, from picking to delivery, including GPS tracking of the assigned Shopper
- **Order Modification** — Add or remove items from the cart while the Shopper is still in the store, without opening the mobile app
- **Shopper Communication** — Retrieve contact details for assigned Shoppers to resolve delivery issues instantly

### How it works

1. Subscribe to this server
2. Enter your Cornershop Client ID and Secret (via the B2B portal or Uber Eats Direct)
3. Start managing your grocery logistics from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Corporate Office Managers** — automate office grocery and supply runs
- **B2B Resellers** — programmatically place orders for fulfillment
- **Personal Assistants** — manage client grocery lists and track deliveries efficiently


## Available Tools (14)
- **cancel_order**: Note: Orders can only be cancelled without penalty if the shopper hasn't started picking.

Cancel a pending order
- **create_order**: Requires a JSON string defining the cart (product IDs, quantities) and delivery address details.

Place a new delivery order
- **create_webhook**: g., shopper_assigned, order_delivered).

Create a new explicit webhook
- **get_order**: Get full details of a specific order
- **get_product**: Get details of a specific product
- **get_store**: Get details of a specific store branch
- **list_store_aisles**: List categories and aisles of a store
- **list_orders**: List your delivery orders
- **list_shoppers**: Get information about the assigned Shopper
- **list_stores**: g. Jumbo, Lider, pharmacies). Can be geographically filtered by latitude and longitude.

List available grocery stores and partners
- **list_webhooks**: List configured order webhooks
- **search_products**: Returns matching SKUs, names, current pricing, and availability.

Search for specific groceries and products
- **track_order**: Get real-time tracking for a delivery
- **update_order**: Useful for last-minute replacements or additions.

Update an active order (e.g. add/remove items)


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Cornershop** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Search for Jumbo stores near latitude -33.4372 and longitude -70.6506 (Santiago Centro)."

**🤖 AI Agent:**
> I found 3 Jumbo stores serving that location: 1. Jumbo Costanera Center (Store ID: JMB-992, Delivery ETA: 90 mins). 2. Jumbo Bilbao (Store ID: JMB-841, Delivery ETA: 120 mins). 3. Jumbo Paseo San Bernardo (Store ID: JMB-221, Delivery ETA: Next day). Which store would you like to search products in?

---

**👤 You:**
> "Where is the shopper for my order #CS-44919?"

**🤖 AI Agent:**
> Tracking order #CS-44919: The order is in 'delivering' status. Your Shopper (Carlos V., rating 4.9) is currently 3 blocks away (Lat: -33.412, Lng: -70.590) heading southbound. Current ETA is 7 minutes. Would you like me to verify the drop-off instructions?

---

**👤 You:**
> "Place an order at Lider (ID: LDR-10) for 2 units of SKU 'Milk-Whole-1L' and deliver into the corporate office."

**🤖 AI Agent:**
> Order successfully created! Order ID #CS-89821 has been placed at Lider (LDR-10) for 2x 'Milk-Whole-1L'. The total including service fees is $3,250. A Shopper will be assigned shortly and delivery is scheduled for the next 60 minutes window. I will notify you when shopping begins.


## ❓ FAQ

**Q: Can I add items to my order after the shopper has been assigned?**
Yes! As long as the order status is currently 'shopping', you can use the `update_order` tool to pass a JSON array with new product IDs and quantities. The Shopper's app will update dynamically with the new additions.

**Q: How can I find out the exact location of my delivery?**
If the order has reached the 'delivering' status, you can invoke the `track_order` tool with your order ID. It will return the last known latitude/longitude of the courier along with the ETA (Estimated Time of Arrival) to your destination address.

**Q: Does this work across all LATAM countries where Cornershop operates?**
Yes. The API uses global endpoints. When mapping stores using `list_stores`, you supply your local latitude and longitude to receive the stores available in your immediate geographic region (Chile, Mexico, Brazil, Colombia, Peru, etc).


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/cornershop](https://vinkius.com/mcp/cornershop)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Cornershop** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `cornershop` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Cornershop** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "cornershop": {
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
