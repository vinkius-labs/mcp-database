# IndoorAtlas (Indoor Positioning) MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/indooratlas-indoor-positioning)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [iot-hardware](../categories/iot-hardware.md)

Manage indoor positioning via IndoorAtlas — list venues, upload floorplans, and analyze positioning sessions.

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


## Available Tools (10)
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


## 💬 Prompt Examples

Here are some examples of how you can interact with the **IndoorAtlas (Indoor Positioning)** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all indoor venues in my IndoorAtlas account"

**🤖 AI Agent:**
> I've found 3 venues: 'Corporate HQ' (ID: v-123), 'Retail Mall' (ID: v-456), and 'Logistic Warehouse' (ID: v-789). All are currently mapped and calibrated. Which one would you like to see floorplans for?

---

**👤 You:**
> "Check the calibration paths for the 3rd floor of the 'Retail Mall'"

**🤖 AI Agent:**
> Retrieving calibration paths… I've fetched the walk paths for Floor 3 (ID: fp-987). The GeoJSON data shows extensive coverage in the main aisles, but the storage areas appear to need more fingerprinting. Would you like the coordinate list?

---

**👤 You:**
> "List the most recent positioning sessions recorded today"

**🤖 AI Agent:**
> I've found 12 positioning sessions from today. The longest session lasted 45 minutes in the 'Corporate HQ'. Average accuracy across all sessions is 2.4 meters. Would you like to inspect the trace data for the most active session?


## ❓ FAQ

**Q: How do I start the map generation process for a new floor plan?**
Use the `trigger_map_generation` tool with your Floorplan ID. This initiates the server-side computation that creates the positioning model. It's a critical step before indoor positioning can work on that level.

**Q: Can I determine a position using Wi-Fi scans through my agent?**
Yes. The `position_from_wifi_scan` tool allows you to submit observed Wi-Fi signal strengths. Your agent will return estimated coordinates and floor level, which is perfect for server-side positioning logic.

**Q: How can I analyze visitor traffic patterns in our building?**
Use the `list_positioning_sessions` tool to retrieve historical traces. Your agent can help you analyze occupancy patterns and dwell times by processing the timestamped coordinate fixes from past sessions.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/indooratlas-indoor-positioning](https://vinkius.com/mcp/indooratlas-indoor-positioning)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **IndoorAtlas (Indoor Positioning)** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `indooratlas-indoor-positioning` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **IndoorAtlas (Indoor Positioning)** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "indooratlas-indoor-positioning": {
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
