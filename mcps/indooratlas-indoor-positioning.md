# IndoorAtlas (Indoor Positioning) MCP Server

Manage indoor positioning via IndoorAtlas — list venues, upload floorplans, and analyze positioning sessions.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/indooratlas-indoor-positioning)

## Overview
**Category:** iot-hardware
**Tools Count:** 10

## Description
Connect your **IndoorAtlas** account to any AI agent and take full control of your smart building infrastructure and indoor positioning services through natural conversation.

### What you can do

- **Venue Management** — List all registered indoor venues and retrieve detailed metadata including geographic anchor points and floor counts directly from your agent
- **Floorplan Orchestration** — Upload new floor plans as GeoJSON and manage geo-referencing to real-world coordinates for accurate indoor positioning
- **Map Generation** — Trigger the radio map generation process to compute positioning models from signal fingerprint data and floor geometry
- **Analytics & Sessions** — Retrieve historical positioning sessions and trace data to analyze occupancy patterns, dwell times, and path optimization
- **Wi-Fi Positioning** — Determine indoor location from Wi-Fi scans using the Positioning API to receive estimated coordinates and floor levels
- **Calibration Audit** — Inspect fingerprinting walk paths to assess calibration coverage and identify areas needing additional signal mapping

### How it works

1. Subscribe to this server
2. Enter your IndoorAtlas API Key
3. Start managing your indoor spaces from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Smart Building Developers** — integrate indoor location services into AI agents and monitor venue calibration statuses
- **GIS Analysts** — manage indoor floor plans and coordinate geo-referencing through natural conversation without complex GIS software
- **Operations Managers** — audit occupancy analytics and positioning session data to optimize building usage and visitor flows


## Available Tools
- **upload_floorplan_geojson**: After upload, trigger map generation to enable positioning on this floor.

Upload a new floor plan to an IndoorAtlas venue as a GeoJSON document, geo-referencing the indoor map image to real-world coordinates for accurate positioning overlay
- **create_venue**: The venue serves as the top-level container for floor plans and positioning data. After creation, upload floor plan images and calibrate for positioning accuracy.

Create a new indoor venue in the IndoorAtlas platform by specifying the building name, geographic coordinates of the entrance, and initial configuration parameters for indoor positioning deployment
- **trigger_map_generation**: This is a critical step — positioning will not work on a floor until map generation completes successfully. The process is asynchronous and may take several minutes depending on floor plan complexity.

Trigger the IndoorAtlas radio map generation process for a specific floor plan, initiating the server-side computation that creates the positioning model from fingerprint data and floor plan geometry
- **get_fingerprint_paths**: Returns GeoJSON LineString features representing calibration paths. Use to assess calibration coverage and identify areas of the floor that need additional fingerprinting for better positioning accuracy.

Retrieve the fingerprinting walk paths recorded for a specific floor plan as GeoJSON, showing the routes surveyors walked while collecting Wi-Fi/BLE signal data for positioning calibration
- **get_session_data**: Returns the complete position trace as a series of timestamped fixes. Use for path visualization, behavioral analysis, and positioning quality assessment. Large sessions may contain thousands of position fixes.

Retrieve the full positioning trace data for a specific IndoorAtlas session, including timestamped coordinate fixes, floor transitions, accuracy metrics, and sensor readings throughout the session duration
- **get_venue_details**: Returns the venue configuration including coordinate reference, building dimensions, and mapping completeness metrics. Use to inspect a venue before deploying positioning or wayfinding features.

Retrieve detailed metadata for a specific IndoorAtlas venue including its geographic anchor point, floor count, total mapped area, calibration status, and associated floor plan identifiers
- **list_floorplans**: Returns an array of floor plan metadata objects ordered by floor number. Each entry includes the plan dimensions, pixel-to-meter scale, and whether radio map generation has been completed.

List all floor plans uploaded to a specific IndoorAtlas venue, returning floor plan IDs, floor numbers, dimensions, geo-alignment status, and map generation readiness for each level of the building
- **list_positioning_sessions**: Returns a paginated list of positioning sessions. Each session represents a continuous period of indoor tracking by a single device. Use for occupancy analytics, dwell time analysis, and path optimization studies.

List historical indoor positioning sessions recorded by IndoorAtlas, returning session IDs, start/end times, venue associations, and device information for analytics and path replay
- **list_venues**: Returns an array of venue objects. Each venue represents a physical building that has been set up for indoor positioning. Use to discover available venues before requesting floor plans or positioning data.

List all indoor venues registered in your IndoorAtlas organization, returning venue IDs, names, geographic coordinates, and configuration status for each mapped building or facility
- **position_from_wifi_scan**: Returns estimated coordinates with uncertainty radius. Use for server-side positioning when mobile SDK integration is not feasible.

Determine indoor position from a Wi-Fi access point scan using the IndoorAtlas Positioning API, submitting observed signal strengths to receive a calculated latitude, longitude, floor level, and accuracy estimate


## Installation & Usage

To install and use the **IndoorAtlas (Indoor Positioning)** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/indooratlas-indoor-positioning](https://vinkius.com/mcp/indooratlas-indoor-positioning)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
