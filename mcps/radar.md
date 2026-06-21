# Radar MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/radar)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [cloud-infrastructure](../categories/cloud-infrastructure.md)

Equip your AI with geolocation tools — convert coordinates to addresses, map intellectual territories, calculate routes, and perform IP-based lookups.

## Description
Integrate **Radar** with an AI agent to bring enterprise-level location intelligence directly to your workflow. This server allows the AI to perform complex spatial lookups and geographical computations on your behalf.

### What you can do

- **Geocoding & Reverse Geocoding** — Convert readable addresses into exact coordinates (latitude/longitude), or vice versa.
- **Route Calculation** — Determine distance and driving times between multiple locations, predicting transit metrics efficiently.
- **Geofencing & Context** — Check whether specific coordinates fall within defined geographical boundaries (e.g., regions, stores, administrative borders).
- **IP Geolocation** — Locate a user or device strictly based on an IP address.

### How it works

1. Enable the server integration.
2. Add your Radar Publishable API Key.
3. Instruct your AI to plan coordinates, route distances, or geofence user locations on demand.

### Who is this for?

- **Software Engineers** — Resolve coordinate bugs, fetch boundary parameters, or quickly verify distance calculations in ongoing backend projects.
- **Logistics Planners** — Assess routing strategies and times without leaving the IDE workspace.
- **Data Analysts** — Quickly validate raw IP inputs into actionable regions or postal codes.


## Available Tools (10)
- **autocomplete**: Provides address or place suggestions as a user types
- **calculate_route_distance**: Calculates travel distance and duration between two points
- **calculate_routing_matrix**: Calculates travel times and distances between multiple origins and destinations
- **forward_geocode**: Converts a human-readable address into geographic coordinates (latitude and longitude)
- **get_location_context**: Retrieves contextual information for a location, such as geofences and weather
- **ip_geocode**: Retrieves geographic location information based on an IP address
- **reverse_geocode**: Converts geographic coordinates into a human-readable address
- **search_geofences**: Searches for active geofences near a specific location
- **search_places**: Searches for nearby places (POIs) based on coordinates
- **validate_address**: Validates and cleans up a structured address


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Radar** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Geocode '1600 Amphitheatre Parkway, Mountain View, CA'."

**🤖 AI Agent:**
> Calling Radar `geocode`, the coordinates are Latitude: 37.422, Longitude: -122.084.

---

**👤 You:**
> "Find the driving distance between my office in San Francisco (lat, lng) and the San Jose airport."

**🤖 AI Agent:**
> Using `get_routing`, the driving distance is approximately 45.2 miles, with an estimated travel time of 55 minutes, avoiding current traffic bottlenecks indicated by Radar.

---

**👤 You:**
> "Locate the country based on the IP address 8.8.8.8."

**🤖 AI Agent:**
> Using Radar's IP tool, `ip_geocode` resolves `8.8.8.8` to the United States.


## ❓ FAQ

**Q: Where do I find my Radar API key?**
Log into your Radar dashboard. Under 'Project Settings' or the dedicated API keys section, look for your 'Publishable Key'. This is the standard read-only key used for client integrations and MCP operations.

**Q: Should I use the Publishable Key or the Secret Key?**
Always use the **Publishable Key** for this MCP server instance if possible, as the operations (geocoding, routing, lookup) are typically safe read-only spatial actions.

**Q: Can it calculate multi-stop routes like a delivery app?**
Yes, but indirectly through distance comparisons. The basic routing API fetches times from Point A to Point B. The AI can chain these requests together to establish an estimated schedule contextually in your chat.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/radar](https://vinkius.com/mcp/radar)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Radar** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `radar` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Radar** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "radar": {
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
