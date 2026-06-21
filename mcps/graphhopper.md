# GraphHopper MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/graphhopper)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [developer-tools](../categories/developer-tools.md)

Empower routing and geocoding via GraphHopper — calculate optimal routes, perform reverse geocoding, solve vehicle routing problems, and analyze reachability directly from any AI agent.

## Description
Connect your **GraphHopper** account to any AI agent and take full control of your geospatial routing, geocoding, and fleet optimization through natural conversation.

### What you can do

- **Route Orchestration** — Calculate optimal routes between multiple GPS stops, identifying precise asynchronous directions and time calculations bypassing URL length limits natively
- **Geocoding discovery** — Extract explicitly attached REST arrays targeting `/geocode` to translate human-readable addresses into precise LatLon coordinates for spatial analysis
- **Reverse Geocoding** — Perform structural extraction of properties matching GPS pins exactly against named physical streets to verify localized entity bounds flawlessly
- **Routing Matrix Calculation** — Generate N x M arrays of travel times and distances to analyze complex grid logistics and distance tables between multiple points synchronously
- **Isochrone Reachability** — Identify precisely the boundary reachable in a specific time limit from a starting point, defining reachability polygons for site selection or delivery zones
- **VRP Optimization** — Command explicit JSON targets firing Traveling Salesman configs for multiple vehicles, checking time windows and capacity constraints to solve complex logistics synchronously
- **Map Matching Auditing** — Validate API logic correcting imprecise GPS jumps by snapping raw GPX tracks perfectly onto street vectors limitlessly

### How it works

1. Subscribe to this server
2. Enter your GraphHopper API Key (found in your GraphHopper Dashboard under API Keys)
3. Start optimizing your logistics and routing from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Logistics & Delivery Managers** — optimize multi-stop routes and solve vehicle routing problems without manual spreadsheet calculations
- **GIS & Data Analysts** — perform geocoding and analyze isochrone reachability for site selection using natural language
- **Developers** — test and debug routing parameters and verify map matching logic directly from the chat interface
- **Supply Chain Planners** — calculate routing matrices and verify distance tables across entire distribution networks in real-time


## Available Tools (10)
- **search_geocode**: Identify bounded routing spaces inside the Headless GraphHopper Engine
- **calculate_distance_isochrone**: Provision a highly-available JSON Payload generating physical borders
- **calculate_reachability_polygon**: Enumerate explicitly attached structured rules exporting active Reachability
- **snap_gpx_to_road**: Irreversibly vaporize explicit validations extracting GPX logic natively
- **calculate_routing_matrix**: Inspect deep internal arrays mitigating specific Math tables
- **reverse_geocode**: Perform structural extraction of properties driving active OSM bindings
- **calculate_url_route**: Retrieve explicit Cloud logging tracing explicit lightweight Directions
- **calculate_heavy_route**: Identify precise active arrays spanning native multi-stop geometries
- **submit_vrp_optimizer**: Dispatch an automated validation check routing explicit jsprit solves
- **poll_vrp_solution**: Retrieve the exact structural matching verifying Delivery alternatives


## 💬 Prompt Examples

Here are some examples of how you can interact with the **GraphHopper** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Calculate a car route between '40.71, -74.00' and '40.75, -73.98'"

**🤖 AI Agent:**
> Route calculated! I've found the optimal driving path. Total distance: 3.5 miles. Estimated time: 12 minutes. I can provide the step-by-step turn directions for you now.

---

**👤 You:**
> "Show me the 10-minute reachability zone from central Berlin"

**🤖 AI Agent:**
> Isochrone generated! I've mapped the area reachable within 10 minutes from your location in Berlin. I can provide the polygon coordinates or verify if specific addresses fall within this boundary.

---

**👤 You:**
> "Reverse geocode these coordinates: '48.85, 2.35'"

**🤖 AI Agent:**
> Coordinates matched! The location for 48.85, 2.35 corresponds to 'Rue de Rivoli, Paris, France'. It is located in the 4th arrondissement. Would you like more venue details for this spot?


## ❓ FAQ

**Q: Can my agent calculate reachability zones using time limits?**
Yes. Use the 'calculate_reachability_polygon' tool. Provide a starting point and a time limit in seconds. The agent will retrieve the isochrone polygon defining exactly what area is reachable within that duration natively.

**Q: How do I optimize a multi-stop delivery route via chat?**
Use the 'submit_vrp_optimizer' tool. Provide a JSON payload defining your vehicles and service stops. The agent will trigger the VRP solver to calculate the most efficient sequence, accounting for time windows and capacities synchronously.

**Q: Can I perform reverse geocoding to find a street name through the agent?**
Absolutely. Use the 'reverse_geocode' tool. Provide the latitude and longitude. Your agent will analyze the global OSM bounds to match the coordinates exactly against the nearest physical street address flawlessy.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/graphhopper](https://vinkius.com/mcp/graphhopper)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **GraphHopper** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `graphhopper` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **GraphHopper** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "graphhopper": {
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
