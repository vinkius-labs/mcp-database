# Volvo Cars Connected MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/volvo-cars-connected)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [industry-titans](../categories/industry-titans.md)

Monitor and manage your connected Volvo vehicle — check fuel levels, battery status, door locks, and trip statistics directly via AI.

## Description
Connect your AI agent to the **Volvo Cars Connected Vehicle API**. This integration allows you to interact with your Volvo vehicle in real-time, retrieving essential telemetry data and status updates through natural conversation.

### What you can do

- **Vehicle Oversight** — List all vehicles associated with your Volvo ID and get detailed metadata for each (VIN, Model, Year)
- **Real-time Status** — Check battery levels for EVs/Hybrids, fuel levels for ICE vehicles, and estimated distance to empty
- **Security Monitoring** — Verify if doors and windows are locked/closed without opening the app
- **Health Checks** — Monitor tire pressure status and engine states across your fleet
- **Operational Metrics** — Retrieve odometer readings and trip statistics to track usage and efficiency

### How it works

1. Subscribe to this server
2. Enter your **Volvo Access Token** (obtained via Volvo ID OAuth) and **VCC API Key**
3. Start managing your vehicle or fleet directly through chat

### Who is this for?

- **Volvo Owners** — quickly check car status while planning your day
- **Fleet Managers** — monitor the health and usage of multiple Volvo vehicles
- **Tech Enthusiasts** — build automated workflows based on real-time vehicle telemetry


## Available Tools (10)
- **get_battery_status**: Retrieve the current battery level and charging status
- **get_doors_status**: Check if doors are locked or unlocked
- **get_engine_status**: Check the current state of the engine
- **get_fuel_status**: Retrieve the current fuel level and range
- **get_odometer**: Retrieve the current odometer reading
- **get_vehicle_statistics**: Retrieve usage statistics and trip meter data
- **get_tires_status**: Check the pressure status of all tires
- **get_vehicle_details**: Get comprehensive metadata for a specific vehicle
- **get_windows_status**: Check if windows are open or closed
- **list_vehicles**: Retrieve a list of all vehicles associated with the Volvo ID


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Volvo Cars Connected** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is the battery level of my Volvo?"

**🤖 AI Agent:**
> Checking your vehicle... Your Volvo (VIN: ...123) has a 78% battery charge remaining, with an estimated range of 320 km.

---

**👤 You:**
> "Are my car doors locked?"

**🤖 AI Agent:**
> Status update: All doors on your vehicle are currently LOCKED and secure.


## ❓ FAQ

**Q: How do I get a VCC API Key?**
You must register at the [**Volvo Cars Developer Portal**](https://developer.volvocars.com/), create an application, and subscribe to the 'Connected Vehicle API' to receive your key.

**Q: Where do I get the Access Token?**
The access token is generated via the Volvo ID authentication flow (OAuth 2.0). You can use tools like Postman or the Volvo portal's interactive documentation to generate a test token for your Volvo ID.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/volvo-cars-connected](https://vinkius.com/mcp/volvo-cars-connected)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Volvo Cars Connected** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `volvo-cars-connected` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Volvo Cars Connected** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "volvo-cars-connected": {
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
