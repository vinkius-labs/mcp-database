# LeafLink MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/leaflink)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [ecommerce](../categories/ecommerce.md)

Manage cannabis wholesale orders, products, and inventory via the LeafLink API.

## Description
Connect your **LeafLink** account to any AI agent to automate your cannabis wholesale operations. This MCP server enables your agent to manage product listings, monitor real-time inventory, and track received orders directly from natural language.

### What you can do

- **Order Oversight** — List and retrieve detailed information for all wholesale orders received from buyers
- **Inventory Visibility** — Get real-time stock levels and availability for your entire product catalog
- **Catalog Management** — List, retrieve, create, and update products including pricing and metadata
- **Status Transitions** — Move orders through their lifecycle (accept, fulfill, cancel) via simple commands
- **Partner Tracking** — List registered brands and buyers to maintain clear visibility of your wholesale network

### How it works

1. Subscribe to this server
2. Enter your LeafLink API Key (JWT Bearer Token)
3. Start managing your wholesale business from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Wholesale Managers** — Monitor incoming orders and update product availability without opening the dashboard
- **Operations Teams** — Automate inventory updates and order fulfillment workflows via natural language
- **Sales Directors** — Quickly query brand catalogs and buyer information during planning sessions


## Available Tools
- **list_wholesale_brands**: List all brands in your account
- **create_new_product**: Requires a JSON body with product details.

Add a new product to your wholesale catalog
- **list_wholesale_customers**: List all buyers and customers
- **get_order_details**: Get details for a specific order
- **get_product_details**: Get details for a specific product
- **list_received_orders**: List all wholesale orders received
- **list_wholesale_products**: List all products available in your inventory
- **update_order_status**: g., accept, fulfill, cancel, reject).

Transition an order through its lifecycle
- **update_product_inventory**: Update inventory level for a specific product


## 💬 Prompt Examples

Here are some examples of how you can interact with the **LeafLink** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Show me all active wholesale orders in LeafLink."

**🤖 AI Agent:**
> I've retrieved your received orders. You have 8 active orders, including Order #ORD-101 from 'Green Valley Dispensary' and #ORD-102 from 'High Peak Wellness'. Would you like to see the details for any of them?

---

**👤 You:**
> "Check the inventory level for 'Sour Diesel Flower 3.5g'."

**🤖 AI Agent:**
> For 'Sour Diesel Flower 3.5g', I found 150 units currently in stock with 25 units reserved for pending orders, leaving 125 units available for wholesale.

---

**👤 You:**
> "Accept the order #ORD-101."

**🤖 AI Agent:**
> Successfully accepted order #ORD-101. Its status has been updated in LeafLink, and the buyer has been notified.


## ❓ FAQ

**Q: How do I update the inventory level for a product?**
Use the `update_product_inventory` tool with the unique product ID and the new total quantity. This will update the quantity field in LeafLink.

**Q: Can I fulfill an order using the agent?**
Yes, use the `update_order_status` tool with the order number and set the action to 'fulfill' to transition the order status.

**Q: Is it possible to see my buyer list?**
Absolutely. The `list_wholesale_customers` tool retrieves all organizational buyers and dispensary accounts registered in your LeafLink network.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/leaflink](https://vinkius.com/mcp/leaflink)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **LeafLink** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `leaflink` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **LeafLink** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "leaflink": {
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
