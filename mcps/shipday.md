# Shipday MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/shipday)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [industry-titans](../categories/industry-titans.md)

Dispatch and track local deliveries with driver management, route optimization, and real-time tracking for last-mile operations.

## Description
Connect your **Shipday** account to any AI agent and take full control of your last-mile delivery and dispatch orchestration through natural conversation. Shipday provides a premier platform for managing local delivery operations, and this integration allows you to retrieve order metadata, assign drivers, and track delivery progress directly from your chat interface.

### What you can do

- **Order & Dispatch Orchestration** — List all managed delivery orders and retrieve detailed metadata, including status and customer info programmatically.
- **Driver Lifecycle Management** — Access and monitor your driver directory and assign drivers to specific orders directly from the AI interface.
- **Delivery Progress Intelligence** — Retrieve real-time tracking progress for active orders to keep your customers informed via natural language.
- **Status Lifecycle Control** — Update order statuses and monitor carrier metadata to ensure your delivery pipeline is always synchronized.
- **Operational Monitoring** — Track system activity and monitor order fulfillment to ensure reliable last-mile orchestration using simple AI commands.

### How it works

1. Subscribe to this server
2. Enter your Shipday API Key from your dashboard settings
3. Start managing your local deliveries from Claude, Cursor, or any MCP-compatible client

No more juggling multiple delivery tabs to coordinate your fleet. Your AI acts as a dedicated dispatcher or delivery operations manager.

### Who is this for?

- **Restaurant & Retail Managers** — quickly dispatch orders and monitor driver availability without switching apps.
- **Delivery Operations Teams** — automate the assignment of drivers and track order progress via natural conversation.
- **Customer Support Teams** — streamline the retrieval of delivery status and monitor fulfillment directly within the chat.


## Available Tools
- **assign_driver**: Assign an order to a driver
- **create_order**: Provide orderNumber, customer details, and restaurant info.

Create a new delivery order
- **delete_order**: Delete/Cancel an order
- **get_carrier_order**: Get details for a carrier order
- **get_order**: Get details of a specific order
- **get_tracking_progress**: Get real-time tracking for a delivery
- **list_active_orders**: List all active delivery orders
- **list_drivers**: List all drivers
- **update_order_status**: Update the status of an order


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Shipday** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all active delivery orders in Shipday."

**🤖 AI Agent:**
> I've retrieved your active orders. You have 4 deliveries in progress: '#ORD-101' (Picked up), '#ORD-102' (Out for delivery), and two others. Would you like to see the driver tracking for any of them?

---

**👤 You:**
> "Assign driver ID 12345 to order ID 98765."

**🤖 AI Agent:**
> Assignment processed! Order 98765 is now assigned to 'Mike R.' (ID 12345). Should I notify the customer about the updated delivery status?

---

**👤 You:**
> "List all available drivers in Shipday."

**🤖 AI Agent:**
> Retrieving drivers... I found 6 active drivers in your fleet. 'Marcus' and 'Sarah' are currently idle and ready for dispatch. Would you like to see their contact info?


## ❓ FAQ

**Q: Can my AI automatically find the status of a delivery order just by providing its ID?**
Yes! Use the `get_order` tool with the Order ID. Your agent will respond with the current status, customer details, and scheduled delivery times in seconds.

**Q: How do I assign a specific driver to an active order?**
Simply ask the agent to run the `assign_driver` action. You will need to provide both the Order ID and the Driver ID to complete the assignment.

**Q: How do I find my Shipday API Key?**
Log in to your Shipday dashboard, navigate to **Settings** > **API**, and you will find your unique secret API key there.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/shipday](https://vinkius.com/mcp/shipday)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Shipday** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `shipday` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Shipday** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "shipday": {
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
