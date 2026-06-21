# Megaventory MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/megaventory)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [supply-chain](../categories/supply-chain.md)

Inventory and order management via Megaventory — track products, stock levels, and orders.

## Description
Connect your **Megaventory** account to any AI agent and take full control of your inventory management and order fulfillment through natural conversation.

### What you can do

- **Inventory Management** — List all products, search by description, and fetch detailed SKU metadata
- **Stock Tracking** — Retrieve real-time stock levels across all configured inventory locations
- **Order Orchestration** — List and inspect sales orders and purchase orders with full status visibility
- **Entity Management** — Manage your directory of suppliers and clients directly from your agent
- **Warehouse Oversight** — Enumerate active inventory locations and their specific configurations

### How it works

1. Subscribe to this server
2. Enter your Megaventory API Key
3. Start managing your inventory from Claude, Cursor, or any MCP-compatible client


## Available Tools
- **get_product**: Get details for a specific product SKU
- **get_purchase_order**: Get details for a specific purchase order
- **get_sales_order**: Get details for a specific sales order
- **get_product_stock**: Get stock levels for a product SKU
- **list_suppliers_clients**: List all suppliers and clients
- **list_inventory_locations**: List all inventory locations
- **list_products**: List all products
- **list_purchase_orders**: List all purchase orders
- **list_sales_orders**: List all sales orders
- **search_products**: Search for products by description


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Megaventory** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all products in my Megaventory account."

**🤖 AI Agent:**
> Retrieving products... I found several items including 'Standard Widget' (SKU: WID-001) and 'Premium Gadget' (SKU: GAD-999).

---

**👤 You:**
> "What is the stock level for SKU 'WID-001'?"

**🤖 AI Agent:**
> Checking stock levels... SKU 'WID-001' has 150 units available across your 3 inventory locations.

---

**👤 You:**
> "Show the last 5 sales orders."

**🤖 AI Agent:**
> Querying sales orders... I found your most recent orders, including SO-12345 for Client 'TechCorp' and SO-12344 for 'Global Solutions'.


## ❓ FAQ

**Q: How do I find my Megaventory API Key?**
Log in to Megaventory, go to Settings, and look for the API section to generate or copy your API Key.

**Q: Can I check stock levels for a specific SKU?**
Yes! Use the `get_product_stock` tool and provide the product SKU to see current availability across all locations.

**Q: Is my inventory data secure?**
Absolutely. Your token is encrypted at rest and injected securely at runtime.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/megaventory](https://vinkius.com/mcp/megaventory)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Megaventory** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `megaventory` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Megaventory** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "megaventory": {
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
