# General Motors MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/general-motors)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [industry-titans](../categories/industry-titans.md)

AI connected car: control GM vehicles, check diagnostics, and track location via agents.

## Description
### What you can do

Connect AI agents to the General Motors Connected Vehicle API for comprehensive car management:

- **List registered vehicles** to manage fleets or personal garages
- **Track GPS location** to find parked cars or monitor fleet movement
- **Monitor diagnostics** including oil life, battery voltage, and check engine status
- **Check EV charge levels** and estimated range for electric vehicles
- **Lock and unlock doors** remotely for security or guest access
- **Start and stop engines** remotely to pre-condition cabin temperature
- **Flash lights and sound horn** to locate vehicles in crowded areas
- **Send navigation destinations** directly to the infotainment system

### How it works

1. **Register at GM Developer Portal** and create an application
2. **Authenticate via OAuth** to obtain an access token for your vehicle
3. **Ask your AI agent** to check status, run diagnostics, or send commands
4. **Natural language commands** replace the myChevrolet/OnStar app navigation

### Who is this for?

Perfect for **GM vehicle owners**, **fleet managers**, **service advisors**, and **roadside assistance teams**. Let AI agents automate morning warm-ups, monitor tire pressure for safety, track mileage for maintenance schedules, and locate vehicles. Ideal for drivers who want to integrate their car into their smart home or AI assistant workflow for seamless mobility management.


## Available Tools (14)
- **flash_horn**: Requires VIN. Use this to locate a vehicle in a crowded parking lot or driveway.

Trigger the horn of a GM vehicle to locate it
- **flash_lights**: Requires VIN. Use this to locate a vehicle in the dark or signal ownership.

Flash the headlights and taillights of a GM vehicle
- **get_charge_status**: Requires VIN. Use this to manage EV range anxiety or schedule charging during off-peak hours.

Get the charging status and battery level of a GM EV (Bolt, Ultium, etc)
- **get_vehicle_diagnostics**: Requires VIN. Use this for maintenance scheduling, pre-trip inspections, or health monitoring.

Get comprehensive diagnostic data for a GM vehicle
- **get_fuel_level**: Requires VIN. Use this to plan refueling stops or monitor fuel economy.

Get the current fuel tank level of a GM vehicle
- **get_vehicle_location**: Requires VIN. Use this to find your parked car, track fleet assets, or verify vehicle movement.

Get the current GPS location of a specific GM vehicle
- **get_odometer**: Requires VIN. Use this to track service intervals, lease mileage limits, or fleet utilization.

Get the current mileage (odometer reading) of a GM vehicle
- **get_tire_pressure**: Requires VIN. Use this to identify leaks, ensure safety, or prepare for long trips.

Get the current tire pressure readings for all four tires
- **get_vehicles**: Use this as the first step to identify which VIN to use for commands or diagnostics.

List all GM vehicles associated with the account
- **lock_doors**: Requires VIN. Returns command status (success/failed/in-progress). Use this to secure the vehicle after parking or if you forgot to lock it.

Lock the doors of a specific GM vehicle remotely
- **send_turn_by_turn**: Requires VIN and a destination object with latitude, longitude, and address. Use this to plan a trip on your phone and have it ready in the car.

Send a destination to the vehicle's built-in navigation system
- **start_vehicle**: Requires VIN. Returns command status. Use this to warm up the car in winter or cool it down in summer before entering.

Remotely start the engine of a GM vehicle
- **stop_vehicle**: Requires VIN. Returns command status. Use this to cancel a remote start if the vehicle is now in use or if there is a safety concern.

Remotely stop the running engine of a GM vehicle
- **unlock_doors**: Requires VIN. Returns command status. Use this to let a passenger in or if keys are locked inside.

Unlock the doors of a specific GM vehicle remotely


## 💬 Prompt Examples

Here are some examples of how you can interact with the **General Motors** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Start the engine on my Bolt EV and tell me the current battery charge level and estimated driving range."

**🤖 AI Agent:**
> Engine started remotely on your 2024 Chevrolet Bolt EV (VIN: ...7X92). Battery charge: 78% (estimated range: 215 miles). Cabin pre-conditioning: active (72°F). Estimated ready time: 3 minutes.

---

**👤 You:**
> "Get the current GPS location of my GMC Sierra and flash the lights so I can spot it in the parking lot."

**🤖 AI Agent:**
> Your 2024 GMC Sierra is located at: 350 5th Avenue, New York, NY 10118 (parking level B2). Coordinates: 40.7484° N, 73.9857° W. Lights flashed successfully — look for the blinking hazards. Last parked: 2 hours ago.

---

**👤 You:**
> "Send the navigation destination 'Home' to my Cadillac's infotainment system so it's ready when I get in the car."

**🤖 AI Agent:**
> Navigation destination 'Home' sent to your 2024 Cadillac Escalade. The route will appear on the infotainment screen when you enter the vehicle. Estimated drive time: 25 minutes (14.2 miles via I-95 N). Current traffic: moderate.


## ❓ FAQ

**Q: Which vehicles are supported by this MCP server?**
This MCP server supports GM vehicles from model year 2015 and newer that are equipped with OnStar connectivity. This includes most Chevrolet, GMC, Buick, and Cadillac models. You can verify compatibility by checking if your vehicle has the OnStar button or the myChevrolet/myGMC/myBuick/myCadillac app support.

**Q: Do I need an active OnStar subscription to use this server?**
Yes, an active OnStar subscription is required to access the GM Connected Vehicle API. The specific features available depend on your OnStar plan. Remote commands like lock/unlock, remote start, and diagnostics require a plan that includes those capabilities. Check your OnStar plan details at my.chevrolet.com or contact OnStar support for more information.

**Q: How are vehicle commands secured?**
All vehicle commands are authenticated through the GM Developer Portal OAuth flow. Each command requires a valid access token tied to your GM account. The MCP server does not store credentials; it uses the token provided during setup. Only vehicles linked to your GM account can be controlled, and all commands are logged in the OnStar activity history for audit purposes.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/general-motors](https://vinkius.com/mcp/general-motors)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **General Motors** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `general-motors` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **General Motors** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "general-motors": {
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
