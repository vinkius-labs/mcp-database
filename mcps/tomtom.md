# TomTom MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/tomtom)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [industry-titans](../categories/industry-titans.md)

Equip your AI agent with global mapping, routing, and real-time traffic capabilities powered by TomTom.

## Description
Connect your **TomTom** API account directly to any AI agent to unlock enterprise-grade geospatial and logistical capabilities native to your platform. Convert complex addresses instantly, evaluate driving routes based on exact origin and destination coordinates, and visualize live traffic blocks directly through chat queries.

### What you can do

- **Precision Geocoding** — Process any physical address string into absolute geographic latitude/longitude coordinates using fuzzy logic or structured fields, as well as reversing coordinates back to plain street names
- **Route Computation** — Calculate the exact travel time, polyline geometry, and distance for a trip between two precise coordinates
- **Real-Time Traffic** — Map traffic incidents (accidents, constructions, jams) constrained within a bounding box, or survey the traffic flow speed of a particular avenue segment
- **Poi Discovery** — Find global Points of Interest based on categories (e.g., hospitals, fuel) and retrieve rich contact metadata or opening hours for specific locations
- **Travel Boundaries** — Calculate reachable ranges (polygonal limits) to understand exactly how far your fleet or agents can travel within a set time budget

### How it works

1. Add this marketplace component to your workflow
2. Open the TomTom Developer Portal and produce a secure API token
3. Plug the key above, and start interrogating global geography immediately

### Who is this for?

- **Fleet Managers** — Ensure continuous auditing of road incidents and calculate travel time differences organically
- **Logistics Engineers** — Implement and test route shedding, time boundaries, and flow calculations locally
- **App Developers** — Programmatically pull local Points of Interest strings and contact numbers directly into their coding setup


## Available Tools (10)
- **calculate_reachable_range**: Provide center coordinates and a time budget in seconds.

Calculates an area reachable within a specific time or distance budget
- **calculate_route**: Returns the route polyline and a summary.

Calculates a route and travel time between two points
- **search_poi_by_category**: Provide a category name and a center coordinate.

Searches for points of interest (POIs) near a location by category (e.g., gas stations, hospitals)
- **fuzzy_geocoding**: Converts a physical address string into geographic coordinates using fuzzy matching
- **get_poi_details**: Retrieves rich metadata for a specific point of interest ID
- **get_traffic_incidents**: Provide min/max lat/lon coordinates.

Retrieves real-time traffic incident details within a bounding box
- **get_traffic_flow_segment**: Provide center coordinates.

Retrieves the traffic flow speed and quality for a specific road segment
- **reverse_geocoding**: Converts geographic coordinates into a physical address
- **autocomplete_place_search**: Provide a partial string and optional bias coordinates.

Provides predictive location suggestions based on partial input
- **structured_geocoding**: Provide parameters like countryCode and postalCode.

Performs geocoding using explicit address components (e.g., street, city, zip)


## 💬 Prompt Examples

Here are some examples of how you can interact with the **TomTom** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Convert these coordinates into an address: Lat 40.7128, Lon -74.0060."

**🤖 AI Agent:**
> The coordinates return an address explicitly linked to the parameter grid:
- Broad St, New York, NY 10004, United States

---

**👤 You:**
> "Check for any traffic incidents on the 101 freeway bounded roughly by these dimensions."

**🤖 AI Agent:**
> A real-time scan revealed 1 active traffic incident in that bounding box:
- Type: Accident/Lane blocked
- Severity: Major delay expected
- Center: Lat 34.05, Lon -118.25


## ❓ FAQ

**Q: Where and how do I extract my TomTom API Key?**
Log into your account at the `developer.tomtom.com` portal. Go to the dashboard console and select **Keys** (or My Dashboard). Either use your default developer API Key or click **Add new Key** for this specific agent usage. Copy the entire cryptographic string and insert it below securely.

**Q: Can the agent interact with or update the maps itself?**
No. The integration exclusively lists and pulls read-only endpoints (timelines, distances, addresses). The AI agent leverages TomTom merely to process geographic conversions securely; it lacks parameters capable of feeding corruptions or modifying raw data maps.

**Q: Should I secure my TomTom API Key?**
Yes. It is highly recommended to set a Domain Whitelist in your key management settings on the TomTom developer portal. This restricts the use of your key to specific domains, preventing unauthorized use or rate limit exhaustion.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/tomtom](https://vinkius.com/mcp/tomtom)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **TomTom** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `tomtom` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **TomTom** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "tomtom": {
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
