# Extensiv MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/extensiv)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [ecommerce](../categories/ecommerce.md)

Manage omnichannel operations via Extensiv — track orders and shipments, monitor inventory and warehouses, and manage vendors directly from any AI agent.

## Description
Connect your **Extensiv** (formerly Skubana) account to any AI agent and take full control of your omnichannel e-commerce operations and inventory management through natural conversation.

### What you can do

- **Order Orchestration** — List and filter omnichannel orders to retrieve order numbers, statuses, channel mappings, and line items natively
- **Inventory Auditing** — Monitor current stock levels across all warehouses, including available, committed, on-order, and in-transit quantities
- **Warehouse Management** — Retrieve configurations for 3PL and in-house warehouses, identifying addresses and capability settings flawlessly
- **Supply Chain Oversight** — List purchase orders (POs) and track vendor shipments, expected delivery dates, and receiving statuses securely
- **Product Master Data** — Access core product details including SKUs, dimensions, weights, and costs to manage your catalog metadata
- **Vendor & Brand Control** — Manage supplier contact details, lead times, and payment terms, and list all product brands configured in the system
- **Return & RMA Tracking** — Monitor return merchandise authorizations with reason codes, status updates, and linked refund amounts in real-time
- **Customer Intelligence** — Retrieve customer profiles with shipping addresses and order history summaries to resolve inquiries limitlessly

### How it works

1. Subscribe to this server
2. Enter your Extensiv API Access Token (obtained via OAuth or from your App details)
3. Start managing your omnichannel operations from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **E-commerce Ops Managers** — monitor inventory levels and track shipments across multiple channels using natural language
- **Inventory Coordinators** — audit warehouse stock and manage purchase orders without opening the Extensiv dashboard
- **Customer Support Teams** — quickly look up order statuses and customer histories to resolve inquiries in real-time
- **Supply Chain Analysts** — track vendor performance and monitor lead times through natural conversation


## Available Tools
- **list_orders**: 1/orders with pagination. Returns orders with order number, status, channel, shipping address, line items, and fulfillment tracking. Pass limit to control page size (default 100).

List Extensiv/Skubana orders
- **list_products**: 1/products with pagination. Returns product master data including SKU, name, dimensions, weight, cost, and linked vendor information.

List Extensiv products
- **list_inventory**: 1/inventory with pagination. Returns current stock levels by warehouse and product, including available, committed, on-order, and in-transit quantities.

List Extensiv inventory levels
- **list_warehouses**: 1/warehouses. Returns all configured 3PL and in-house warehouses with name, address, type, and capability settings. No parameters required.

List Extensiv warehouses
- **list_pos**: 1/purchaseorders with pagination. Returns PO number, vendor, expected date, line items with SKU and quantity, and receiving status.

List Extensiv purchase orders
- **list_vendors**: 1/vendors. Returns all configured vendors with name, contact details, lead time, currency, and payment terms. No parameters required.

List Extensiv vendors/suppliers
- **list_shipments**: 1/shipments with pagination. Returns shipment tracking details including carrier, tracking number, ship date, delivery status, and linked order references.

List Extensiv shipments
- **list_rmas**: 1/rmas with pagination. Returns return merchandise authorizations with reason code, status, linked order, refund amount, and items being returned.

List Extensiv returns (RMAs)
- **list_brands**: 1/brands. Returns all product brands configured in the system with brand name and description. No parameters required.

List Extensiv brands
- **list_customers**: 1/customers with pagination. Returns customer profiles with name, email, phone, shipping address, and order history summary.

List Extensiv customers


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Extensiv** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List the last 5 orders from my Shopify channel"

**🤖 AI Agent:**
> Retrieving Shopify orders... I found 5 recent orders including #SH-1001 (Processing) and #SH-1002 (Shipped). Would you like to see the line items for the most recent order?

---

**👤 You:**
> "What is the available stock for SKU 'TSHIRT-BLU-L' at the Main Warehouse?"

**🤖 AI Agent:**
> Checking inventory for 'TSHIRT-BLU-L'... In the Main Warehouse, you have 45 units available, 10 committed to pending orders, and 25 currently in transit from the supplier.

---

**👤 You:**
> "Show me the status of purchase order PO-999"

**🤖 AI Agent:**
> Retrieving PO details... Purchase Order PO-999 for vendor 'Global-Fabrics' is currently 'Awaiting Receipt'. It includes 500 units of cotton fabric and is expected to arrive on 2024-05-15.


## ❓ FAQ

**Q: Can my agent list inventory levels across different warehouses?**
Yes. Use the 'list_inventory' tool. The agent retrieves current stock levels by warehouse and product, including available, committed, and in-transit quantities natively.

**Q: How do I track a specific shipment through the agent?**
Use the 'list_shipments' tool. Your agent will pull shipment tracking details including the carrier, tracking number, ship date, and delivery status for linked orders.

**Q: Can I audit purchase orders from my suppliers via chat?**
Absolutely. The 'list_pos' tool retrieves PO numbers, vendor names, expected delivery dates, and line item details, allowing you to monitor your supply chain replenishment natively.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/extensiv](https://vinkius.com/mcp/extensiv)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Extensiv** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `extensiv` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Extensiv** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "extensiv": {
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
