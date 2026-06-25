# CartonCloud MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/cartoncloud)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [erp-operations](../categories/erp-operations.md)

Manage warehouse and transport operations via CartonCloud — track orders, monitor stock, and manage consignments directly from any AI agent.

## Description
Connect your **CartonCloud** account to any AI agent and orchestrate your WMS (Warehouse Management System) and TMS (Transport Management System) through natural conversation. Streamline 3PL operations and inventory management.

### What you can do

- **Order Fulfillment** — List and retrieve details for outbound sale orders and inbound purchase orders natively
- **Inventory Visibility** — Monitor current stock levels by product and warehouse location in real-time
- **Transport Management** — List transport consignments and track delivery statuses securely
- **Master Data Control** — Access warehouse product details, including SKUs and unit of measure metadata
- **Customer Oversight** — List and manage customer profiles and associated logistics data flawlessly
- **Financial Auditing** — Retrieve generated invoices for logistics services directly within your workspace

### How it works

1. Subscribe to this server
2. Enter your CartonCloud Client ID, Client Secret, and Region subdomain
3. Start managing your logistics operations from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Warehouse Managers** — monitor stock levels and inbound shipments using natural language
- **Transport Coordinators** — track consignments and delivery progress without opening the dashboard
- **Logistics Administrators** — audit invoices and manage customer master data straight from their chat interface
- **3PL Operators** — automate routine logistics inquiries and reporting workflows


## Available Tools (8)
- **search_warehouse_products**: Returns product IDs, names, SKUs, and unit-of-measure metadata.

Search warehouse products and master data
- **get_consignment**: Get details for a specific transport consignment
- **get_customer**: Get details for a specific customer
- **get_inbound_order**: Get details for a specific inbound order (purchase order)
- **get_outbound_order**: Returns full order details including items, references, and delivery info.

Get details for a specific outbound order (sale order)
- **get_warehouse_product**: Get details for a specific warehouse product
- **get_account_info**: Get the authenticated user account information
- **list_customers**: Returns customer name and UUID.

List all customers associated with the tenant
- **list_transport_products**: List transport products available for consignments
- **search_consignments**: Returns consignment IDs, statuses, and delivery run info.

Search transport consignments in CartonCloud
- **search_inbound_orders**: Returns order ID, status, customer, warehouse, and arrival date.

Search inbound orders (purchase orders) in CartonCloud
- **search_outbound_orders**: Returns order ID, status, customer, warehouse, and timestamps.

Search outbound orders (sale orders) in CartonCloud


## 💬 Prompt Examples

Here are some examples of how you can interact with the **CartonCloud** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List my last 10 sale orders in CartonCloud."

**🤖 AI Agent:**
> Retrieving your recent sale orders... I found 10 orders including #SO-123 (Picking) and #SO-124 (Dispatched). Would you like the details for any specific order?

---

**👤 You:**
> "What is the current stock for product ID 555?"

**🤖 AI Agent:**
> Checking stock for product 555... You currently have 150 units available in the North Warehouse and 45 units in the South Warehouse.

---

**👤 You:**
> "Show me the transport consignments for today."

**🤖 AI Agent:**
> Retrieving today's consignments... I found 5 active shipments. 3 are 'Out for Delivery' and 2 are 'Booked'. Should I check the status of a specific tracking number?


## ❓ FAQ

**Q: How do I search for warehouse products?**
Use the `search_warehouse_products` tool. The agent will query your CartonCloud tenant and return a list of products with their SKU, name, and unit-of-measure metadata.

**Q: How do I see all my outbound orders?**
Use the `search_outbound_orders` tool. Your agent will search your outbound orders and return their status, customer, and warehouse details.

**Q: Which regions does this integration support?**
It supports all CartonCloud regions. Use `api.cartoncloud.com` for Global/APAC or `api.na.cartoncloud.com` for North America during setup.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/cartoncloud](https://vinkius.com/mcp/cartoncloud)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **CartonCloud** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `cartoncloud` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **CartonCloud** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "cartoncloud": {
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
