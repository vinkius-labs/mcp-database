# Strava MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/strava-alternative)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/strava-alternative-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/strava-alternative-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Connect Strava to your AI agent to track activities, analyze athlete performance stats, and manage segments or routes directly.

## Description
Connect your **Strava** account to any AI agent to analyze your fitness data and manage your athletic activities through natural conversation.

### What you can do

- **Athlete Insights** — Retrieve your profile details, all-time performance stats, and specific heart rate or power zones.
- **Activity Management** — List recent activities, fetch detailed metrics for specific sessions, or manually create and update activity metadata.
- **Social & Engagement** — List comments and kudos on activities to stay connected with your athletic community.
- **Segments & Routes** — Explore popular segments, list your starred segments, and fetch detailed route information including GPX/TCX exports.
- **Data Streams** — Access raw data streams for activities, segments, and routes for deep performance analysis.

### How it works

1. Subscribe to this server
2. Enter your Strava Access Token
3. Start analyzing your fitness journey from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Athletes & Cyclists** — analyze your training blocks and heart rate zones without digging through the mobile app.
- **Coaches** — quickly retrieve athlete stats and activity laps to provide data-driven feedback.
- **Data Enthusiasts** — export routes and activity streams directly into your workflow for custom analysis.


## Available Tools
- **create_activity**: Create a manual activity
- **explore_segments**: Explore segments by bounds
- **export_route_gpx**: Export route as GPX
- **export_route_tcx**: Export route as TCX
- **get_activity_streams**: Get activity streams
- **get_activity**: Get activity details
- **get_activity_zones**: Get zones for an activity
- **get_athlete_stats**: Get athlete stats
- **get_authenticated_athlete**: Get the currently authenticated athlete
- **get_athlete_zones**: Get athlete heart rate and power zones
- **get_club**: Get club details
- **get_route_streams**: Get route streams
- **get_route**: Get route details
- **get_segment_effort_streams**: Get segment effort streams
- **get_segment_effort**: Get segment effort details
- **get_segment_streams**: Get segment streams
- **get_segment**: Get segment details
- **list_activity_comments**: List comments for an activity
- **list_activity_kudos**: List kudoers for an activity
- **list_activity_laps**: List laps for an activity
- **list_athlete_activities**: List athlete activities
- **list_athlete_clubs**: List athlete clubs
- **list_athlete_routes**: List athlete routes
- **list_club_activities**: List club activities
- **list_club_admins**: List club administrators
- **list_club_members**: List club members
- **list_segment_efforts**: List segment efforts
- **list_starred_segments**: List starred segments
- **star_segment**: Star or unstar a segment
- **update_activity**: Update an activity
- **update_athlete**: Update the authenticated athlete


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Strava** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List my last 5 activities on Strava."

**🤖 AI Agent:**
> I've retrieved your recent activities. Your last sessions include a 'Morning Run' (5.2km), an 'Evening Ride' (25km), and a 'Swim' (1500m). Would you like the details for any of these?

---

**👤 You:**
> "Show me my heart rate and power zones."

**🤖 AI Agent:**
> Fetching your zones... Your Heart Rate zones are set from Zone 1 (110-130 bpm) up to Zone 5 (175+ bpm). Your Power zones range from Z1 (0-150W) to Z7 (450W+).

---

**👤 You:**
> "Update activity 123456789: change the name to 'Epic Trail Run' and add 'Great views!' to the description."

**🤖 AI Agent:**
> Activity 123456789 has been updated successfully. The name is now 'Epic Trail Run' and the description has been appended with your notes.


## Installation & Usage

To install and use the **Strava** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/strava-alternative](https://vinkius.com/mcp/strava-alternative)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
