# Google Maps Platform MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/google-maps-platform)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [industry-titans](../categories/industry-titans.md)

Get directions, place details, geocoding, and timezone data via official Google Maps APIs.

## Description
Connect **Google Maps Platform** to any AI agent and access the world's most accurate location intelligence — from turn-by-turn directions and distance matrices to rich place details and timezone data.

### What you can do
- **Geocoding** — Convert any address into precise latitude/longitude coordinates
- **Place Details** — Get comprehensive info for any business (hours, phone, ratings, reviews)
- **Directions & Routing** — Calculate routes for driving, walking, cycling, or public transit
- **Distance Matrix** — Compare travel times and distances between multiple locations
- **Nearby Search** — Find businesses or points of interest around a specific location
- **Elevation & Timezone** — Get altitude data and timezone info for any coordinate

### How it works
1. Subscribe to this server
2. Enter your Google Maps API Key
3. Start navigating and discovering locations from Claude, Cursor, or any MCP-compatible client

Google Maps provides the gold standard in global mapping data, used by millions of developers.

### Who is this for?
- **Travelers** — Get precise directions, travel times, and find nearby amenities like restaurants or gas stations
- **Logistics Coordinators** — Calculate efficient routes and compare travel times for multiple stops
- **Developers** — Integrate accurate geocoding and rich place data into their applications


## Available Tools
- **get_directions**: Supports modes: "driving" (default), "walking", "bicycling", "transit".

Get travel directions between two points
- **get_distance_matrix**: Origins and destinations can be single or multiple addresses/coordinates separated by pipe (|).

Calculate travel distance and time for multiple origins and destinations
- **get_elevation**: Input can be single "lat,lng" or multiple locations.

Get elevation data for locations on the earth
- **find_place_from_text**: Useful to get the Place ID or location before getting details.

Find a place based on a text query
- **geocode_address**: g., "1600 Amphitheatre Parkway, Mountain View, CA") and need the exact GPS coordinates. Returns the formatted address and the place_id.

Convert a physical address into geographic coordinates (latitude/longitude)
- **search_nearby_places**: You can filter by "type" (e.g., "restaurant", "gas_station") or "keyword". Radius is in meters.

Search for places of interest near a specific coordinate
- **get_place_details**: Requires a valid Place ID obtained from other search tools.

Get detailed information about a specific place using its Place ID
- **reverse_geocode**: Useful for identifying locations from GPS data.

Convert GPS coordinates back into a physical address
- **get_timezone**: Essential for scheduling across time zones.

Get timezone information for a specific location


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Google Maps Platform** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Find the address for 'Statue of Liberty'."

**🤖 AI Agent:**
> Statue of Liberty is located at Liberty Island, New York, NY 10004. Coordinates: 40.6892° N, 74.0445° W.

---

**👤 You:**
> "Get directions from Times Square to Central Park."

**🤖 AI Agent:**
> Driving route: Distance: 2.5 miles, Duration: 12 mins. Walk route: Distance: 2.1 miles, Duration: 40 mins.

---

**👤 You:**
> "Find coffee shops near 'Pike Place Market'."

**🤖 AI Agent:**
> Found 5 nearby: 1. Starbucks Reserve Roastery (4.8⭐). 2. Storyville Coffee (4.7⭐). 3. Cafe Campagne (4.5⭐).


## ❓ FAQ

**Q: How do I get a Google Maps API Key?**
Go to the Google Cloud Console, create a project, enable the Maps APIs (Geocoding, Places, Directions, etc.), and generate an API Key in the Credentials section.

**Q: What is a Place ID?**
A Place ID is a unique text identifier for a place (e.g., 'ChIJN1t_tDeuEmsRUsoyG83frY4'). You can get it using the 'search_nearby_places' or 'find_place_from_text' tools, and use it to get detailed info via 'get_place_details'.

**Q: Can I get travel times for public transit?**
Yes! Use 'get_directions' or 'get_distance_matrix' with mode set to 'transit'. Note that transit data availability depends on the city and Google's coverage.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/google-maps-platform](https://vinkius.com/mcp/google-maps-platform)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Google Maps Platform** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `google-maps-platform` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Google Maps Platform** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "google-maps-platform": {
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
