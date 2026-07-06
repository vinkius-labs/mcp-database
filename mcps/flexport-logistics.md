# Flexport Logistics MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/flexport-logistics)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [ecommerce](../categories/ecommerce.md)

Manage e-commerce fulfillment, inventory, and returns via AI agents with Flexport Logistics.

## Description
Connect your **Flexport Logistics** account to any AI agent and automate your e-commerce fulfillment and warehousing operations through the Model Context Protocol (MCP). Flexport Logistics (formerly Deliverr) provides a high-speed fulfillment network that ensures your customers get their orders fast. Now, you can manage orders, track real-time inventory, and handle returns directly through natural conversation.

### What you can do

- **Order Fulfillment** — Create and track fulfillment orders for your end customers across multiple sales channels.
- **Real-time Inventory** — Check current stock levels across the entire Flexport warehouse network to avoid stockouts.
- **Inbound Management** — List and monitor inbound shipments of inventory being sent to warehouses.
- **Product Catalog** — Access your fulfillment product library and fetch detailed metadata for specific SKUs.
- **Return Handling** — Manage customer return requests and track the status of returned items.
- **Shipping Labels** — List and retrieve purchased parcel shipping labels for your e-commerce shipments.
- **Warehouse Network** — Get visibility into the active warehouses in the Flexport fulfillment network.

### How it works

1. Subscribe to this server through the Vinkius Marketplace
2. Enter your Flexport Logistics API Key (found in your Logistics Portal settings)
3. Start managing your e-commerce operations from Claude, Cursor, or any MCP client

### Who is this for?

- **E-commerce Merchants** — quickly check if a specific SKU is in stock or track a customer's fulfillment order.
- **Warehouse Operations** — get a real-time overview of inbound shipments and inventory arrivals via simple AI commands.
- **Customer Service Teams** — automate the retrieval of tracking numbers and return statuses to provide faster support.


## Available Tools (12)
- **get_warehouse_network**: List warehouses
- **list_inbounds**: List inbound shipments
- **list_inventory**: Check stock levels
- **list_labels**: List shipping labels
- **list_logistics_orders**: List fulfillment orders
- **list_products**: List product catalog
- **list_returns**: List customer returns
- **create_logistics_order**: Create fulfillment order
- **get_inbound**: Get inbound details
- **get_logistics_order**: Get order details
- **get_product**: Get product details
- **get_return**: Get return details


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Flexport Logistics** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Check the current inventory level for SKU 'SKU-999'."

**🤖 AI Agent:**
> Checking inventory... For SKU 'SKU-999', you have 150 units available across the network, with the largest concentration in the California fulfillment center.

---

**👤 You:**
> "List all fulfillment orders that were shipped today."

**🤖 AI Agent:**
> Retrieving orders... I found 12 fulfillment orders shipped today, including orders for 'Customer A' and 'Customer B'. Would you like the tracking numbers for these shipments?

---

**👤 You:**
> "Show me the status of my inbound shipment 'INB-123'."

**🤖 AI Agent:**
> Fetching inbound details... Shipment 'INB-123' is currently 'In Transit' and is expected to arrive at the warehouse by Friday. I'll notify you once it's been received and processed.


## ❓ FAQ

**Q: Can I check my inventory levels across all Flexport warehouses using the agent?**
Yes! The 'list_inventory' tool retrieves real-time stock data across the entire warehouse network, helping you manage SKU availability and prevent stockouts.

**Q: How do I track a customer's fulfillment order using this server?**
Use the 'get_logistics_order' tool and provide the Flexport Order ID or your external reference. The agent will return the fulfillment status and any available tracking numbers.

**Q: Can I manage product SKUs through the agent?**
Absolutely. The 'list_products' tool provides a view of your entire fulfillment catalog, while 'get_product' allows you to drill down into the metadata for a specific item.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/flexport-logistics](https://vinkius.com/mcp/flexport-logistics)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Flexport Logistics** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `flexport-logistics` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Flexport Logistics** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "flexport-logistics": {
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
