# Nominatim MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/nominatim)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [developer-tools](../categories/developer-tools.md)

Geocode addresses, reverse geocode coordinates and explore OpenStreetMap data — no API key required.

## Description
Connect to **Nominatim** and search the world's most comprehensive open-source geographic database through natural conversation — no API key needed.

### What you can do

- **Address Search** — Find any place by name, address or type of place (restaurants, schools, hospitals)
- **Reverse Geocoding** — Convert GPS coordinates to human-readable addresses
- **OSM Lookup** — Look up detailed info for any OpenStreetMap object by its ID
- **Structured Addresses** — Get detailed address components (street, city, state, postal code, country)
- **Multi-language Names** — Retrieve place names in different languages
- **Bounding Boxes** — Get geographic boundaries for cities, countries and regions

### How it works

1. Subscribe to this server
2. No API key needed — start searching immediately
3. Explore geographic data from Claude, Cursor, or any MCP-compatible client

No API key required — completely free, powered by OpenStreetMap community data.

### Who is this for?

- **Developers** — geocode addresses and convert coordinates without paid geocoding services
- **Travelers** — find addresses and discover what's at any GPS coordinate
- **Researchers** — explore OpenStreetMap object details, administrative boundaries and place hierarchies
- **Data Analysts** — batch geocode addresses and extract structured location data


## Available Tools
- **get_details**: Returns the object's full name, display name, place rank, importance score, bounding box, parent place hierarchy, linked Wikipedia/Wikidata articles and optional extratags. OSM type: N (node), W (way), R (relation).

Get detailed info for an OSM object
- **lookup_osm**: IDs are formatted as "type{id}" where type is N (node), W (way) or R (relation). Multiple IDs are comma-separated. Returns the object's display name, coordinates, bounding box and properties.

Look up OSM objects by ID
- **reverse_geocode**: Returns the nearest address, city, state, country and other location details. Supports different zoom levels for varying detail granularity.

Convert coordinates to an address
- **search**: Returns results with coordinates, bounding box, display name, address components and OSM type/id. Supports structured searches with country codes and viewbox for region prioritization. Rate limited to 1 request/second.

Search for places by name or address
- **get_status**: Returns status message and response latency. Useful for verifying the service is operational before making other requests.

Get Nominatim server status


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Nominatim** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Find the coordinates for the Eiffel Tower."

**🤖 AI Agent:**
> Found: Eiffel Tower at coordinates 48.8584, 2.2945. Address: Champ de Mars, 5 Avenue Anatole France, 75007 Paris, France. Bounding box: 48.8574-48.8594, 2.2935-2.2955. OSM ID: W5013364 (way).

---

**👤 You:**
> "What address is at coordinates 40.7128, -74.0060?"

**🤖 AI Agent:**
> Coordinates 40.7128, -74.0060 correspond to: City Hall Park, New York, NY 10007, United States. Borough: Manhattan. County: New York County. State: New York. Country: United States. Place type: park.

---

**👤 You:**
> "Search for 'Central Park' and show me its bounding box."

**🤖 AI Agent:**
> Central Park, New York: Bounding box 40.7644 to 40.8006 (lat), -73.9818 to -73.9491 (lon). OSM ID: W326168186 (way). Place type: park. Address: Manhattan, New York County, New York, 10024, United States.


## ❓ FAQ

**Q: Do I need an API key?**
No! Nominatim is completely free and requires no authentication. It's powered by the OpenStreetMap community. Just subscribe and start searching. Rate limit is 1 request per second.

**Q: How accurate is the geocoding?**
Nominatim uses OpenStreetMap data, which is crowd-sourced and varies by region. Urban areas typically have very accurate results. Use addressdetails=1 to get structured address components and namedetails=1 for multi-language names.

**Q: Can I convert coordinates to an address?**
Yes! Use reverse_geocode with latitude and longitude. Returns the nearest address with street name, house number, city, state, postal code and country. Supports different zoom levels for varying detail granularity.

**Q: What is an OSM ID and how do I use it?**
OSM IDs are unique identifiers for OpenStreetMap objects: N for nodes (points), W for ways (lines/areas), R for relations (groups). Use lookup_osm with IDs like 'W123456' or 'N987654'. Use get_details for comprehensive info on a single object.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/nominatim](https://vinkius.com/mcp/nominatim)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Nominatim** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `nominatim` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Nominatim** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "nominatim": {
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
