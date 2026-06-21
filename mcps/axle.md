# Axle MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/axle)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [shipping-logistics](../categories/shipping-logistics.md)

Fleet management and logistics automation — track vehicles, manage drivers, and monitor loads via AI.

## Description
Empower your AI agent to orchestrate your entire logistics operation with **Axle**, the comprehensive fleet management platform. By connecting Axle to your agent, you transform complex supply chain monitoring into a natural conversation. Your agent can instantly track real-time vehicle locations, audit driver duty statuses, monitor shipment progress, and retrieve essential shipping documents without you ever touching a heavy transportation dashboard. Whether you're managing a local delivery crew or a national trucking network, your agent acts as a real-time dispatch coordinator, ensuring your fleet is always moving and compliant.

### What you can do

- **Vehicle Tracking** — List all vehicles in your fleet and retrieve real-time GPS locations and technical health details.
- **Driver Management** — Audit driver profiles, monitor current duty statuses (On Duty, Driving, etc.), and check available Hours of Service (HOS).
- **Load Orchestration** — Monitor shipment progress, list active loads, and update shipment details dynamically via natural language.
- **Document Retrieval** — Access scanned shipping documents and paperwork associated with specific loads for instant auditing.
- **System Health** — Quickly verify connection status and logistics network integrity directly from your chat interface.

### How it works

1. Subscribe to this server
2. Enter your Axle API Key and Base URL
3. Start managing your fleet operations through Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Fleet Managers** — monitor vehicle locations and driver availability in real-time through natural language.
- **Logistics Coordinators** — audit load statuses and verify delivery documentation without manual dashboard logins.
- **Compliance Officers** — perform rapid checks on driver Hours of Service (HOS) to ensure regulatory safety.
- **Operations Leads** — identify shipment bottlenecks and optimize dispatch workflows directly from chat.


## Available Tools (12)
- **get_account_check**: Verify Axle connection and system health
- **get_driver_availability**: Check a driver remaining hours of service (HOS)
- **get_driver**: Get specific profile details for a driver
- **get_load**: Get details for a specific load
- **get_vehicle_location**: Get the last known GPS location of a vehicle
- **get_vehicle**: Get specific details for a single vehicle
- **list_documents**: Retrieve scanned shipping documents associated with shipments
- **list_drivers**: List all drivers in the system
- **list_loads**: List all shipments/loads
- **list_vehicles**: List all vehicles in the fleet
- **update_driver_status**: Update a driver current duty status
- **update_load**: Update a load/shipment details


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Axle** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Where is vehicle ID 'TRUCK-101' right now?"

**🤖 AI Agent:**
> Checking GPS location for TRUCK-101... The vehicle was last seen 2 minutes ago at 123 Main St, moving at 45 mph heading North.

---

**👤 You:**
> "List all active loads and their current status."

**🤖 AI Agent:**
> I've retrieved 5 active loads. Load #9876 is 'In Transit' to Chicago, while Load #5432 is 'Pending Dispatch'. Would you like full details for any of them?

---

**👤 You:**
> "Check the available Hours of Service (HOS) for driver 'John Doe'."

**🤖 AI Agent:**
> Driver John Doe has 4 hours and 15 minutes of drive time remaining for today. His current duty status is 'Driving'.


## ❓ FAQ

**Q: How can I check if a vehicle is currently moving?**
Use the `get_vehicle_location` tool. It returns the last known GPS coordinates, speed, and heading for the specified vehicle ID.

**Q: Can I update a driver's status through the agent?**
Yes. Use the `update_driver_status` tool and provide the new duty status (e.g., 'On Duty', 'Driving', or 'Off Duty') to keep your logs accurate.

**Q: How do I access shipping documents for a load?**
Use the `list_documents` tool. It retrieves all scanned paperwork associated with your shipments, allowing your agent to audit or summarize the contents.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/axle](https://vinkius.com/mcp/axle)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Axle** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `axle` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Axle** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "axle": {
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
