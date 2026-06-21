# DCL Logistics MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/dcl-logistics)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [ecommerce](../categories/ecommerce.md)

Equip your AI agent to manage order fulfillment, track shipments, and monitor warehouse inventory via the DCL Logistics API.

## Description
Integrate **DCL Logistics**, the leader in third-party logistics (3PL) and fulfillment, directly into your AI workflow. Manage your fulfillment orders, track shipments in real-time, and monitor warehouse inventory levels using natural language.

### What you can do

- **Order Oversight** — List and retrieve detailed statuses for all your fulfillment orders across DCL facilities.
- **Shipment Tracking** — Track recent shipments, access carrier details, and monitor delivery progress.
- **Inventory Management** — Check real-time stock levels for your SKUs and identify low-stock items.
- **Return Processing** — Monitor customer returns (RMAs) and their processing status directly via chat.

### How it works

1. Connect the DCL Logistics integration to your AI assistant.
2. Authorize using your DCL API Key and Account ID (found in your eFactory portal).
3. Orchestrate your supply chain and fulfillment operations through intuitive conversation.

### Who is this for?

- **E-commerce Brands** — Quickly check order statuses and stock levels during peak seasons.
- **Operations Managers** — Monitor shipment delays and warehouse inventory via chat.
- **Customer Support Teams** — Gather tracking information and return statuses for customer inquiries.


## Available Tools
- **get_account_details**: Returns account-level metadata such as company name, service tier, and active warehouse assignments.

Retrieve metadata for your DCL Logistics account
- **get_sku_inventory_status**: Provides a detailed breakdown of inventory status, including warehouse locations and any pending stock movements.

Get current stock level and status for a specific SKU
- **get_order_details**: Resolves line item details, recipient addresses, and the complete audit trail of order processing events.

Get detailed information for a specific order
- **get_shipment_details**: Resolves carrier-level status updates, estimated delivery dates, and proof of delivery (if available).

Get tracking and shipping details for a specific shipment ID
- **list_warehouse_inventory**: Returns a list of SKUs with their total on-hand, available, and reserved quantities.

List current inventory levels across all items
- **list_low_stock_items**: Identifies SKUs where the available quantity has fallen below the defined reorder point (e.g., < 10 units).

Identify items with inventory levels below a threshold (mock logic)
- **list_fulfillment_orders**: Returns order metadata including system IDs, current fulfillment status, and customer identifiers.

List all fulfillment orders in your DCL account
- **list_customer_returns**: Returns a list of Return Merchandise Authorizations (RMAs) including return reason, status of the returned goods, and credit processing info.

List all processed and pending customer returns (RMAs)
- **list_recent_shipments**: Returns a collection of shipment objects with associated carrier info, tracking numbers, and departure timestamps.

List all shipments processed by DCL
- **search_orders_by_keyword**: Matches keywords against order references, customer names, and shipping addresses to isolate specific fulfillment records.

Search for orders using a keyword or customer name


## 💬 Prompt Examples

Here are some examples of how you can interact with the **DCL Logistics** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all fulfillment orders that are 'Awaiting Shipment'."

**🤖 AI Agent:**
> I've found 15 orders awaiting shipment, including 'Order #EF123' and 'Order #EF124'. Most are scheduled to ship later today. Would you like to see the SKU breakdown for these orders?

---

**👤 You:**
> "What is the inventory status for SKU 'WR-9988'?"

**🤖 AI Agent:**
> SKU 'WR-9988' currently has 45 units in stock at the Fremont facility and 12 units at the Kentucky facility. There are 5 units reserved for pending orders. Should I check if there are any inbound shipments for this SKU?

---

**👤 You:**
> "Show me the tracking details for shipment 'SHP-1001'."

**🤖 AI Agent:**
> Shipment 'SHP-1001' was shipped via UPS Ground on June 12th. The current status is 'Out for Delivery' in Chicago, IL. The estimated arrival is by 5:00 PM today. Would you like the tracking link?


## ❓ FAQ

**Q: How do I get a DCL Logistics API Key?**
Log in to your DCL Logistics eFactory portal and navigate to the API settings or Integrations section to generate your API Key and find your Account ID.

**Q: Is inventory data real-time?**
Yes, this integration retrieves real-time stock levels directly from DCL warehouse management systems, providing accurate data for your planning.

**Q: Can the agent process new RMAs?**
This integration currently focuses on monitoring existing orders, shipments, and returns. Initiating new fulfillment orders or RMAs should be handled via the eFactory dashboard.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/dcl-logistics](https://vinkius.com/mcp/dcl-logistics)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **DCL Logistics** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `dcl-logistics` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **DCL Logistics** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "dcl-logistics": {
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
