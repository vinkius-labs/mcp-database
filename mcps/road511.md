# Road511 MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/road511)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [data-analytics](../categories/data-analytics.md)

Access real-time US and Canada traffic data via Road511 — track incidents, monitor cameras, check road conditions, and analyze trends from any AI agent.

## Description
Connect your **Road511** real-time traffic data API to any AI agent and take full control of North American traffic monitoring, incident tracking, infrastructure awareness, and operational analytics through natural conversation.

### What you can do

- **Traffic Incidents** — Track real-time incidents, construction, closures, special events, and weather advisories across all 50 US states and 13 Canadian provinces
- **Traffic Cameras** — Access live traffic camera feeds for visual traffic monitoring across North America
- **Road Conditions** — Check current road conditions, surface status, and weather impacts on roadways
- **EV Charging** — Find electric vehicle charging stations across the US and Canada for trip planning
- **Rest Areas** — Locate rest areas, weigh stations, and ferry terminals along major corridors
- **Weather Stations** — Access road-side weather station data for weather-aware routing
- **Geospatial Mapping** — Get all data in GeoJSON format for direct mapping and GIS integration
- **Incident Analytics** — Analyze traffic incident trends, resolution times, and operational metrics
- **System Health** — Monitor API health and data source status across 65 jurisdictions

### How it works

1. Subscribe to this server
2. Enter your Road511 API key (free 14-day trial available)
3. Start monitoring North American traffic from Claude, Cursor, or any MCP-compatible client

No more navigating multiple state 511 websites or manually checking traffic cameras. Your AI acts as a dedicated traffic analyst and route planning assistant.

### Who is this for?

- **Fleet Operators** — monitor incidents, plan routes, and track road conditions for logistics optimization
- **Daily Commuters** — check traffic incidents and construction before heading out
- **EV Drivers** — find charging stations and plan electric vehicle trips
- **Traffic Analysts** — study incident trends, resolution metrics, and traffic pattern analytics


## Available Tools (8)
- **get_clearance**: Returns average resolution times by incident type, severity, jurisdiction, and time period. Essential for operational efficiency analysis, resource planning, performance benchmarking, and understanding how quickly traffic incidents are resolved in different regions. AI agents should use this when users ask "what is the median resolution time for incidents in California", "how long do major incidents take to clear in Texas", or need performance metrics for traffic incident management analysis.

Get incident resolution time metrics (P50/P95) for operational analysis
- **get_events_geojson**: Each feature contains event properties (type, severity, jurisdiction, road, times, status, descriptions) in the properties object and point/line geometry in the geometry object. Supports all the same filtering parameters as get_events. Essential for mapping applications, spatial analysis, GIS integration, and visualization dashboards. AI agents should use this when users need to plot traffic events on a map, perform spatial queries, or integrate with GeoJSON-based mapping tools.

Get traffic events in GeoJSON format for mapping and spatial analysis
- **get_events**: Returns event type, severity (minor, moderate, major, critical, info), jurisdiction, road affected, start and end times, lifecycle status, geometry (line/point), and detailed descriptions. Supports filtering by jurisdiction (e.g., CA), type (incidents, construction, closures, events, advisories), severity, road name, status, and geographic area (bbox, lat/lon/radius). Essential for real-time traffic awareness, route planning, delivery logistics, and commuter decision-making. AI agents should use this when users ask "what incidents are on I-405", "show construction in California", or need traffic event data for route optimization.

Get traffic incidents, construction, closures, and events across US and Canada
- **get_features_geojson**: Each feature includes properties (type, jurisdiction, status, camera URL, road condition, weather data, EV charger info) and point geometry. Supports all the same filtering parameters. Essential for mapping applications, GIS workflows, spatial databases, and visualization dashboards. AI agents should reference this when users need to plot infrastructure features on a map, integrate with GeoJSON tools, or perform spatial analysis on road infrastructure.

Get road infrastructure features in GeoJSON format for mapping and GIS integration
- **get_features**: Returns type, jurisdiction, coordinates, status, and feature-specific details. Use when users ask about traffic cameras, EV chargers, rest areas, road conditions, or need infrastructure data for mapping.

Get road infrastructure features including cameras, road conditions, weather stations, and more
- **get_health**: Returns API availability, response times, data source connectivity (per jurisdiction), last update timestamps, and system alerts. Essential for monitoring API reliability, verifying data freshness, troubleshooting integration issues, and ensuring production system uptime. AI agents should use this as a diagnostic tool when users report missing data, when debugging integration issues, or as a periodic health check before making complex traffic data queries.

Check API health and data source status
- **get_summary**: Returns event counts by type and severity, active camera counts, data source status (healthy, degraded, down), refresh rates, and data freshness indicators. Essential for data quality monitoring, system health checks, understanding data coverage by region, and verifying API reliability before production use. AI agents should use this when users ask "how many active incidents are there nationwide", "is the California data source healthy", or need a system-wide overview of Road511 data quality and coverage.

Get summary statistics and data source health across all jurisdictions
- **get_trends**: Returns incident counts over time, severity distributions, trend directions (increasing, decreasing, stable), peak incident times, and comparative analysis between regions. Essential for traffic pattern analysis, operational planning, resource allocation, and understanding temporal traffic safety trends. AI agents should use this when users ask "are incidents increasing in Texas this week", "show me traffic incident trends for the past month", or need analytical data for traffic safety reporting.

Get traffic incident trends and time-series analytics


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Road511** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Show me all active traffic incidents on I-5 in California."

**🤖 AI Agent:**
> Querying Road511 for incidents on I-5 in California... I found 7 active events: Major accident at mile marker 342 near Grapevine — 2 lanes blocked, CHP on scene, estimated clearance 45 minutes. Construction zone between Bakersfield and Lost Hills — right lane closed until 6 PM, expect 15-minute delays. Disabled vehicle at mile marker 198 near Coalinga — shoulder blocked, tow truck dispatched. Weather advisory for mountain sections — chains required, reduce speed. Plus 3 additional minor incidents with minimal impact. Would you like me to plot these on a map or suggest alternate routes?

---

**👤 You:**
> "Find traffic cameras near downtown Seattle."

**🤖 AI Agent:**
> Searching for traffic cameras near downtown Seattle (lat: 47.6062, lon: -122.3321)... Found 14 active cameras within 10km radius: I-5 at Mercer Street — live feed available, currently showing moderate congestion. SR-99 at Aurora Bridge — live feed available, free-flowing traffic. I-90 at Mount Baker Tunnel — live feed available, heavy eastbound traffic. SR-520 floating bridge — 3 cameras, moderate westbound flow. Plus 10 additional cameras covering major intersections and highway interchanges. All cameras operational with live video feeds. Would you like direct links to any specific camera feed?

---

**👤 You:**
> "What is the overall traffic health across all states right now?"

**🤖 AI Agent:**
> Fetching Road511 system summary... Currently tracking across 65 jurisdictions (50 US states + 13 Canadian provinces). Active incidents: 1,247 (312 major, 523 moderate, 412 minor). Construction zones: 892 active. Closures: 67 active. Data source health: 61 of 65 jurisdictions reporting healthy, 3 degraded, 1 temporarily down. Average data freshness: 2.3 minutes. Camera network: 8,456 active feeds operational. API response time: 142ms average. Would you like a breakdown by specific state or incident type?


## ❓ FAQ

**Q: Can my AI check for traffic incidents on a specific highway like I-405 in California?**
Yes! Use the `get_events` tool with road=I-405 and jurisdiction=CA to filter incidents specifically on that highway. You can further filter by type (incidents, construction, closures) and severity (minor, moderate, major, critical). The results include incident descriptions, affected lanes, estimated clearance times, and alternate route suggestions. For mapping visualization, use `get_events_geojson` to get the same data in GeoJSON format ready for Mapbox or Leaflet.

**Q: How do I find traffic cameras and EV charging stations along my route?**
Use the `get_features` tool with type=cameras to find all traffic cameras in a jurisdiction, or type=ev_chargers for EV charging stations. You can filter by bounding box (bbox) or by radius from a lat/lon point. For mapping applications, use `get_features_geojson` which returns data in GeoJSON format ready for direct integration with mapping libraries. Camera features include live stream URLs and road conditions include surface status and weather impacts.

**Q: Can I analyze traffic incident trends to understand if traffic is getting worse in my state?**
Absolutely! Use `get_trends` with your jurisdiction code (e.g., jurisdiction=CA for California) to get time-series incident data showing whether incidents are increasing, decreasing, or stable over time. Use `get_clearance` to understand how quickly incidents are being resolved (P50 median and P95 resolution times). Combined with `get_summary` for current snapshot data, you can build comprehensive traffic safety and efficiency reports. This is perfect for transportation planning, resource allocation, and operational performance benchmarking.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/road511](https://vinkius.com/mcp/road511)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Road511** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `road511` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Road511** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "road511": {
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
