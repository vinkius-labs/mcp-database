# HERE (Location & Maps) MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/here-location-maps)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [industry-titans](../categories/industry-titans.md)

Build with location data via HERE — geocode addresses, calculate routes, track traffic, and get weather.

## Description
Connect your **HERE Technologies** account to any AI agent and take full control of cloud-native spatial analytics and location services through natural conversation.

### What you can do

- **Geocoding & Search** — Convert addresses to precise coordinates (and vice versa) and discover points of interest (POI) with advanced autosuggest directly from your agent
- **Routing & Logistics** — Calculate optimal routes for cars, trucks, or pedestrians, and generate complex distance matrices for efficient fleet management
- **Isolines & Reachability** — Visualize reachability polygons to see how far you can travel within a set time or distance limit from any origin point
- **Traffic & Flow** — Monitor real-time traffic speeds and congestion patterns using precise bounding box queries to optimize delivery times
- **Weather & Environment** — Fetch live weather observations and forecasts for any location on the globe to prepare for environmental impacts
- **Place Details** — Lookup rich metadata and schema for specific places using unique HERE Place IDs for deep point-of-interest analysis

### How it works

1. Subscribe to this server
2. Enter your HERE API Key
3. Start building location-aware applications from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **GIS Analysts** — perform complex geocoding and reachability analysis through natural conversation without GIS software
- **Logistics Managers** — calculate optimal routes and travel-time matrices for delivery fleets and supply chain optimization
- **Developers** — integrate real-time traffic, routing, and weather data into AI agents for context-aware automation
- **Urban Planners** — analyze city accessibility, traffic flow patterns, and environmental conditions at scale


## Available Tools
- **autosuggest_query**: Identify precise active arrays spanning native Location suggestions
- **calculate_v8_isoline**: router` optimizing where a user can travel within a set `time` or `distance` limit.

Dispatch an automated validation check routing explicit Reachability Polygons
- **calculate_routing_matrix**: Provision a highly-available JSON Payload generating multi-node Maps
- **calculate_v8_route**: Inspect deep internal arrays mitigating specific Traffic pathways
- **discover_places**: Retrieve explicit Cloud logging tracing explicit POI categories
- **forward_geocode**: Identify bounded routing spaces inside the Headless HERE Search limit
- **get_traffic_flow**: json` detecting current congestion patterns via a Bounding Box limit.

Retrieve the exact structural matching verifying Delivery Flow speeds
- **get_weather_observation**: Enumerate explicitly attached structured rules exporting active Meteorology
- **lookup_place_id**: Irreversibly vaporize explicit App nodes dropping live Place contexts
- **reverse_geocode**: Perform structural extraction of properties driving active Pin boundaries


## 💬 Prompt Examples

Here are some examples of how you can interact with the **HERE (Location & Maps)** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What's the best route from San Francisco to San Jose by car?"

**🤖 AI Agent:**
> Calculating route… The optimal path via US-101 S is approximately 48 miles and will take about 55 minutes with current traffic. Would you like to see the turn-by-turn summary?

---

**👤 You:**
> "How far can I drive in 15 minutes from Times Square, NY?"

**🤖 AI Agent:**
> Generating isoline… Based on current road conditions, you can reach most of Midtown Manhattan, parts of Hell's Kitchen, and cross into Weehawken via the Lincoln Tunnel within 15 minutes. Would you like the coordinate boundaries?

---

**👤 You:**
> "What is the current weather observation for Tokyo?"

**🤖 AI Agent:**
> Current weather in Tokyo: 18°C, Partly Cloudy, Humidity 62%, Wind 12km/h from the SE. The forecast for the next 6 hours shows a slight chance of rain. Would you like a detailed 24-hour forecast?


## ❓ FAQ

**Q: Can I geocode a list of addresses through my agent?**
Yes. Use the `forward_geocode` tool to convert any text-based address into precise coordinates. Your agent can process multiple addresses in a single conversation, making it ideal for cleaning up location datasets.

**Q: How do I calculate travel time between multiple points?**
The `calculate_routing_matrix` tool allows you to generate distance and duration spans between arrays of origins and destinations, perfect for fleet optimization and logistics planning.

**Q: Can I get real-time traffic updates for a specific area?**
Absolutely. Use the `get_traffic_flow` tool with a bounding box (bbox) query to detect current congestion patterns and flow speeds, helping you optimize routes based on live road conditions.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/here-location-maps](https://vinkius.com/mcp/here-location-maps)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **HERE (Location & Maps)** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `here-location-maps` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **HERE (Location & Maps)** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "here-location-maps": {
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
