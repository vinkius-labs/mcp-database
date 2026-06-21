# SkuVault MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/skuvault)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [order-management](../categories/order-management.md)

Manage your SkuVault inventory, products, lots, and purchase orders directly from any AI agent.

## Description
Connect your **SkuVault** account to any AI agent to streamline your warehouse and inventory management workflows through natural conversation.

### What you can do

- **Inventory Management** — Add inventory quantities to specific warehouse locations individually or in bulk.
- **Product & Brand Catalog** — Create products, bulk-import items, and configure brands or suppliers.
- **Lot & Hold Tracking** — Retrieve and manage product lots, inspect lot inventory by location, and create inventory holds.
- **Kits & Bundles** — Create product kits and bundles to optimize your catalog.
- **Purchase Orders & Shipments** — Generate purchase orders and record shipments directly.

### How it works

1. Subscribe to this server
2. Enter your SkuVault Tenant Token and User Token
3. Start managing your inventory from Claude, Cursor, or any MCP-compatible client


## Available Tools
- **add_item_bulk**: Bulk add items to inventory
- **add_item**: Adds inventory quantity to a specific warehouse location
- **add_shipments**: Add shipment records
- **create_brands**: Create new product brands
- **create_holds**: Create inventory holds
- **create_kit**: Create product kits/bundles
- **create_lot**: Create product lots
- **create_po**: Create Purchase Orders
- **create_product**: Create a single product
- **create_products**: Bulk create products
- **create_suppliers**: Create product suppliers
- **get_available_quantities**: Retrieve available inventory quantities
- **get_brands**: Retrieve brands
- **get_classifications**: Retrieve product classifications
- **get_external_warehouse_quantities**: Retrieve quantities in external warehouses
- **get_external_warehouses**: Retrieve external warehouse details
- **get_handling_time**: Retrieve product handling times
- **get_incoming_items**: Retrieve incoming items (e.g., from POs or shipments)
- **get_lot_inventory_by_location**: Retrieve lot inventory details filtered by location
- **get_lots**: Retrieve product lots


## 💬 Prompt Examples

Here are some examples of how you can interact with the **SkuVault** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Add 15 units of SKU 'WIDGET-A' to warehouse 2, location 'LOC-99' with reason 'Restock'."

**🤖 AI Agent:**
> I will call the `add_item` tool with Sku: 'WIDGET-A', WarehouseId: 2, LocationCode: 'LOC-99', Quantity: 15, and Reason: 'Restock' to update the inventory.

---

**👤 You:**
> "Retrieve lot inventory details for location 'ZONE-B'."

**🤖 AI Agent:**
> I will query the SkuVault API using the `get_lot_inventory_by_location` tool with the location filter set to 'ZONE-B' to fetch the lot details.

---

**👤 You:**
> "Create a new product with SKU 'SHIRT-XL-RED' named 'Red XL Shirt'."

**🤖 AI Agent:**
> I will use the `create_product` tool to create a new product with SKU 'SHIRT-XL-RED' and name 'Red XL Shirt' in your SkuVault catalog.


## ❓ FAQ

**Q: How can I add inventory to a specific warehouse location?**
You can use the `add_item` tool. Provide the SKU or Code, the WarehouseId, the LocationCode, the Quantity, and a valid transaction Reason.

**Q: Can I retrieve product lot details filtered by location?**
Yes! Use the `get_lot_inventory_by_location` tool to retrieve lot inventory details filtered by specific locations.

**Q: Is there a way to create multiple products at once?**
Yes, you can use the `create_products` tool to bulk-create products by passing a JSON payload with the product details.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/skuvault](https://vinkius.com/mcp/skuvault)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **SkuVault** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `skuvault` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **SkuVault** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "skuvault": {
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
