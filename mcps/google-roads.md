# Google Roads MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/google-roads)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/google-roads-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/google-roads-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [industry-titans](../categories/industry-titans.md)

Access Google Roads API — snap GPS tracks to roads, find nearest road segments, and get speed limit data for any road segment worldwide from any AI agent.

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


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Google Roads** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Snap these GPS coordinates to roads: 40.7128,-74.0060|40.7135,-74.0055|40.7142,-74.0048"

**🤖 AI Agent:**
> Snapping GPS coordinates to roads... 3 points snapped successfully. Point 1: Original (40.712800, -74.006000) -> Snapped to (40.712820, -74.005980), placeId: ChIJd8BlQ2BZwokRAFUEcm_qrcA. Point 2: Original (40.713500, -74.005500) -> Snapped to (40.713510, -74.005490), placeId: ChIJd8BlQ2BZwokRAFUEcm_qrcB. Point 3: Original (40.714200, -74.004800) -> Snapped to (40.714190, -74.004810), placeId: ChIJd8BlQ2BZwokRAFUEcm_qrcC. All points snapped to Broadway in Lower Manhattan. Would you like speed limit data for these road segments?

---

**👤 You:**
> "Get speed limits for these place IDs: ChIJd8BlQ2BZwokRAFUEcm_qrcA|ChIJd8BlQ2BZwokRAFUEcm_qrcB"

**🤖 AI Agent:**
> Fetching speed limits... 2 road segments found. Segment 1: placeId ChIJd8BlQ2BZwokRAFUEcm_qrcA, speed limit 40 km/h (25 mph), road name Broadway, New York NY. Segment 2: placeId ChIJd8BlQ2BZwokRAFUEcm_qrcB, speed limit 40 km/h (25 mph), road name Broadway, New York NY. Both segments are in a downtown urban zone with reduced speed limits.

---

**👤 You:**
> "Find the nearest road to these coordinates: 34.0522,-118.2437 and 34.0530,-118.2445"

**🤖 AI Agent:**
> Finding nearest roads... Point 1 (34.0522, -118.2437) snapped to Spring Street, Los Angeles CA, placeId: ChIJYWRSrVHHwoARpVl2b3cFzQE. Point 2 (34.0530, -118.2445) snapped to Broadway, Los Angeles CA, placeId: ChIJYWRSrVHHwoARpVl2b3cFzQF. Both points are in downtown Los Angeles within 15 meters of major roads. Would you like speed limits for these road segments?


## Installation & Usage

To install and use the **Google Roads** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/google-roads](https://vinkius.com/mcp/google-roads)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
