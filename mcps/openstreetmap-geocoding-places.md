# OpenStreetMap (Geocoding & Places) MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/openstreetmap-geocoding-places)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [developer-tools](../categories/developer-tools.md)

Geocode any city or address to coordinates and back — forward/reverse geocoding, place search and location details via OpenStreetMap. No API key.

## Description
Give your AI agent a reliable sense of place. **Geocoding & Places** turns names and addresses into precise latitude/longitude, resolves coordinates back into cities and full addresses, searches for matching places, and returns complete location details — all through natural conversation.

### What you can do

- **Forward geocoding** — Convert a city name or street address into exact WGS84 latitude/longitude
- **Reverse geocoding** — Turn a latitude/longitude pair into a city, country and full formatted address
- **Place search** — Search free text and get a ranked list of matching places, each with its own id and coordinates
- **Location details** — Fetch the complete profile of a place (address components, bounding box, type) by id or coordinates

### How it works

1. Subscribe to this server
2. No credentials required — it uses the free OpenStreetMap **Nominatim** service, with automatic fallback to **Photon**
3. Every response comes back in one consistent shape, no matter which provider answered — the fallback is fully transparent

### Who is this for?

- **Developers** — add geocoding to apps and agents without signing up for a paid maps API
- **Data teams** — enrich records with coordinates or resolve coordinates to human-readable places
- **Logistics & travel** — look up addresses, validate locations and plan around real coordinates
- **Anyone** — ask "where is X?" or "what's at these coordinates?" and get a precise answer


## Available Tools (4)
- **get_latitude_longitude**: Use search_location to see multiple candidates, or get_location_details for the full record.

Convert a city name or street address into latitude/longitude coordinates. Use for "what are the coordinates of X?" or "geocode this address"
- **get_location**: Coordinates are WGS84 decimal degrees.

Convert latitude/longitude coordinates into a place: city, country and full address. Use for "what city is at these coordinates?" or "reverse geocode this point"
- **search_location**: Each item carries a place_id you can pass to get_location_details.

Search for places matching free text and return a ranked list of candidates. Use when a query is ambiguous or when you need several options to choose from
- **get_location_details**: place_id resolves via Nominatim. Coordinates ("lat,lon" in `place_id`, or the latitude/longitude params) resolve via reverse geocoding with automatic Photon fallback.

Fetch the complete details of a place, identified either by a place_id (from search_location / get_latitude_longitude) or by coordinates. Returns name, address components and bounding box


## 💬 Prompt Examples

Here are some examples of how you can interact with the **OpenStreetMap (Geocoding & Places)** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What are the coordinates of the Eiffel Tower?"

**🤖 AI Agent:**
> The Eiffel Tower is located at latitude 48.858370, longitude 2.294481 (Paris, France).

---

**👤 You:**
> "What city is at 40.7128, -74.0060?"

**🤖 AI Agent:**
> Those coordinates are in New York City, United States — the full address resolves to the Manhattan area of New York, NY.

---

**👤 You:**
> "Search for places called Springfield"

**🤖 AI Agent:**
> I found several matches for "Springfield": Springfield, Illinois; Springfield, Missouri; and Springfield, Massachusetts — each with its own coordinates and place_id you can inspect further.


## ❓ FAQ

**Q: Does this server require an API key or account?**
No. It uses the free OpenStreetMap Nominatim service and falls back to Photon automatically. Neither requires an API key, so you can start geocoding immediately.

**Q: What happens if one provider is down?**
The server queries Nominatim first and automatically falls back to Photon on any failure or empty result. Both are normalized to the same response shape, so the fallback is completely transparent to you.

**Q: How do I get full details for a place I found in a search?**
Every search result includes a place_id. Pass that id to get_location_details to retrieve the full record, or pass coordinates directly if you already have them.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/openstreetmap-geocoding-places](https://vinkius.com/ai-agent-connect/openstreetmap-geocoding-places)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **OpenStreetMap (Geocoding & Places)** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `openstreetmap-geocoding-places` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **OpenStreetMap (Geocoding & Places)** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "openstreetmap-geocoding-places": {
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
