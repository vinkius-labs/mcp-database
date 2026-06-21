# Mercado Livre Orders MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/mercado-livre-orders)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [industry-titans](../categories/industry-titans.md)

Search sales, manage shipments, track packages, and handle cancellations on Mercado Livre.

## Description
Connect **Mercado Livre Orders** to any AI agent and take full control of your order management system — search sales, track shipments, register invoices, and handle cancellations through natural conversation.

### What you can do
- **Order Search** — Find sales by status (paid, shipping, delivered, cancelled)
- **Order Details** — Get full info on buyer, items, and totals for a specific sale
- **Shipping Management** — View shipping status, carrier info, and tracking codes
- **Tracking Updates** — Set tracking numbers for shipments handled outside Mercado Envios
- **Buyer Feedback** — Check ratings and comments left by buyers
- **Order Cancellation** — Cancel sales when necessary (requires valid reason)

### How it works
1. Subscribe to this server
2. Enter your Mercado Livre OAuth2 Access Token
3. Start managing orders from Claude, Cursor, or any MCP-compatible client

### Who is this for?
- **Sellers** — Monitor sales activity and shipping status without manual dashboard checks
- **Customer Support** — Quickly access order details and tracking info to answer buyer queries
- **Logistics Teams** — Register invoices and update tracking codes in bulk via AI


## Available Tools
- **cancel_order**: Requires a valid reason.

Cancel a sale
- **get_feedback**: Get buyer feedback/reputation for a sale
- **get_order**: Get details of a specific sale
- **search_orders**: Search for sales/orders
- **get_shipments**: List shipments associated with an order
- **get_shipping_info**: Get shipping details for an order
- **set_tracking**: Set tracking number for a shipment


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Mercado Livre Orders** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Show me all orders that need shipping."

**🤖 AI Agent:**
> Found 3 orders ready for shipping: 1. MLB-Order123 (R$150.00). 2. MLB-Order456 (R$89.90). 3. MLB-Order789 (R$210.00).

---

**👤 You:**
> "Get details for order MLB-Order123."

**🤖 AI Agent:**
> Order MLB-Order123: Status: Paid. Buyer: João Silva. Total: R$150.00. Item: Wireless Headphones.

---

**👤 You:**
> "Register invoice 9999 for shipment 12345 with tracking XYZ."

**🤖 AI Agent:**
> Invoice registered successfully! Tracking code XYZ set for shipment 12345.


## ❓ FAQ

**Q: How can I see all my pending orders?**
Use the `search_orders` tool with status set to 'paid' or 'handling'. It will return a list of orders ready to be shipped.

**Q: How do I update the tracking number for a shipment?**
Use the `set_tracking` action with the Order ID, Shipment ID, Carrier ID, and the Tracking Number.

**Q: Can I cancel a sale?**
Yes, use `cancel_order`. Be aware that cancelling orders can negatively impact your seller reputation metrics.

**Q: Can I register an invoice (Nota Fiscal) for a shipment?**
Absolutely. Use the `register_invoice` tool with the shipment ID, invoice number (NF-e key), and access key. This is required for sellers in Brazil to comply with tax regulations.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/mercado-livre-orders](https://vinkius.com/mcp/mercado-livre-orders)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Mercado Livre Orders** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `mercado-livre-orders` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Mercado Livre Orders** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "mercado-livre-orders": {
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
