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


## Available Tools
- **get_sale_order_details**: Get details for a specific sale order
- **get_product_stock**: Get current stock levels for a specific product
- **list_consignments**: List transport consignments
- **list_logistics_customers**: List customers associated with the tenant
- **list_logistics_invoices**: List generated invoices for logistics services
- **list_warehouse_products**: List warehouse products and master data
- **list_purchase_orders**: List inbound purchase orders
- **list_sale_orders**: List outbound sale orders


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

**Q: Can I check stock levels for a specific SKU?**
Yes! Use the `get_product_stock` tool with the product's unique ID. The agent will return the current available quantities across your warehouses.

**Q: How do I see all pending sale orders?**
Use the `list_sale_orders` tool. Your agent will fetch the list of outbound orders along with their current status and customer information.

**Q: Which regions does this integration support?**
It supports all CartonCloud regions. You just need to specify your region subdomain (e.g., `api-au` for Australia, `api-us` for United States) during setup.


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
3. Set Type to "SSE", enter `cartoncloud` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
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
