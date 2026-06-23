# DROPBOY MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/dropboy)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [erp-operations](../categories/erp-operations.md)

Equip your AI agent to manage logistics orders, track fleet vehicles, and monitor delivery drivers via the DROPBOY API.

## Description
Integrate **DROPBOY**, the advanced logistics and delivery management platform, directly into your AI workflow. Manage your inbound and outbound delivery orders, track fleet vehicles and their operational status, monitor driver assignments and route history, and oversee your entire logistics operation using natural language.

### What you can do

- **Order Oversight** — List and retrieve detailed information and real-time status for all your logistics and delivery orders.
- **Fleet Intelligence** — Monitor fleet vehicles, including types, capacities, and current operational statuses across your organization.
- **Driver Management** — Track driver profiles, contact details, and active vehicle assignments to ensure efficient fulfillment.
- **Logistics Auditing** — Retrieve high-level summaries of fleet activity, delivery success rates, and active in-progress shipments.

### How it works

1. Connect the DROPBOY integration to your AI assistant.
2. Authorize using your DROPBOY API Key (found in your platform settings).
3. Orchestrate your logistics management and fleet optimization through intuitive conversation.

### Who is this for?

- **Logistics Managers** — Quickly check order statuses and vehicle availability on the go.
- **Fleet Operations** — Monitor driver assignments and route progress via chat.
- **Supply Chain Teams** — Research specific delivery details and organizational logistics metadata instantly.


## Available Tools (10)
- **get_dropboy_account_metadata**: Retrieve metadata and limits for your DROPBOY account
- **get_driver_profile**: Get full profile and route history for a specific driver
- **get_order_details**: Get detailed information and real-time status for a specific order
- **quick_fleet_status_audit**: Retrieve a high-level summary of fleet activity and vehicle availability
- **list_fleet_drivers**: List all drivers registered in your DROPBOY organization
- **list_active_deliveries**: Identify orders that are currently in the "In Progress" or "Out for Delivery" status
- **list_logistics_orders**: List all logistics and delivery orders in your DROPBOY account
- **list_latest_logistics_orders**: Identify the most recently created delivery orders
- **list_fleet_vehicles**: List all vehicles registered in your DROPBOY fleet
- **search_logistics_orders**: Search for orders using an order number or delivery address


## 💬 Prompt Examples

Here are some examples of how you can interact with the **DROPBOY** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all active delivery orders."

**🤖 AI Agent:**
> I've found 8 active orders, including 'ORD-123' (In Progress) and 'ORD-456' (Dispatched). Would you like to see the delivery address for ORD-123?

---

**👤 You:**
> "Show me the status of our fleet vehicles."

**🤖 AI Agent:**
> Currently, you have 5 vehicles 'In Operation', 2 'Available', and 1 'In Maintenance'. Vehicles include 3 Heavy Trucks and 5 Delivery Vans. Should I pull the driver assignment for the active trucks?

---

**👤 You:**
> "Search for order 'ORD-9988'."

**🤖 AI Agent:**
> Order 'ORD-9988' is currently 'In Progress' and assigned to driver 'Mark Thompson'. The delivery address is '123 Business Way, New York'. ETA is 2:30 PM. Should I pull the itemized cargo list?


## ❓ FAQ

**Q: How do I get a DROPBOY API Key?**
Log in to your DROPBOY platform account, navigate to **Settings > Integrations** or the **API** section, and you can generate or retrieve your unique API Key from there. Ensure you have the necessary administrative permissions.

**Q: Can the agent track vehicles in real-time?**
Yes, you can use the list_fleet_vehicles or get_order_details tools to retrieve the current operational status and location data for your fleet assets.

**Q: Does the integration support driver route history?**
Yes, the get_driver_profile tool allows you to retrieve granular profile details and the history of assigned routes for specific drivers in your fleet.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/dropboy](https://vinkius.com/mcp/dropboy)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **DROPBOY** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `dropboy` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **DROPBOY** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "dropboy": {
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
