# Strava Training MCP Server

Analyze Strava activities, segments, streams (HR, power, GPS), zones, laps, and athlete stats.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/strava-training)

## Overview
**Category:** data-analytics
**Tools Count:** 12

## Description
Connect **Strava Training** to any AI agent and unlock deep performance analysis from your Strava data — activity details, time-series streams, heart rate/power zones, segment efforts, lap splits, and lifetime athlete statistics.

### What you can do
- **Activity Details** — Full metrics: distance, time, elevation, HR, power, speed, weather, gear
- **Activity Streams** — Raw GPS, heart rate, power, cadence, altitude, speed, temperature, grade data
- **Activity Zones** — Heart rate and power zone distribution for training intensity analysis
- **Activity Laps** — Auto-split lap data with pace, distance, and elevation per split
- **Segment Efforts** — Find, compare, and analyze all efforts on any segment with detailed metrics
- **Segment Streams** — Elevation and grade profiles along segments for previewing difficulty
- **Segment Details** — Distance, elevation, grade, effort count, and personal records
- **Athlete Statistics** — Lifetime and recent totals for runs, rides, and all activities
- **Athlete Zones** — Personal heart rate and power zone configurations
- **Gear Tracking** — Equipment mileage, models, and primary gear assignments

### How it works
1. Subscribe to this server
2. Enter your Strava Access Token (OAuth2)
3. Start analyzing training data from Claude, Cursor, or any MCP-compatible client

### Who is this for?
- **Endurance Athletes** — analyze training volume, zone distribution, and segment PRs to optimize training plans
- **Coaches** — review athlete streams, zone data, and segment efforts to provide data-driven coaching
- **Cyclists** — analyze power data, segment efforts, and gear mileage for performance and maintenance planning
- **Runners** — track pace consistency through lap splits, elevation profiles, and heart rate trends


## Available Tools
- **get_activity**: The activityId is the numeric ID from Strava activity URLs (e.g., strava.com/activities/12345678 → 12345678). Use this for deep analysis of any workout, ride, or run.

Get detailed information about a specific Strava activity
- **get_activity_laps**: Each lap includes distance, moving time, average speed, elevation gain, and pace. GPS devices and Strava auto-split activities into laps (typically ~1km or ~1mi). Use this to analyze pace consistency, identify fast/slow sections, and compare splits within a single activity.

Get lap/split data for a Strava activity
- **get_activity_streams**: The "types" parameter is comma-separated stream types: "time", "distance", "latlng", "altitude", "velocity_smooth", "heartrate", "cadence", "watts", "temp", "moving", "grade_smooth". Example: "heartrate,watts,velocity_smooth" for HR, power, and speed data. Each stream returns an array of values with corresponding timestamps. Use this for detailed performance analysis, visualization, or export.

Get raw time-series data streams from a Strava activity (GPS, heart rate, power, cadence, altitude, speed, etc)
- **get_activity_zones**: Requires activity ID. This data helps understand training intensity and whether the workout targeted the correct zones. Only available for activities with heart rate or power data. Summit/subscription feature.

Get heart rate and power zone distribution for a Strava activity
- **get_athlete_stats**: Use the athlete's Strava numeric ID. Returns recent_run_totals, recent_ride_totals, all_run_totals, all_ride_totals. Great for performance overview and progress tracking.

Get consolidated activity statistics for any Strava athlete
- **get_athlete_zones**: Requires profile:read_all scope. Use this to understand training zones for zone-based analysis of activities and efforts.

Get the authenticated athlete's custom heart rate and power zones
- **get_gear**: The gear ID is found in activity data or athlete profile. Use this to track equipment mileage, plan maintenance, or analyze performance with specific gear.

Get details about a piece of equipment (bike, shoes) tracked in Strava
- **list_segment_efforts**: Filter by athlete_id (required), optionally segment_id to get efforts on a specific segment, and date range with start_date_local and end_date_local (ISO 8601 format). Use this to find PRs, analyze progress on segments over time, or compare multiple efforts on the same segment.

List all segment efforts for an athlete, optionally filtered by segment and date range
- **get_segment**: The segment ID is found in Strava segment URLs. Use this to discover segment characteristics before attempting it or to compare segments.

Get details of a Strava segment including distance, elevation, grade, and leaderboards
- **get_segment_effort**: Includes elapsed time, distance, average speed, heart rate, power, start date, and activity reference. The effort ID is found in segment effort listings or activity details. Use this to analyze specific KOM/QOM attempts and compare efforts on the same segment.

Get details of a specific segment effort (KOM/QOM/PR attempt)
- **get_segment_effort_streams**: Same format as activity streams but limited to the segment portion. The "types" parameter is comma-separated: "time", "distance", "latlng", "altitude", "velocity_smooth", "heartrate", "cadence", "watts". Use this for granular analysis of segment performance.

Get time-series data streams for a specific segment effort
- **get_segment_streams**: Useful for previewing a segment's difficulty profile before attempting it. The "types" parameter accepts "distance", "altitude", "grade_smooth". Use this to understand elevation changes and steepness patterns along a segment.

Get time-series data streams for a Strava segment (elevation profile, grade, etc)


## Installation & Usage

To install and use the **Strava Training** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/strava-training](https://vinkius.com/mcp/strava-training)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
