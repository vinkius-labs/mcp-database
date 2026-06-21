# Temu Seller Hub MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/temu-seller-hub)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [industry-titans](../categories/industry-titans.md)

Automate cross-border e-commerce ops via Temu — manage orders, track fulfillment, sync inventory, and process returns natively from any AI agent.

## Description
Bridge your AI agents directly into the **Temu Open Platform**, Pinduoduo's global cross-border marketplace processing millions of orders daily. Automate the complete supply-chain lifecycle without navigating complex seller consoles.

### What you can do

- **Order Management** — List incoming orders from global buyers, retrieve full line-item details, and monitor payment status dynamically
- **Fulfillment & Logistics** — Query valid shipping carriers, mark orders as shipped with tracking numbers, and monitor delivery milestones
- **Inventory Sync** — Automate stock quantity updates across SKUs preventing overselling and stockout situations
- **Product Catalog** — Pull published product listings and detailed goods specifications for auditing and optimization
- **Returns Handling** — Track incoming RMA requests, query refund states, and manage reverse logistics efficiently

### How it works

1. Register as a developer on the [Temu Open Platform](https://seller.kuajingmaihuo.com/)
2. Create an application and obtain your **App Key** and **App Secret**
3. Generate an **Access Token** via the seller OAuth flow
4. Paste these credentials below — the engine handles all MD5 signature generation automatically per request

Eliminate the daily grind of refreshing seller dashboards. Your AI agent now processes orders, updates inventory, and tracks shipments automatically — letting you scale operations without scaling headcount.

### Who is this for?

- **Cross-Border Sellers** — automate order processing and inventory management across multiple regions without switching between seller portals
- **Supply Chain Coordinators** — track fulfillment pipelines and carrier assignments in real-time through natural language queries
- **E-commerce Analysts** — pull product performance data and return rates for optimization decisions directly from the AI workspace


## Available Tools (12)
- **create_ship_order**: Uses the v2 ship order creation API.

Create a shipping order to fulfill a delivery
- **get_aftersale_list**: List after-sale / return requests
- **get_goods_detail**: Get full product details for a specific item
- **get_goods_list**: List published products on Temu store
- **get_goods_sku**: Get SKU-level details for a product
- **get_inventory**: List inventory levels across all SKUs
- **get_logistics_companies**: Get supported shipping carriers on Temu
- **get_order_detail**: Get full details for a specific Temu order
- **get_order_list**: Supports pagination and optional status filter. Uses create_after/create_before timestamps.

Get a list of Temu orders by creation date range
- **get_purchase_orders**: Used to track incoming stock requests from the platform.

Get restocking / purchase orders from Temu
- **get_ship_order_list**: List existing shipping orders
- **sync_inventory**: Update inventory stock quantity for a specific SKU


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Temu Seller Hub** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Get my Temu orders from the last 24 hours and summarize pending fulfillment."

**🤖 AI Agent:**
> Orders retrieved! You have 15 new orders in the last 24 hours. 11 are pending fulfillment, 3 are already shipped, and 1 is awaiting payment confirmation. The pending orders total $2,340 USD across 8 different destination countries. Would you like me to flag orders approaching the shipping SLA deadline?

---

**👤 You:**
> "Mark order TMU-2024-88712 as shipped with tracking number YT2048391004."

**🤖 AI Agent:**
> Order TMU-2024-88712 has been successfully marked as shipped! Carrier: Yanwen Express. Tracking: YT2048391004. The buyer will receive a notification with the tracking link automatically. Estimated delivery: 7-12 business days to destination (USA). Would you like to process the remaining 10 pending orders?

---

**👤 You:**
> "Update inventory for SKU TMU-SHOE-42BLK to 250 units."

**🤖 AI Agent:**
> Inventory updated! SKU TMU-SHOE-42BLK is now set to 250 units (previously 45 units). The change will be reflected on the Temu storefront within 5 minutes. Note: this SKU had 3 pending orders — the new stock level comfortably covers demand. Should I run a full inventory audit across all your active SKUs?


## ❓ FAQ

**Q: How do I obtain the Access Token required for authentication?**
You must complete the OAuth 2.0 authorization flow using your App Key through your specific seller account on the Temu Open Platform. The flow will generate an Access Token that grants scoped permissions to your store's order, inventory, and logistics data.

**Q: Can I manage inventory across multiple SKU variants simultaneously?**
Yes! The `sync_inventory` tool accepts batch SKU updates. You can push quantity changes for multiple product variants in a single call, and the engine handles all MD5 signature computation and parameter encoding automatically.

**Q: Is there any risk of accidentally modifying live product listings or canceling orders?**
All write operations require explicit parameters — order IDs, SKU identifiers, tracking numbers — that must be deliberately specified. The Access Token is scoped to your seller account, and the MD5 signature layer prevents request forgery. Critical actions like order cancellation are logged and require confirmation parameters.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/temu-seller-hub](https://vinkius.com/mcp/temu-seller-hub)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Temu Seller Hub** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `temu-seller-hub` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Temu Seller Hub** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "temu-seller-hub": {
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
