# Order Desk MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/order-desk)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [logistics-supply-chain](../categories/logistics-supply-chain.md)

Order and inventory management — automate your fulfillment workflows via Order Desk.

## Description
Connect your **Order Desk** account to empower your AI agents with multi-channel fulfillment capabilities. This server provides programmatic access to the Order Desk API for managing orders, inventory, and shipments across hundreds of integrations.

### What you can do

- **Order Orchestration** — List and inspect orders across all your sales channels
- **Inventory Management** — Track stock levels and product details in real-time
- **Shipment Monitoring** — Access tracking information and shipment details for your orders
- **Workflow Automation** — Organize orders using folders and custom shipping methods
- **Cross-Channel Visibility** — Monitor your entire commerce operation through simple natural language commands

### How it works

1. Subscribe to this server
2. Enter your **Order Desk Store ID** and **API Key**
3. Start managing your fulfillment from Claude, Cursor, or any MCP client


## Available Tools
- **get_inventory_item**: Get inventory item details
- **get_order**: Get details for a specific order
- **get_order_shipments**: Get shipments for an order
- **list_folders**: List order folders
- **list_inventory_items**: List inventory items
- **list_orders**: You can optionally filter by folder_id.

List all Order Desk orders
- **list_shipping_methods**: List shipping methods


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Order Desk** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List my latest Order Desk orders."

**🤖 AI Agent:**
> Fetching orders... I've found 10 recent orders. Here is the summary...


## ❓ FAQ

**Q: How do I find my Store ID and API Key?**
Log in to Order Desk, go to Store Settings in the sidebar, and click on the API tab.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/order-desk](https://vinkius.com/mcp/order-desk)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Order Desk** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `order-desk` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Order Desk** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "order-desk": {
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
