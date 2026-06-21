# Trimble MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/trimble)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [industry-titans](../categories/industry-titans.md)

Equip your AI agent with enterprise-grade truck routing, commercial geocoding, and advanced toll cost logistics algorithms.

## Description
Connect your AI agent exclusively to your **Trimble PC*MILER** logistics infrastructure. Elevate your transportation operations replacing disjointed navigation screens. Communicate organically to your agent to dictate exact vehicle dimensions to avoid tight bridges, compile meticulous state-by-state fuel mileage reports, or estimate holistic transit budgets using precise industrial coordinates.

### What you can do

- **Heavy Routing Limits** — Command a route trace bypassing commercial hazard zones using variables like actual truck dimensions (height, weight) directly in conversation
- **Toll Estimation** — Ping exactly how much a full route will impact your budget by breaking down both cash and electronic toll values mathematically
- **State Mileage Reporting** — Generate automatic fuel-tax (IFTA) summaries calculating exact penetration mileage crossed inside individual states
- **Logistics Forensics** — Interrogate geographical locations using structured isochrone grids (predicting max travel based on an hour limit) or matrix origins
- **Spatial Exclusions** — Trace itineraries avoiding strictly designated public roads and restricting expressways in the blink of an eye

### How it works

1. Provision this connector inside your central Vinkius matrix
2. Inject your certified Trimble Developer API Key
3. Start addressing fleet transit instructions directly mapping routes over any environment

### Who is this for?

- **Fleet Operations Managers** — Oversee large transport deployments bypassing hazards evaluating toll expenditures across specific trips in milliseconds
- **Logistical Data Scientists** — Plot broad origins-destinations distance matrices interacting solely through terminal queries over heavy machinery requirements
- **Dispatch Analysts** — Investigate delivery reach by requesting an active 'time shed' (isochrone) boundary estimating limits for rush transit manually


## Available Tools
- **calculate_driving_isochrone**: Provide center coordinates and time in minutes.

Calculates the reachable area within a specific time limit from a center point
- **calculate_matrix_routing**: Provide arrays of lon,lat points.

Calculates distances and travel times between multiple origins and destinations
- **calculate_state_mileage**: Calculates mileage broken down by US state or province for a given route
- **calculate_trip_tolls**: Returns cash and electronic toll fees in USD.

Estimates the total toll costs for a specific truck route
- **calculate_truck_route**: Returns distance, time, and routing polyline.

Calculates a truck-compliant route between multiple stops using Trimble PC*MILER
- **get_truck_directions**: Considers bridge heights, HazMat restrictions, and weight limits.

Retrieves turn-by-turn driving directions for a truck route
- **route_avoiding_roads**: Calculates a route that explicitly avoids certain roads or expressways
- **route_by_vehicle_size**: Provide vehicle height in inches and weight in lbs.

Calculates a truck route using specific vehicle dimensions
- **search_trimble_address**: Searches for locations and commercial addresses in the Trimble database
- **reverse_geocode**: Converts geographic coordinates into the nearest commercial address


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Trimble** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Calculate a truck route starting from -74.0,40.7 to -75.0,41.0."

**🤖 AI Agent:**
> Route computed successfully. The total truck-safe distance spans 85.3 miles. Expected travel time is approximately 1 hour and 32 minutes along main highways based on these parameters.

---

**👤 You:**
> "What are the estimated toll costs passing that exact same route?"

**🤖 AI Agent:**
> Checking toll estimators. The total calculated fees are 12.50 USD utilizing verified electronic transponders, scaling higher unpredicted if operating on cash lanes continuously.


## ❓ FAQ

**Q: Where do I recover the operational Trimble API Key?**
Navigate smoothly into your authorized corporate sphere residing on the `developer.trimble.com` suite. Look closely at the primary headers locating your Applications or API Access portal hub. Designate a new instance or inspect an existing module tied to Mapping/PC*MILER bounds, copy the immutable token securely generated, and inject it flawlessly right below.

**Q: Will `route_avoiding_roads` block major US interstates dynamically?**
Yes. This precise endpoint takes an array/string argument of roads to systematically avoid. Instruct the agent to evade specific highways, and Trimble's underlying algorithm recalculates the mathematical vectors completely rendering a path rejecting that specific asphalt footprint unconditionally.

**Q: What is the lifespan of my Trimble API access token?**
Trimble access tokens obtained via OAuth generally have a short lifespan, typically expiring after 60 minutes. Your MCP integration handles this internally by automatically renewing it using refresh processes when necessary, so no manual intervention is required.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/trimble](https://vinkius.com/mcp/trimble)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Trimble** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `trimble` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Trimble** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "trimble": {
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
