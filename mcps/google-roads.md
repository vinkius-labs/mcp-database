# Google Roads MCP Server

Access Google Roads API — snap GPS tracks to roads, find nearest road segments, and get speed limit data for any road segment worldwide from any AI agent.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/google-roads)

## Overview
**Category:** industry-titans
**Tools Count:** 4

## Description
Connect your **Google Roads API** to any AI agent and take full control of GPS map matching, road segment identification, and speed limit data retrieval through natural conversation.

### What you can do

- **Snap to Roads** — Match GPS coordinate paths to the most likely roads travelled with interpolated points for smooth road geometry
- **Nearest Roads** — Find the nearest road segment for up to 100 individual GPS coordinates independently
- **Speed Limits** — Get posted speed limit data for specific road segments using place IDs from road matching
- **Snapped Speed Limits** — Snap GPS coordinates to roads AND get speed limits in a single combined request
- **Place ID Mapping** — Obtain Google place IDs for road segments that can be used with other Google Maps APIs
- **Fleet Tracking** — Clean noisy GPS traces from fleet vehicles for accurate route visualization
- **GPS Correction** — Convert raw GPS points into accurate road-level positions for mapping applications

### How it works

1. Subscribe to this server
2. Enter your Google Maps Platform API key with Roads API enabled
3. Start matching GPS data to roads from Claude, Cursor, or any MCP-compatible client

No more manual map matching or noisy GPS data visualization. Your AI acts as a dedicated GPS data analyst and road matching assistant.

### Who is this for?

- **Fleet Managers** — clean GPS tracks from vehicles, identify roads travelled, and monitor speed compliance
- **Mapping Developers** — convert raw GPS traces into clean road geometries for visualization and analysis
- **Safety Analysts** — retrieve speed limit data for road segments to analyze driver behavior and compliance
- **GIS Professionals** — snap scattered GPS points to road networks for spatial analysis and cartography


## Available Tools
- **get_nearest_roads**: Returns the snapped coordinate, the original coordinate, and the place ID for each nearest road segment. Unlike snapToRoads which assumes coordinates form a continuous path, nearestRoads treats each point independently. Essential for reverse geocoding, finding which road a vehicle is on, identifying road segments for individual location points, and mapping scattered GPS points to roads. Each point is matched to the nearest road segment within a reasonable distance. Place IDs can be used with the speed limits endpoint. AI agents should reference this when users ask "what road is at these coordinates", "find the nearest road for each GPS point", or need to map individual location points to road segments without assuming a path.

Get the nearest road segments for up to 100 individual GPS coordinates
- **snap_to_roads**: Returns snapped coordinates with place IDs, original coordinates, and interpolated points along the road. Essential for map matching, GPS track correction, route reconstruction, fleet tracking visualization, and converting raw GPS traces into clean road geometries. The path parameter accepts up to 100 coordinate pairs in "lat,lng|lat,lng" format. Set interpolate=true to return additional points between input coordinates for smoother road geometry. Place IDs returned can be used with the speed limits endpoint to get speed limit data for each road segment. AI agents should use this when users ask "snap this GPS track to roads", "match these coordinates to the actual roads travelled", or need to clean up noisy GPS data for mapping and visualization.

Snap GPS coordinates to the most likely roads travelled using Google Roads API
- **get_snapped_speed_limits**: Snaps GPS coordinates to the nearest road segments and returns both the snapped coordinates with place IDs AND the speed limits for each road segment. This is more efficient than making separate calls to snapToRoads and then speedLimits. Returns snapped points with place IDs, original coordinates, and speed limit data in km/h for each road segment. Essential for applications that need both map-matched road geometry and speed limit data, such as fleet management, driver safety monitoring, route planning with speed awareness, and GPS track analysis. AI agents should reference this when users ask "snap these GPS points to roads and show speed limits", "get both snapped coordinates and speed limits for this route", or need combined road matching and speed limit data in one call.

Snap GPS coordinates to roads and get speed limits in a single request
- **get_speed_limits**: Returns speed limit values in km/h along with the place IDs and corresponding road segment information. Place IDs are obtained from the snapToRoads or nearestRoads responses. Essential for speed compliance monitoring, fleet safety management, driver behavior analysis, and road safety applications. Speed limits reflect posted legal limits and may vary by road type, urban/rural designation, and local regulations. AI agents should use this when users ask "what is the speed limit on this road segment", "get speed limits for these place IDs", or need speed limit data for specific road segments identified through map matching.

Get speed limit data for specific road segments using place IDs


## Installation & Usage

To install and use the **Google Roads** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/google-roads](https://vinkius.com/mcp/google-roads)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
