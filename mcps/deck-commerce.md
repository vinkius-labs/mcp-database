# Deck Commerce MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/deck-commerce)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [ecommerce](../categories/ecommerce.md)

Equip your AI agent to manage order fulfillment, track shipments, and monitor inventory via the Deck Commerce API.

## Description
Integrate **Deck Commerce**, the leading order management system (OMS) for direct-to-consumer retailers, directly into your AI workflow. Manage your customer orders, track real-time inventory levels across facilities, and monitor shipments and returns using natural language.

### What you can do

- **Order Oversight** — List and retrieve detailed information for all customer orders and their current processing status.
- **Inventory Intelligence** — Access real-time stock levels for your SKUs and monitor backordered items.
- **Shipment Tracking** — Track processed shipments, access tracking numbers, and monitor delivery progress.
- **Return Management** — List customer returns and monitor their status directly via chat.

### How it works

1. Connect the Deck Commerce integration to your AI assistant.
2. Authorize using your Deck Commerce API Key and Site ID (found in your admin portal).
3. Optimize your omnichannel operations and fulfillment through intuitive conversation.

### Who is this for?

- **E-commerce Operations** — Quickly check order statuses and stock availability across multiple nodes.
- **Logistics Managers** — Monitor shipment progress and identify fulfillment bottlenecks via chat.
- **Customer Service Teams** — Gather tracking info and return details for customer inquiries instantly.


## Available Tools (10)
- **get_order_details**: Resolves line item details, shipping addresses, tax information, and the full order history trail.

Get detailed information for a specific order
- **get_shipment_tracking**: Resolves carrier status updates, delivery estimates, and current shipment location.

Get tracking and shipping details for a specific shipment
- **list_backordered_items**: Identifies products where demand exceeds current on-hand availability.

List all items currently on backorder (mock logic)
- **list_available_inventory**: Returns a list of SKUs with their total available-to-sell, on-hand, and reserved quantities across all nodes.

List current inventory levels across all items
- **list_oms_orders**: Returns order metadata including order numbers, current status, and customer identifiers.

List all customer orders in your Deck Commerce OMS
- **list_order_returns**: Returns a list of return requests including return reasons, RMA numbers, and current processing state.

List all customer returns and their processing status
- **get_account_metadata**: Returns account-level metadata such as organization name, active integrations, and system configuration.

Retrieve settings and metadata for your Deck Commerce account
- **get_sku_stock_level**: Provides a detailed breakdown of quantities at individual fulfillment nodes and identifies current inventory status.

Get current stock level and status for a specific SKU
- **list_processed_shipments**: Returns shipment metadata including carrier information, tracking numbers, and fulfillment timestamps.

List all shipments processed by Deck Commerce
- **search_orders_by_number**: Matches keywords against order numbers, customer names, and email addresses to isolate specific OMS records.

Search for orders using an order number or customer info


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Deck Commerce** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all customer orders from today that are 'Pending'."

**🤖 AI Agent:**
> I've found 8 pending orders from today, including 'Order #DC123' and 'Order #DC124'. All are awaiting inventory verification. Would you like to see the items in the largest pending order?

---

**👤 You:**
> "What is the stock level for 'Blue Runner Shoes' (SKU: RUN-99)?"

**🤖 AI Agent:**
> The SKU 'RUN-99' (Blue Runner Shoes) currently has 45 units available across all facilities. 30 units are in the 'Main Node' and 15 are in 'Regional Node 2'. Should I check if there are any backorders for this SKU?

---

**👤 You:**
> "Show me the tracking info for Order #DC123."

**🤖 AI Agent:**
> Order #DC123 was shipped via FedEx on June 12th. The tracking number is 1234567890. The current status is 'Delivered' in New York, NY. Would you like the full shipment history?


## ❓ FAQ

**Q: How do I get Deck Commerce API credentials?**
Log in to your Deck Commerce admin portal, navigate to the API settings or Integrations section to generate your API Key and find your Site ID.

**Q: Can the agent check backordered items?**
Yes, you can use the list_backordered_items tool to identify which SKUs are currently on backorder and monitor their fulfillment status.

**Q: Does the integration support tracking numbers?**
Yes, when retrieving shipment details, the agent provides carrier information and tracking numbers for your customer orders.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/deck-commerce](https://vinkius.com/mcp/deck-commerce)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Deck Commerce** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `deck-commerce` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Deck Commerce** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "deck-commerce": {
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
