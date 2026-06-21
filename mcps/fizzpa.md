# Fizzpa MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/fizzpa)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [ecommerce](../categories/ecommerce.md)

Market your restaurant or food business with digital menus, online ordering integration, and customer engagement tools.

## Description
Connect your **Fizzpa** account to any AI agent and take full control of your e-commerce fulfillment, order management, and warehouse workflows through natural conversation.

### What you can do

- **Order Orchestration** — List and manage customer orders programmatically, including retrieving detailed line items and updating fulfillment statuses
- **Label & Logistics** — Programmatically generate shipping labels and retrieve direct print URLs (PDF/Image) to streamline your shipping operations
- **Inventory Intelligence** — Monitor real-time stock levels across your product catalog and retrieve granular warehouse location metadata
- **Catalog Oversight** — Access complete SKU and product variant details directly through your agent to maintain high-fidelity inventory data
- **Operational Monitoring** — Check API connectivity and manage outbound webhooks for real-time tracking of order and inventory events

### How it works

1. Subscribe to this server
2. Retrieve your **API Key** (Bearer token) from your Fizzpa dashboard (Account Settings > API)
3. Start managing your logistics and fulfillment from Claude, Cursor, or any MCP client

No more manual scrubbing through shipping logs or complex warehouse tables. Your AI acts as your dedicated logistics and operations coordinator.

### Who is this for?

- **E-commerce Ops Managers** — instantly check order statuses and monitor site-wide output using natural language commands
- **Warehouse Supervisors** — retrieve shipping labels and track real-time inventory levels without leaving your workspace
- **Customer Support Teams** — quickly verify shipping details and provide delivery updates through automated AI queries


## Available Tools
- **check_api_health**: Verify Fizzpa API connectivity
- **create_new_order**: Requires customer name and line items.

Add a new order to the system
- **cancel_order**: Delete/Cancel an order
- **get_shipping_label**: Generate shipping label for an order
- **get_account_profile**: Get authenticated account info
- **get_order_details**: Get details for a specific order
- **list_inventory_levels**: List stock levels for items
- **list_warehouse_locations**: List warehouse storage locations
- **list_fizzpa_orders**: Supports filtering by status or date.

List all customer orders
- **list_catalog_products**: List all products in the catalog
- **list_configured_webhooks**: List active webhooks
- **update_order_info**: Modify an existing order


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Fizzpa** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all pending orders in Fizzpa."

**🤖 AI Agent:**
> I've retrieved your pending orders. You have 3 shipments awaiting fulfillment, including Order #101 (John Doe) and Order #102. Which one would you like to process first?

---

**👤 You:**
> "Get the shipping label for order ID 'ord_123'."

**🤖 AI Agent:**
> Label generated! I've retrieved the print URL for order ord_123. You can download or print it here: [link]. Your warehouse team can now finalize the shipment.

---

**👤 You:**
> "What are the stock levels for SKU 'SHIRT-BLUE-L'?"

**🤖 AI Agent:**
> Checking inventory... For SKU 'SHIRT-BLUE-L' (ID: prod_789), you currently have 45 units available in the 'Primary Warehouse'. I can also check availability in other locations if needed.


## ❓ FAQ

**Q: How do I find my Fizzpa API Key?**
Log in to your Fizzpa dashboard and navigate to **Account Settings** > **API**. Copy the Bearer token displayed in your integration settings.

**Q: Can I print shipping labels directly via the agent?**
Yes! The `get_shipping_label` tool provides you with the direct URL to the label's PDF or image file for instant printing.

**Q: Does it support real-time inventory checking?**
Absolutely. The `list_inventory_levels` tool retrieves current stock counts across all your registered products and SKUs.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/fizzpa](https://vinkius.com/mcp/fizzpa)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Fizzpa** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `fizzpa` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Fizzpa** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "fizzpa": {
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
