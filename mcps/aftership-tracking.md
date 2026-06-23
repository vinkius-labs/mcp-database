# AfterShip Tracking MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/aftership-tracking)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [ecommerce](../categories/ecommerce.md)

Shipment tracking and logistics — track packages, manage couriers, and monitor deliveries via AI.

## Description
Connect your **AfterShip Tracking** account to your AI agent to unlock professional logistics orchestration and real-time delivery monitoring. From adding new tracking numbers across 600+ couriers to auditing shipment statuses and detecting carriers automatically, your agent handles your shipping operations through natural conversation.

### What you can do

- **Shipment Orchestration** — Create and manage tracking records for any package using tracking numbers and carrier slugs
- **Real-time Status Auditing** — Retrieve detailed technical metadata for shipments, including current location and delivery estimates
- **Courier Management** — List active couriers in your account and automatically detect the carrier for any tracking number
- **Logistics Oversight** — Monitor your entire shipping pipeline and identify delayed or exception shipments directly from chat
- **Delivery Insights** — Quickly retrieve historical tracking data to support customer inquiries and supply chain analysis

### How it works

1. Subscribe to this server
2. Enter your AfterShip API Key
3. Start tracking shipments and managing couriers through Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **E-commerce Operations** — automate tracking updates and monitor shipment exceptions across multiple carriers
- **Customer Support Teams** — quickly look up package locations and provide real-time updates to customers
- **Logistics Managers** — audit carrier performance and delivery success rates instantly
- **Sourcing & Supply Chain** — track inbound shipments from suppliers and identify potential disruptions


## Available Tools (5)
- **list_trackings**: g. InTransit).

Retrieve all active and historical tracked shipments currently monitored by AfterShip
- **create_tracking**: Register a new package tracking number to initiate real-time monitoring and webhooks via AfterShip
- **get_tracking_details**: Retrieve highly accurate real-time location updates and the current delivery status for an AfterShip tracking ID
- **list_couriers**: Retrieve the subset of shipping couriers that are currently actively enabled in your AfterShip account
- **detect_courier**: Analyze a raw tracking number format to automatically identify the likely carriers routing it


## 💬 Prompt Examples

Here are some examples of how you can interact with the **AfterShip Tracking** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Track this FedEx package: 123456789012."

**🤖 AI Agent:**
> I've added tracking for FedEx package 123456789012. It is currently 'In Transit' and is scheduled for delivery tomorrow by 8:00 PM. Would you like to be notified of any status changes?

---

**👤 You:**
> "Identify the carrier for tracking number '9400100000000000000000'."

**🤖 AI Agent:**
> Based on the format, this tracking number belongs to USPS. Would you like me to start monitoring this shipment for you?

---

**👤 You:**
> "Show me all shipments with an 'Exception' status."

**🤖 AI Agent:**
> I've filtered your shipments. You have 2 packages with an 'Exception' status, both due to incorrect address information. I've listed the details so you can contact the customers.


## ❓ FAQ

**Q: How do I add a new tracking number?**
Use the `create_tracking` tool and provide the tracking number and the courier slug (e.g., 'fedex', 'dhl'). Your agent will add it to AfterShip and start monitoring the status.

**Q: Can the agent automatically detect the courier?**
Yes! Use the `detect_courier` tool with any tracking number. AfterShip will analyze the format and return a list of potential carrier matches.

**Q: What tracking statuses are supported?**
AfterShip normalizes tracking data into standard statuses: Pending, In Transit, Out for Delivery, Delivered, Exception, and Failed Attempt.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/aftership-tracking](https://vinkius.com/mcp/aftership-tracking)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **AfterShip Tracking** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `aftership-tracking` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **AfterShip Tracking** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "aftership-tracking": {
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
