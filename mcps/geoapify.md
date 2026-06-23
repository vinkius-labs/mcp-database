# Geoapify MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/geoapify)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [data-analytics](../categories/data-analytics.md)

Access powerful location intelligence — geocoding, routing, place search, and IP tracking directly from your AI agent.

## Description
Integrate **Geoapify** into your AI workflows to provide your agent with advanced geospatial capabilities. From simple address lookups to complex route matrix calculations, this server enables precise location-based decision making.

### What you can do

- **Geocoding & Search** — Convert addresses to coordinates with `geocode_search` or get real-time suggestions using `geocode_autocomplete`.
- **Reverse Geocoding** — Identify human-readable addresses from GPS coordinates using `geocode_reverse`.
- **Routing & Logistics** — Calculate optimal paths with `calculate_route` or generate distance matrices for multiple origins and destinations via `calculate_route_matrix`.
- **Location Intelligence** — Detect user regions via `get_ip_info` or find specific points of interest with `search_places`.
- **Map Matching** — Snap messy GPS tracks to the actual road network using `map_matching` for precise fleet tracking.

### How it works

1. Subscribe to this server
2. Enter your Geoapify API Key
3. Start querying location data from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Logistics Managers** — automate route planning and distance calculations for delivery fleets.
- **Developers** — implement address validation and autocomplete features without leaving the IDE.
- **Data Analysts** — enrich datasets with precise coordinates, elevation data, and administrative boundaries.


## Available Tools (17)
- **calculate_isoline**: Calculate areas reachable within a certain time (isochrones) or distance (isodistances)
- **calculate_route_matrix**: Calculate travel times and distances between multiple sources and targets
- **calculate_route**: Calculate routes for various modes (drive, truck, bicycle, walk, transit)
- **create_batch_job**: Process up to 1000 requests in a single asynchronous job
- **geocode_autocomplete**: Get real-time suggestions for address input fields
- **geocode_reverse**: Find the address for a specific GPS coordinate
- **geocode_search**: Convert free-form or structured addresses into coordinates
- **geometry_operation**: Perform spatial operations on GeoJSON data (union, intersection, buffer, etc.)
- **get_batch_job**: Get results for an asynchronous batch job
- **get_boundaries_consists_of**: Retrieve sub-boundaries within an area
- **get_boundaries_part_of**: Retrieve administrative, postal, or political boundaries containing a point
- **get_elevation**: Get elevation data for specific coordinates
- **get_place_details**: Get detailed info (contact, opening hours, building geometry) for a place
- **get_ip_info**: Detect user location based on IP address
- **map_matching**: Snap GPS tracks to the road network
- **route_planner**: Solve Vehicle Routing Problems (VRP), including TSP and delivery optimization
- **search_places**: Find points of interest (POIs) by category


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Geoapify** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Find the latitude and longitude for '1600 Amphitheatre Parkway, Mountain View, CA'."

**🤖 AI Agent:**
> I've located the coordinates for that address using `geocode_search`. The location is Latitude: 37.4224857, Longitude: -122.0855845.

---

**👤 You:**
> "Calculate a driving route from Paris to Lyon."

**🤖 AI Agent:**
> Using `calculate_route`, I've found the optimal driving path. The trip is approximately 465km and will take about 4 hours and 20 minutes under normal traffic conditions.

---

**👤 You:**
> "What city is associated with the IP address 8.8.8.8?"

**🤖 AI Agent:**
> I've checked the IP info for 8.8.8.8. It is located in Mountain View, California, United States.


## ❓ FAQ

**Q: How can I find the coordinates of a specific street address?**
Use the `geocode_search` tool. You can provide a free-form text string or structured data like city and street to get precise latitude and longitude coordinates.

**Q: Can the AI calculate travel times for multiple delivery destinations at once?**
Yes! The `calculate_route_matrix` tool allows you to submit multiple source and target locations to receive a comprehensive matrix of travel times and distances.

**Q: Is it possible to identify where a user is located based on their IP address?**
Absolutely. Use the `get_ip_info` tool to retrieve location metadata, including country, city, and timezone, associated with a specific IP address.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/geoapify](https://vinkius.com/mcp/geoapify)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Geoapify** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `geoapify` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Geoapify** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "geoapify": {
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
