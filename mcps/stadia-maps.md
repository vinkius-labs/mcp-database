# Stadia Maps MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/stadia-maps)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [data-analytics](../categories/data-analytics.md)

Equip your AI with advanced geospatial routing and mapping logic. Calculate distances, geocode coordinates, and plot optimized trips securely.

## Description
Imbue your artificial intelligence environment with the geospatial and routing capabilities of **Stadia Maps**. Seamlessly audit logistical questions and compute optimal transit routes across numerous delivery points without leaving your conversational interface. Empower your assistant to translate standard addresses into precise geographic coordinates, calculate time-and-distance matrices objectively, or parse topographical elevation data efficiently, connecting global mapping infrastructure directly to your local workflows.

### What you can do

- **Geospatial Coordination** — Convert physical addresses into exact coordinates using `forward_geocode`, or deduce properties from latitude and longitude via `reverse_geocode`.
- **Route Computation** — Instruct your AI to generate accurate driving vectors between locations via `calculate_route`, and establish extensive routing cost-matrices utilizing `calculate_distance_matrix`.
- **Logistical Optimization** — Resolve complex routing problems automatically with `optimized_trip_route`, and map exact reachable perimeters utilizing `calculate_isochrone`.
- **Topography & Precision** — Align raw GPS tracks to official street networks accurately with `execute_map_matching`, and retrieve detailed elevation metrics applying `get_path_elevation`.

### How it works

1. Connect the Stadia Maps MCP module natively to your active AI environment.
2. Securely provide your Developer API Key within the MCP configuration.
3. Engage your coding assistant: "Plot the most efficient vehicle route intersecting these specific delivery coordinates."

### Who is this for?

- **Logistics Engineers** — Construct and test delivery scheduling models natively, instructing the AI to solve complex routing problems.
- **GIS Data Analysts** — Accurately refine and correct noisy fleet GPS tracker data points entirely through the integration.
- **Fleet Dispatchers** — Audit and establish local timezone contexts for globally distributed assets effectively.


## Available Tools (10)
- **autocomplete_location**: Provides predictive address suggestions based on partial input
- **calculate_isochrone**: Calculates an area reachable within a specific time or distance
- **calculate_distance_matrix**: Calculates distances and travel times between multiple points
- **calculate_route**: Locations should be a JSON array of {lat, lon}. Costing can be "auto", "bicycle", or "pedestrian".

Calculates a route between multiple geographic points
- **forward_geocode**: Converts a physical address string into geographic coordinates
- **get_path_elevation**: Retrieves elevation/height data for a specific geographic path
- **get_timezone**: Retrieves the local timezone for specific geographic coordinates
- **execute_map_matching**: Snaps raw GPS points to the road network
- **optimized_trip_route**: Returns the optimized path.

Calculates the most efficient route between multiple stops
- **reverse_geocode**: Converts geographic coordinates into a physical address


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Stadia Maps** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Locate and securely return the comprehensive latitude and longitude values associated with this address: '1600 Amphitheatre Parkway, Mountain View, CA'."

**🤖 AI Agent:**
> Initiating query analysis to index string formats effectively via `forward_geocode` targeting official datasets...

**Coordinates Resolved** 📍
- **Latitude:** `37.4225`
- **Longitude:** `-122.084`

The targeted input accurately evaluates to corresponding geographical metrics.

---

**👤 You:**
> "Analyze these targeted locations formatting parameters into a complete trip route simulation enforcing an algorithmic analysis assuming optimal routing for automobiles."

**🤖 AI Agent:**
> Evaluating parameters defined specifically for operation execution utilizing mode "auto" via `optimized_trip_route`.

**System Routing Computed and Sequenced**:
1. 🏁 Node Departure A (Lat: 40.71, Lon: -74.00)
2. 🚙 Logistical Intermediate Segment Node B (Lat: 40.75, Lon: -73.98)
3. 🏁 Objective Target Completion Target C (Lat: 40.78, Lon: -73.96)


## ❓ FAQ

**Q: Does it return visual maps or raw data?**
Raw structured JSON only — coordinates, distances, durations, and elevation values. No interactive map tiles are rendered. You can use the data to plot maps in your own application.

**Q: Does `optimized_trip_route` solve the Traveling Salesman Problem?**
Yes. Pass an unordered set of coordinates and it returns the optimal visit sequence minimizing total travel time or distance.

**Q: Is there a free tier?**
Yes. Stadia Maps offers a free tier with generous limits for geocoding, routing, and elevation queries. Sign up at stadiamaps.com and generate an API key from the dashboard.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/stadia-maps](https://vinkius.com/mcp/stadia-maps)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Stadia Maps** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `stadia-maps` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Stadia Maps** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "stadia-maps": {
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
