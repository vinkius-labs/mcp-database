# Amplifier MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/amplifier)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [ecommerce](../categories/ecommerce.md)

E-commerce fulfillment orchestration — manage orders, inventory, and shipments via AI.

## Description
Connect your **Amplifier** account to your AI agent to unlock professional e-commerce fulfillment orchestration. From managing incoming orders and auditing real-time inventory to retrieving tracking details for recent shipments, your agent handles your logistics pipeline through natural conversation.

### What you can do

- **Order Management** — List incoming fulfillment orders, retrieve detailed item lists, and submit new orders to the warehouse
- **Inventory Auditing** — Retrieve comprehensive inventory reports and monitor stock levels across all your SKUs
- **Shipment Tracking** — List recent shipments and retrieve tracking numbers and delivery statuses effortlessly
- **Catalog Oversight** — Search and list items in your catalog to retrieve technical metadata and identifiers
- **Logistics Insights** — Quickly identify low-stock items or verify order fulfillment statuses directly from your chat interface

### How it works

1. Subscribe to this server
2. Enter your Amplifier API Key
3. Start managing your fulfillment operations and monitoring logistics through Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **E-commerce Managers** — automate order audits and monitor warehouse fulfillment times effortlessly
- **Logistics Operations** — track shipment statuses and manage stock replenishment alerts on the fly
- **Customer Support Teams** — quickly look up tracking numbers and order details to resolve shipping inquiries
- **Developers** — submit test orders using Sandbox keys and verify API configurations using simple commands


## Available Tools (7)
- **list_orders**: List fulfillment orders
- **get_order_details**: Get order metadata
- **create_order**: Submit new order
- **list_items**: List catalog items
- **get_inventory_report**: Get inventory stock levels
- **get_shipment_report**: Get shipment tracking
- **get_item_details**: Get item metadata


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Amplifier** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List my recent fulfillment orders."

**🤖 AI Agent:**
> I've retrieved your recent orders. There are 5 pending orders waiting for fulfillment in the warehouse. Would you like me to check the specific items for the most recent order?

---

**👤 You:**
> "Get the inventory report for all items."

**🤖 AI Agent:**
> I've retrieved your inventory report. Your 'Premium T-Shirt (Large)' currently has 120 units in stock, while the 'Coffee Mug' is running low with only 5 units remaining. Would you like me to flag any other low-stock items?

---

**👤 You:**
> "Retrieve the latest shipment tracking details."

**🤖 AI Agent:**
> I've accessed your shipment reports. The last 3 orders were shipped via UPS Ground. The tracking number for the most recent order (Order #1005) is '1Z9999999999999999'. Would you like the tracking numbers for the others?


## ❓ FAQ

**Q: How do I get my Amplifier API Key?**
Log in to your Amplifier account. You need a PRO account to generate production API keys. You can also create Sandbox keys for testing. The API key is used as the username in Basic Auth with a blank password.

**Q: Can I test orders without fulfilling them?**
Yes! If you use a Sandbox API key, the `create_order` tool will simulate the order creation without triggering actual fulfillment in the warehouse.

**Q: How do I check my current stock levels?**
Use the `get_inventory_report` tool. It retrieves the current stock levels for all your catalog items at once, making it easy to identify low-stock SKUs.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/amplifier](https://vinkius.com/mcp/amplifier)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Amplifier** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `amplifier` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Amplifier** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "amplifier": {
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
