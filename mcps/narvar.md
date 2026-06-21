# Narvar MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/narvar)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [ecommerce](../categories/ecommerce.md)

Streamline post-purchase experiences — track shipments, manage returns, and provide delivery estimates directly through your AI agent.

## Description
Connect **Narvar** to your AI agent to take full control of the post-purchase customer journey. From real-time tracking to automated returns, manage every logistics touchpoint through natural conversation.

### What you can do

- **Shipment Tracking** — Get real-time status updates and event history for any carrier tracking number using `get_tracking`.
- **Returns Management** — Initiate return requests and generate labels for orders instantly with `create_return`.
- **Order Insights** — Retrieve comprehensive order details, line items, and fulfillment status using `get_order`.
- **Customer Notifications** — Trigger transactional Email or SMS notifications for shipment milestones with `trigger_notification`.
- **Delivery Estimates** — Calculate precise estimated delivery dates (EDD) for checkout optimization using `get_estimated_delivery_dates`.

### How it works

1. Subscribe to this server
2. Enter your Narvar API Key
3. Start managing logistics from Claude, Cursor, or any MCP-compatible client

No more switching between carrier portals and internal dashboards. Your AI acts as a dedicated logistics coordinator.

### Who is this for?

- **E-commerce Managers** — Monitor shipment health and order fulfillment across multiple carriers in one view.
- **Customer Support Teams** — Instantly answer "where is my order" queries and process returns without leaving the chat.
- **Logistics Operations** — Analyze delivery performance and trigger customer alerts for delays or successful deliveries.


## Available Tools
- **get_estimated_delivery_dates**: Uses POST but acts as a query.

Calculate estimated delivery dates (EDD)
- **create_return**: Initiate a return request for an order
- **trigger_notification**: Trigger a transactional notification
- **get_order**: Get comprehensive order details
- **get_tracking**: Get real-time tracking information for a shipment


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Narvar** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Track shipment 1Z999AA10123456789 for me."

**🤖 AI Agent:**
> I've retrieved the tracking for 1Z999AA10123456789. The package is currently 'In Transit' via UPS and is expected to arrive tomorrow by 7:00 PM. The last update was in Louisville, KY.

---

**👤 You:**
> "Get the details for order #ORD-5521."

**🤖 AI Agent:**
> Order #ORD-5521 contains 2 items: 'Wireless Headphones' and 'USB-C Cable'. The fulfillment status is 'Shipped' and it is linked to tracking number 9876543210.

---

**👤 You:**
> "Send a 'DELIVERED_CONFIRMATION' email to customer@example.com for order ORD-123."

**🤖 AI Agent:**
> I have triggered the 'DELIVERED_CONFIRMATION' notification for order ORD-123. It has been sent to customer@example.com via Email.


## ❓ FAQ

**Q: Can I track a package without knowing the carrier?**
Yes, although providing the carrier helps accuracy. Use `get_tracking` with the tracking number, and the system will attempt to retrieve the latest events from Narvar's network.

**Q: How do I generate a return label for a customer?**
Use the `create_return` tool. You will need to provide the order number, customer details, and the items being returned. The agent will then initiate the return flow in Narvar.

**Q: Can I get delivery estimates before an order is placed?**
Absolutely. Use the `get_estimated_delivery_dates` tool by providing the origin, destination, and items. This is perfect for showing accurate shipping times during checkout.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/narvar](https://vinkius.com/mcp/narvar)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Narvar** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `narvar` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Narvar** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "narvar": {
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
