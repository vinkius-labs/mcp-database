# TomTom MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/tomtom-alternative)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [geocoding-maps](../categories/geocoding-maps.md)

Access global mapping, geocoding, and routing services. Search for addresses, calculate optimal routes, and retrieve map tiles directly through AI.

## Description
Connect **TomTom**'s industry-leading location technology to your AI agent to unlock powerful spatial intelligence and navigation capabilities.

### What you can do

- **Fuzzy Search** — Find addresses, points of interest (POIs), and streets using flexible, free-text queries.
- **Geocoding** — Convert structured addresses into precise geographic coordinates for mapping and analysis.
- **Smart Routing** — Calculate optimal paths between locations with support for real-time traffic, vehicle types (truck, car, bicycle), and travel modes.
- **Advanced Logistics** — Use advanced routing for route reconstruction with supporting points and avoid specific country vignettes.
- **Map Visualization** — Retrieve raster map tiles (basic, hybrid, or labels) to visualize locations in different styles like 'main' or 'night'.

### How it works

1. Subscribe to this server
2. Enter your TomTom API Key
3. Start querying locations and routes from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Logistics & Fleet Managers** — optimize delivery routes and calculate travel times based on vehicle profiles.
- **Travel & Hospitality** — help users find points of interest and navigate between destinations.
- **Developers** — integrate location-based context into applications without leaving the chat or IDE.


## Available Tools (6)
- **calculate_advanced_route**: Calculate an advanced route with supporting points or avoid vignettes
- **calculate_route**: Calculate a route between origin and destination
- **geocode**: Convert addresses into geographic coordinates
- **get_map_tile**: Returns the URL to the tile image.

Get a raster map tile URL
- **fuzzy_search**: Single-line fuzzy search for addresses and POIs
- **get_traffic_incidents**: Get real-time traffic incidents and flow information


## 💬 Prompt Examples

Here are some examples of how you can interact with the **TomTom** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Search for 'Eiffel Tower' in Paris using fuzzy search."

**🤖 AI Agent:**
> I found the Eiffel Tower at Champ de Mars, 5 Av. Anatole France, 75007 Paris, France. Coordinates: 48.8584, 2.2945.

---

**👤 You:**
> "Calculate a car route from 52.509,13.429 to 52.502,13.438."

**🤖 AI Agent:**
> The fastest route by car is approximately 1.2km and will take about 4 minutes with current traffic conditions.

---

**👤 You:**
> "Get a basic map tile URL for zoom level 15 at x=17600, y=10700."

**🤖 AI Agent:**
> Here is the URL for the requested map tile: https://api.tomtom.[REDACTED].png?key=YOUR_API_KEY


## ❓ FAQ

**Q: Can I search for a place using just a name like 'Coffee Shop'?**
Yes! Use the `fuzzy_search` tool. It allows you to search for points of interest, streets, and addresses using free-text queries.

**Q: Does the routing tool take real-time traffic into account?**
Yes, by default the `calculate_route` tool uses real-time traffic data to provide the most accurate travel times and paths.

**Q: How can I get the latitude and longitude for a specific address?**
You can use the `geocode` tool. Simply provide the address string, and it will return the geographic coordinates.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/tomtom-alternative](https://vinkius.com/mcp/tomtom-alternative)
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
3. Set Type to "SSE" (or "streamable HTTP"), enter `tomtom-alternative` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **TomTom** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "tomtom-alternative": {
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
