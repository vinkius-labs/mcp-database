# Omnitracs Fleet Intelligence MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/omnitracs-fleet-intelligence)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [supply-chain](../categories/supply-chain.md)

Manage your fleet and logistics via Omnitracs — track vehicles, drivers, and shipments directly from your AI agent.

## Description
Connect your **Omnitracs** account to your AI agent and streamline your fleet management and logistics operations through natural conversation and real-time data access.

### What you can do

- **Vehicle Tracking** — List all fleet vehicles and retrieve current GPS locations and statuses in real-time.
- **Driver Oversight** — Access a list of all registered drivers and check their current duty statuses and profile details.
- **Route Management** — View active and scheduled transport routes and inspect detailed stops for any route.
- **Shipment Monitoring** — Track active shipments and cargo, and retrieve estimated delivery times and statuses.
- **Performance Analytics** — Access aggregated fleet performance metrics, including fuel efficiency and safety data.
- **Dispatch Messaging** — List recent messages exchanged between dispatch and vehicles/drivers for operational oversight.
- **Deep Inspection** — Fetch complete metadata for specific vehicles, drivers, or routes using their unique IDs.

### How it works

1. Subscribe to this server
2. Enter your Omnitracs API Key
3. Start managing your fleet intelligence from Claude, Cursor, or any MCP client

### Who is this for?

- **Fleet Managers** — quickly check vehicle locations or driver statuses without opening the tracking portal.
- **Logistics Coordinators** — monitor shipment progress and route completion through natural language.
- **Operations Leads** — automate the retrieval of fleet performance metrics for daily briefings.


## Available Tools (10)
- **get_driver_details**: Get specific driver info
- **get_route_stops**: List stops for a specific route
- **get_shipment_status**: Get specific shipment status
- **get_vehicle_location**: Get vehicle GPS location
- **list_fleet_drivers**: List all registered drivers
- **list_fleet_messages**: List recent fleet messages
- **get_fleet_performance**: Get fleet performance metrics
- **list_active_routes**: List active fleet routes
- **list_fleet_shipments**: List active shipments
- **list_fleet_vehicles**: List all fleet vehicles


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Omnitracs Fleet Intelligence** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all vehicles currently in my fleet."

**🤖 AI Agent:**
> Retrieving fleet vehicles... I found 25 vehicles registered. Notable units include 'Truck-101' (Active), 'Van-202' (Maintenance), and 'Trailer-303'. Would you like the current GPS location for Truck-101?

---

**👤 You:**
> "Where is driver 'John Doe' right now?"

**🤖 AI Agent:**
> Fetching driver status... John Doe is currently operating vehicle 'Truck-101'. His last reported location was near Chicago, IL, at 10:45 AM. He is currently 'On Duty' and has 4 hours remaining in his shift. Shall I list his assigned stops for today?

---

**👤 You:**
> "Show me the performance report for the fleet this week."

**🤖 AI Agent:**
> Generating performance report... For this week, your fleet averaged 6.5 MPG with a total idle time of 12%. You had 2 safety alerts for hard braking. Would you like to see which vehicles contributed most to the idle time?


## ❓ FAQ

**Q: How do I get an Omnitracs API Key?**
You can obtain an API key by contacting your Omnitracs account representative or through the Omnitracs Customer Portal under the API/Integration settings section.

**Q: Can I see real-time GPS locations?**
Yes! Use the `get_vehicle_location` tool with a specific vehicle ID to retrieve the latest reported GPS coordinates and status.

**Q: What metrics are included in fleet performance?**
Performance metrics typically include fuel consumption data, engine hours, safety events (like hard braking), and overall idle time across the fleet.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/omnitracs-fleet-intelligence](https://vinkius.com/mcp/omnitracs-fleet-intelligence)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Omnitracs Fleet Intelligence** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `omnitracs-fleet-intelligence` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Omnitracs Fleet Intelligence** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "omnitracs-fleet-intelligence": {
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
