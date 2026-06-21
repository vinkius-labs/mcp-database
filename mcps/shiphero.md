# ShipHero MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/shiphero)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [ecommerce](../categories/ecommerce.md)

Manage e-commerce logistics via ShipHero — track orders, monitor inventory levels, and handle warehouse movements directly from your AI agent.

## Description
Connect your **ShipHero** account to any AI agent to streamline your warehouse and fulfillment operations through natural language.

### What you can do

- **Order Management** — List recent orders and create new ones with full shipping and line item details.
- **Inventory Control** — Check real-time stock levels by SKU, track history of inventory changes, and add or remove stock instantly.
- **Bulk Operations** — Sync inventory levels in bulk using CSV URLs for rapid warehouse updates.
- **Product Insights** — Retrieve deep metadata for products, including warehouse-specific availability and legacy ID conversion.
- **Automation** — Register webhooks to stay updated on inventory changes or order statuses.

### How it works

1. Subscribe to this server
2. Enter your ShipHero Access Token
3. Start managing your logistics from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **E-commerce Managers** — monitor fulfillment health and stock levels without leaving your workspace
- **Operations Teams** — quickly adjust inventory and track movement history during audits
- **Developers** — integrate warehouse data into your workflow and test webhooks via simple prompts


## Available Tools
- **add_inventory**: Add or remove inventory for a SKU
- **create_order**: Create a new order in ShipHero
- **create_webhook**: Register a new webhook
- **get_uuid**: Get UUID from a legacy numeric ID
- **list_inventory_changes**: List inventory changes for a SKU
- **list_orders**: List ShipHero orders
- **get_product**: Get product details by SKU
- **sync_inventory**: Bulk sync inventory via CSV URL


## 💬 Prompt Examples

Here are some examples of how you can interact with the **ShipHero** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List the 10 most recent orders from my primary warehouse."

**🤖 AI Agent:**
> I've retrieved the latest orders. You have 10 recent records, including Order #SH-1029 (Status: Pending) and Order #SH-1030 (Status: Fulfilled). Would you like details on a specific one?

---

**👤 You:**
> "Check the current inventory level and warehouse details for SKU 'BLUE-SHIRT-L'."

**🤖 AI Agent:**
> For SKU 'BLUE-SHIRT-L', I found 45 units available in Warehouse A and 12 units in Warehouse B. The total on-hand inventory is 57 units.

---

**👤 You:**
> "Add 25 units to SKU 'GIFT-WRAP' in warehouse 'WH-99' because of a new shipment."

**🤖 AI Agent:**
> Successfully updated inventory for 'GIFT-WRAP'. Added 25 units to warehouse 'WH-99'. The new balance has been synchronized.


## ❓ FAQ

**Q: How can I track the history of stock movements for a specific product?**
You can use the `list_inventory_changes` tool by providing the product SKU. It will return a detailed history of inventory adjustments, helping you audit stock movements over time.

**Q: Is it possible to bulk update inventory levels across my warehouse?**
Yes! The `sync_inventory` tool allows you to provide a URL to a CSV file containing your inventory data. The server will process the file and sync the levels for the specified warehouse ID.

**Q: What should I do if I only have a legacy numeric ID for an order or product?**
Use the `get_uuid` tool. It is specifically designed to convert legacy numeric IDs into the opaque UUIDs required by the modern ShipHero API for entities like Orders or Products.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/shiphero](https://vinkius.com/mcp/shiphero)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **ShipHero** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `shiphero` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **ShipHero** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "shiphero": {
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
