# VTEX Orders MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/vtex-orders)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [ecommerce](../categories/ecommerce.md)

Search, track, invoice, and cancel orders on your VTEX store — manage your entire order lifecycle from any AI agent.

## Description
Connect your **VTEX** Order Management System (OMS) to any AI agent and take full control of your store's order lifecycle through natural conversation.

### What you can do

- **Order Lookup** — Retrieve the full details of any order by ID, including items, client profile, payment method, logistics, and current status.
- **Order Search** — Search and filter orders by status (e.g., 'ready-for-handling', 'invoiced', 'canceled') with built-in pagination for large result sets.
- **Status Updates** — Advance orders through the fulfillment pipeline by updating their status (e.g., move from 'ready-for-handling' to 'handling').
- **Shipment Tracking** — Retrieve tracking information for shipped packages, including carrier, tracking number, and tracking URL.
- **Invoice Registration** — Attach tax invoices (NF-e) and tracking numbers to orders, automatically moving them to 'Invoiced' status.
- **Order Cancellation** — Cancel orders with an optional reason, triggering automatic refund processing.

### How it works

1. Subscribe to this server
2. Enter your VTEX Account Name, App Key, and App Token (found in **Account Settings → Application Keys** in your VTEX Admin)
3. Start managing orders from Claude, Cursor, or any MCP-compatible agent

### Who is this for?

- **Fulfillment Teams** — Track order queues, update statuses, and register invoices without navigating the VTEX Admin.
- **Customer Support** — Instantly look up order details, check tracking, or process cancellations during live conversations.
- **Operations Managers** — Monitor order flow, identify bottlenecks, and audit fulfillment performance across sellers.


## Available Tools
- **cancel_order**: Cancel an order
- **get_order**: Get full details of a specific order
- **register_invoice**: Register a tax invoice and tracking number
- **search_orders**: g., "ready-for-handling").

Search for orders by status or pagination
- **update_order_status**: Update the status of an order
- **get_tracking_info**: Get tracking info for an order package


## 💬 Prompt Examples

Here are some examples of how you can interact with the **VTEX Orders** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Show me the details of order v-1234567890"

**🤖 AI Agent:**
> Order **v-1234567890** found! Status: **Ready for Handling**.

👤 Customer: Maria Silva (maria@example.com)
📦 Items: 2x 'Nike Air Max 90' (SKU: 12345) — R$ 599.90 each
💳 Payment: Credit Card (Visa ending 4321)
🚚 Shipping: PAC (5-7 business days) to CEP 01310-100

**Total: R$ 1,212.30** (including R$ 12.50 shipping). Shall I move it to 'handling'?

---

**👤 You:**
> "List all orders with status 'ready-for-handling'"

**🤖 AI Agent:**
> Found **23 orders** in 'ready-for-handling' status. Here are the first 5:

1. **v-111** — Maria Silva, R$ 299.90 (1 item)
2. **v-222** — João Souza, R$ 1,450.00 (3 items)
3. **v-333** — Ana Lima, R$ 89.90 (1 item)
4. **v-444** — Pedro Santos, R$ 2,100.00 (2 items)
5. **v-555** — Carla Fernandes, R$ 450.00 (1 item)

Would you like to move any of these to 'handling' status?

---

**👤 You:**
> "Cancel order v-444 — customer requested wrong size"

**🤖 AI Agent:**
> Order **v-444** has been canceled. Reason logged: 'Customer requested wrong size'. The payment refund of R$ 2,100.00 has been automatically initiated via the original payment method (Credit Card). The customer will receive the refund within 5-10 business days.


## ❓ FAQ

**Q: How do I get my VTEX API credentials?**
Log in to your VTEX Admin, go to **Account Settings → Application Keys**, and create a new App Key. You'll receive an App Key and App Token pair. You also need your Account Name (the subdomain you use to access the VTEX Admin, e.g., 'mystore'). Ensure the key has **OMS** read/write permissions. No code, no SDK — just connect and go.

**Q: Can my agent register an invoice and tracking number at the same time?**
Yes! The 'register_invoice' tool accepts the invoice number and an optional tracking number in one call. Once submitted, the order automatically moves to 'Invoiced' status — eliminating the manual step of navigating to the VTEX Admin, opening the order detail, and filling each field separately.

**Q: How does the agent handle order cancellations with refunds?**
Just tell your agent to cancel the order. It uses the 'cancel_order' tool with an optional reason (so your team has an audit trail). VTEX then handles the refund automatically based on the payment method. No tab-switching, no admin navigation — your support team resolves it in one conversation.

**Q: Can I monitor fulfillment status across hundreds of orders?**
Absolutely. The 'search_orders' tool supports status filters and pagination, so your agent can scan the entire order queue — for example, listing all orders stuck in 'ready-for-handling' to identify fulfillment delays. Perfect for operations teams managing high-volume VTEX stores with multiple sellers.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/vtex-orders](https://vinkius.com/mcp/vtex-orders)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **VTEX Orders** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `vtex-orders` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **VTEX Orders** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "vtex-orders": {
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
