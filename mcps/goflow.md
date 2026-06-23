# Goflow MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/goflow)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [ecommerce](../categories/ecommerce.md)

Manage multichannel e-commerce inventory, orders, and listings with ease.

## Description
Connect your **Goflow** account to your AI agent and take control of your multichannel e-commerce operations. From inventory tracking to order fulfillment, manage your store directly through natural conversation.

### What you can do

- **Order Management** — List all current orders, filter by status (pending, ready to ship), and deep-dive into individual order details
- **Inventory Tracking** — Fetch real-time stock levels across all your warehouses and adjust quantities as needed directly from the chat
- **Product & Listing Visibility** — Browse your entire product catalog and see active listings on marketplaces like Amazon, Walmart, and Shopify
- **Customer & Shipment Monitoring** — View customer profiles and track shipment status to stay on top of your fulfillment pipeline
- **Operational Reports** — List and access system-generated reports for fast, data-driven operational decisions

### How it works

1. Subscribe to this server
2. Enter your Goflow Subdomain and API Bearer Token (found in your Goflow settings)
3. Start managing your e-commerce operations from Claude, Cursor, or any MCP-compatible client

No more jumping between browser tabs to check if a specific SKU is in stock or if an order has been shipped. Your AI acts as your dedicated operations assistant.

### Who is this for?

- **Store Managers** — quickly check shipment status or pending orders without manually navigating the Goflow portal
- **Warehouse Teams** — update stock levels and check inventory positions using simple voice or text commands
- **E-commerce Operations** — audit listings across multiple channels and monitor daily sales volume effortlessly


## Available Tools (12)
- **get_customer**: Get detailed info for a specific customer
- **get_inventory**: Check stock levels in Goflow
- **get_order**: Get details for a specific Goflow order
- **get_store_stats**: Get a summary of recent store activity
- **list_customers**: List customer records from Goflow
- **list_listings**: List marketplace listings (Amazon, Walmart, etc.)
- **list_orders**: List Goflow orders
- **list_products**: List products in Goflow
- **list_reports**: List available reports
- **list_shipments**: List shipments and tracking info
- **list_webhooks**: List active webhooks in Goflow
- **update_inventory**: Adjust inventory stock levels


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Goflow** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List the 10 most recent orders that are ready to ship."

**🤖 AI Agent:**
> Fetching recent shipments... I found 10 orders ready for fulfillment. Notable orders include #GF-20492 and #GF-20510. Would you like to see the packing list for order #GF-20492?

---

**👤 You:**
> "Check the inventory level for SKU 'TSHIRT-XL-BLUE'."

**🤖 AI Agent:**
> Checking stock levels... The SKU 'TSHIRT-XL-BLUE' currently has 45 units available in Warehouse A and 12 units in Warehouse B. Total stock is 57 units.

---

**👤 You:**
> "Show me the details of order GF-93021."

**🤖 AI Agent:**
> Inspecting order GF-93021... It contains 3 items: 2x 'Lid Protectors' and 1x 'Glass Jar'. The customer is 'John Doe' and the shipping address is in New York. The order is currently marked as 'Pending Fulfillment'.


## ❓ FAQ

**Q: Can I update the status of an order directly through this integration?**
Currently, the tools focus on investigative queries and inventory adjustments. Direct order status transitions are handled via the main Goflow dashboard to ensure full compliance with marketplace workflows.

**Q: Does the integration support multi-warehouse inventory management?**
Yes! When fetching inventory levels or performing adjustments with the `update_inventory` tool, you can specify the target Warehouse ID to accurately manage stock across your entire infrastructure.

**Q: How many marketplaces can I monitor with this server?**
You can monitor all marketplaces synced with your Goflow account. The `list_listings` tool will retrieve active listings from Amazon, Walmart, eBay, Shopify, and any other connected channel in real-time.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/goflow](https://vinkius.com/mcp/goflow)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Goflow** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `goflow` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Goflow** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "goflow": {
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
