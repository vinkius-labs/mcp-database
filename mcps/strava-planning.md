# Strava Planning MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/strava-planning)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Plan routes, export GPX/TCX, create activities, manage gear, and star segments on Strava.

## Description
Connect **Strava Planning** to any AI agent and manage your training logistics — route creation, GPX/TCX export, manual activity logging, gear tracking, segment favoriting, and profile management.

### What you can do
- **Route Management** — List, view, and analyze all your saved routes with distance, elevation, and descriptions
- **Route Streams** — Get GPS coordinates, elevation profiles, and distance data for any route
- **Route Export** — Export routes to GPX and TCX formats for GPS devices (Garmin, Wahoo, etc.)
- **Manual Activity Creation** — Log activities not recorded by Strava (gym, yoga, cross-training) with full details
- **Activity Updates** — Edit activity names, descriptions, assign gear, mark commutes or indoor sessions
- **File Uploads** — Upload FIT, TCX, or GPX files for processing by Strava with status tracking
- **Segment Management** — Star (favorite) or unstar segments for quick training access
- **Athlete Profile** — View and update your profile information including weight for accurate power-to-weight ratios
- **Athlete Zones** — Review your heart rate and power zone configurations
- **Gear Details** — Track equipment mileage, models, and primary gear assignments

### How it works
1. Subscribe to this server
2. Enter your Strava Access Token (OAuth2)
3. Start planning routes and managing training data from Claude, Cursor, or any MCP-compatible client

### Who is this for?
- **Route Planners** — create, review, and export training routes to GPS devices for guided workouts
- **Multi-Sport Athletes** — log non-GPS activities (gym, pool, yoga) alongside Strava-tracked workouts
- **Equipment Managers** — track bike and shoe mileage for maintenance planning and rotation
- **Data Exporters** — export route data in GPX/TCX formats for use with other platforms and devices


## Available Tools (14)
- **get_athlete**: Use this to review personal profile details, check equipment assignments, or verify account settings.

Get the authenticated athlete's profile information
- **get_athlete_zones**: Required for zone-based training analysis. Use this to review training zones, ensure zones are correctly set, or use zone data for activity analysis.

Get the athlete's custom heart rate and power zones
- **create_activity**: Required: name (activity name), type (activity type like "Run", "Ride", "Swim", "Walk", "Hike"), startDate (ISO 8601 format), elapsedTime (seconds). Optional: description, distance (meters). Use this to log activities recorded outside of Strava (gym workouts, yoga, cross-training, etc.). Activity types must match Strava's valid types list.

Create a manual activity in Strava
- **get_gear**: The gearId is found in activity data or athlete profile. Use this to check equipment mileage for maintenance planning or to analyze performance with specific gear.

Get details about a piece of equipment (bike, shoes) tracked in Strava
- **get_route**: The routeId is found in Strava route URLs. Use this to review route characteristics before training or to plan similar routes.

Get detailed information about a specific Strava route
- **export_route_gpx**: GPX files can be downloaded and loaded onto GPS devices (Garmin, Wahoo, etc.) for navigation. The routeId is from Strava route URLs. Use this to export routes to your GPS device for guided training.

Get the GPX export URL for a Strava route
- **get_route_streams**: The "types" parameter is comma-separated: "latlng", "altitude", "distance". Use this to preview a route's elevation profile, understand the terrain, or export GPS data for navigation.

Get elevation and GPS data streams for a Strava route
- **export_route_tcx**: TCX files include route data with additional training metadata. Compatible with Garmin Training Center and other fitness platforms. Use this to export routes with training metadata.

Get the TCX export URL for a Strava route
- **list_routes**: Each route includes: name, distance, elevation gain, type (ride/run), description, and whether it's private. Use this to review saved routes, plan upcoming workouts, or export route data for GPS devices.

List all routes created by the authenticated athlete
- **star_segment**: Set starred=true to favorite, starred=false to unfavorite. The segmentId is from Strava segment URLs. Use this to manage your favorite segments for quick access and training focus.

Star (favorite) or unstar a Strava segment
- **update_activity**: The activityId is the numeric ID. Updatable fields: name, description, sport_type, gear_id (to assign equipment), commute (mark as commute: "true"/"false"), trainer (mark as indoor: "true"/"false"). Use this to correct activity details, assign gear, or add descriptions after the fact.

Update an existing Strava activity
- **update_athlete**: Currently only "weight" (in kg) is supported by the API. Accurate weight is important for power-to-weight ratio calculations and performance analysis. Use this when your weight changes to keep performance metrics accurate.

Update the authenticated athlete's profile information
- **upload_activity**: Supported data_type: "fit", "fit.gz", "tcx", "tcx.gz", "gpx", "gpx.gz". Returns an upload ID to check status with get_upload_status. Note: Actual file upload requires multipart/form-data with the file content. This endpoint initiates the process. Check upload status periodically — processing takes 10-60 seconds.

Upload an activity file (FIT, TCX, GPX) to Strava for processing
- **get_upload_status**: Status values: "Your activity is ready" (success), "Your activity is still processing" (wait and retry), or error messages. The uploadId is returned by upload_activity. Poll this endpoint every 5-10 seconds after upload until ready.

Check the status of a Strava activity upload


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Strava Planning** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all my saved routes."

**🤖 AI Agent:**
> Found 8 routes: 1) Morning Loop — 32.5 km, 450m elev, cycling. 2) Hill Repeats — 5.2 km, 280m elev, running. 3) Weekend Century — 160 km, 1,850m elev, cycling. 4) Recovery Run — 8 km, 50m elev, running. 5) Coastal Ride — 45 km, 320m elev, cycling.

---

**👤 You:**
> "Export route 12345 to GPX format."

**🤖 AI Agent:**
> Route 12345 (Morning Loop) exported to GPX. Download at: https://www.strava.com/api/v3/routes/12345/export_gpx. The file contains 32.5 km of GPS track with 450m elevation gain. Compatible with Garmin Edge, Wahoo ELEMNT, and other GPS cycling computers.

---

**👤 You:**
> "Create a manual activity for today's gym session."

**🤖 AI Agent:**
> Activity created: "Gym Session" — Type: Workout, Date: 2024-03-15 07:00, Duration: 45 min. Description: "Strength training - upper body focus". Activity ID: 9876543210. Now visible in your Strava feed.


## ❓ FAQ

**Q: How do I export a route to my GPS device?**
First, use list_routes to find your route ID. Then use export_route_gpx or export_route_tcx with that route ID. The GPX file can be downloaded and loaded onto Garmin, Wahoo, or other GPS devices for turn-by-turn navigation during your workout.

**Q: Can I log activities that Strava doesn't automatically track?**
Yes! Use create_activity to manually log any workout — gym sessions, yoga, swimming, hiking, cross-training. Provide the name, type (e.g., "Workout", "Yoga", "Swim"), start date, elapsed time, and optionally distance and description. This keeps all your training in one place.

**Q: How do I track my bike and shoe mileage?**
Use get_gear with the gear ID to see total accumulated distance. Gear IDs are found in your athlete profile or assigned to activities. You can assign gear to activities using update_activity with the gear_id parameter. Track mileage to know when to replace chains, tires, or running shoes.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/strava-planning](https://vinkius.com/mcp/strava-planning)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Strava Planning** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `strava-planning` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Strava Planning** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "strava-planning": {
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
