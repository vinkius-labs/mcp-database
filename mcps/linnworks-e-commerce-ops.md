# Linnworks (E-commerce Ops) MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/linnworks-e-commerce-ops)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [ecommerce](../categories/ecommerce.md)

Manage e-commerce operations via Linnworks — audit open orders, track inventory SKUs, and monitor multi-location stock levels.

## Description
Connect your **Linnworks** account to any AI agent and take full control of your multi-channel e-commerce inventory and order management through natural conversation.

### What you can do

- **Order Orchestration** — List all open orders across your integrated marketplaces (Amazon, Shopify, eBay) and retrieve detailed line items and shipping info directly from your agent
- **Inventory Intelligence** — Query specific product details by exact SKU, including weights, categories, and extended property mappings required for accurate listings
- **Multi-Location Stock** — Retrieve real-time stock levels across all your physical warehouses and virtual locations to identify shortages or surplus inventory
- **Logistics Audit** — List configured postal services, shipping methods, and carriers to understand your fulfillment network and cost structures
- **Sales Channel Monitoring** — Enumerate active sales channels and their integration statuses to ensure your multichannel synchronization is healthy
- **Supplier & PO Management** — List configured suppliers and monitor recent returns and refunds from the last 30 days to maintain supply chain visibility

### How it works

1. Subscribe to this server
2. Enter your Linnworks Server URL and API Token
3. Start managing your e-commerce ops from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **E-commerce Managers** — monitor order volumes and inventory health across multiple marketplaces through natural conversation without manual report exports
- **Warehouse Leads** — check stock levels and verified warehouse locations to optimize pick-and-pack operations directly from your workspace
- **Operations Teams** — audit supplier data and sales channel integrations to ensure seamless multichannel growth and logistics compliance


## Available Tools (10)
- **get_stock_level**: Returns available, in-order, due, and minimum quantities per location.

Get Linnworks stock levels across all locations by Item ID
- **list_locations**: Returns location ID, name, address, and configuration settings for each warehouse.

Get Linnworks explicitly configured inventory locations/warehouses
- **list_postal_services**: Returns service names, carriers, tracking capabilities, and cost configuration.

Get Linnworks explicitly configured postal services
- **list_categories**: Returns category IDs, names, and parent-child hierarchy. Use to understand product organization and filter inventory.

Get Linnworks active product grouping categories
- **list_channels**: ) and their properties via /api/Inventory/GetChannels. Returns channel ID, source name, subchannel info, and integration status.

Get Linnworks active sales channel properties (Amazon, Shopify, etc)
- **list_suppliers**: Returns supplier names, codes, contact details, and currency settings.

Get Linnworks configured purchase order suppliers
- **list_returns**: Returns return IDs, reason codes, refund amounts, order references, and processing status.

Get Linnworks recent returns from the last 30 days
- **execute_custom_rpc**: Example path: /api/Inventory/GetInventoryItemTitles. All Linnworks APIs are POST-based RPC. Refer to apps.linnworks.net/Api for the full endpoint list.

Execute any custom fallback POST RPC method exposed by Linnworks API
- **list_open_orders**: Pass limit to control pagination. Returns order details including order IDs, customer info, shipping, and item lines.

Get Linnworks open orders including lines and customer info
- **get_inventory_item**: Use this to check product details, pricing, weight, and category assignment for a specific product.

Get Linnworks inventory item details by exact SKU


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Linnworks (E-commerce Ops)** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List the last 10 open orders from Linnworks"

**🤖 AI Agent:**
> I've retrieved the latest 10 open orders. Highlights include Order #12345 (Amazon US, $45.00), Order #12346 (Shopify UK, £120.00), and Order #12347 (eBay DE, €15.50). All orders are currently in the 'Unprocessed' state. Would you like to see the item lines for any of these?

---

**👤 You:**
> "Show me the stock levels for SKU 'CL-NV-001' across all locations"

**🤖 AI Agent:**
> Retrieving stock for SKU 'CL-NV-001' (ID: 98765-guid)… Main Warehouse: 45 available, Staging Area: 12 available, Retail Store: 2 available. Total across all locations: 59. There are 5 units currently in-order. Would you like to see the minimum quantity thresholds?

---

**👤 You:**
> "What sales channels are currently connected to our account?"

**🤖 AI Agent:**
> I've identified 4 active sales channels: 1) Amazon (US Marketplace), 2) Shopify (Main Webstore), 3) eBay (Global), and 4) TikTok Shop (Beta). All integrations are showing 'Healthy' status. Would you like me to check the last sync time for the Shopify channel?


## ❓ FAQ

**Q: Can I check stock levels across all my warehouses through my agent?**
Yes. Use the `get_stock_level` tool with a targeted Item ID. Your agent will return a breakdown of available, in-order, and due quantities for each of your configured locations, ensuring you have a global view of your inventory.

**Q: How do I find detailed information for a specific product SKU?**
Use the `get_inventory_item` tool and provide the exact SKU code. Your agent will fetch the full product record from Linnworks, exposing pricing, weight, dimensions, and category assignments directly in your conversation.

**Q: Can my agent list all active sales channels connected to Linnworks?**
Absolutely. Use the `list_channels` tool to identify all integrated marketplaces like Amazon, Shopify, or eBay. Your agent will report the channel source, subchannel info, and current integration status to verify your sync health.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/linnworks-e-commerce-ops](https://vinkius.com/mcp/linnworks-e-commerce-ops)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Linnworks (E-commerce Ops)** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `linnworks-e-commerce-ops` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Linnworks (E-commerce Ops)** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "linnworks-e-commerce-ops": {
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
