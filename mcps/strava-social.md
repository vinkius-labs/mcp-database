# Strava Social MCP Server

Explore Strava activities feed, kudos, comments, clubs, and discover new segments.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/strava-social)

## Overview
**Category:** productivity
**Tools Count:** 10

## Description
Connect **Strava Social** to any AI agent and explore the social side of Strava — activity feeds, kudos, comments, club memberships, and segment discovery.

### What you can do
- **Activity Feed** — Browse your recent activities with full details, kudos counts, and comment counts
- **Activity Comments** — Read all comments on any activity with author names and text
- **Activity Kudos** — See who liked/supports your activities with full athlete profiles
- **Athlete Profile** — Get your Strava profile details including location, follower counts, and equipment
- **Club Membership** — List all clubs you belong to with member counts and sport types
- **Club Details** — Explore any club's description, location, and community focus
- **Club Members** — Browse club membership to find training partners and local athletes
- **Club Activities** — See what club members have been doing recently
- **Starred Segments** — Review all your favorited segments with PR times and characteristics
- **Segment Discovery** — Explore segments in any geographic area by bounding box, filterable by type and difficulty

### How it works
1. Subscribe to this server
2. Enter your Strava Access Token (OAuth2)
3. Start exploring your Strava social network from Claude, Cursor, or any MCP-compatible client

### Who is this for?
- **Social Athletes** — stay engaged with training partners, track kudos and community interaction
- **Club Organizers** — monitor club activity levels, member engagement, and discover new training routes
- **Training Groups** — explore what teammates are doing, find popular segments in your area
- **New City Explorers** — discover popular cycling/running segments when traveling to new cities


## Available Tools
- **list_activities**: Activities are sorted by most recent first. Optional filters: "before" (epoch timestamp, defaults to now), "after" (epoch timestamp for date range), "page" and "per_page" (pagination, max 200 per page, max 2000 total). Each activity includes: name, type, distance, moving_time, elevation, kudos_count, comment_count, start_date, and basic stats. Use this to get the activity feed, analyze recent workouts, or review training history. Epoch timestamps can be generated from dates.

List the authenticated athlete's activities with optional date filtering and pagination
- **get_athlete**: Use this to understand the athlete's identity, location, and equipment setup.

Get the authenticated athlete's profile information
- **get_club**: The clubId is found in Strava club URLs. Use this to explore club details before joining or to understand a club's focus and community.

Get detailed information about a specific Strava club
- **list_club_activities**: Each entry includes athlete name, activity name, type, distance, and date. Paginated (30 per page). The clubId is from Strava club URLs. Use this to stay updated on club training activity, discover what members are doing, or find group workout opportunities.

Get recent activities from members of a Strava club
- **list_club_members**: Paginated (30 per page). The clubId is from Strava club URLs. Use this to discover training partners in a club, find athletes in your area, or explore club community composition.

List members of a specific Strava club
- **list_athlete_clubs**: Each club includes name, member count, city, country, sport type (cycling/running/triathlon), and privacy status. Use this to discover club memberships, find training groups, or understand community affiliations.

List all clubs the authenticated athlete belongs to
- **get_activity_comments**: Each comment includes athlete name, text, and creation date. The activityId is the numeric ID from Strava activity URLs. Use this to see community engagement on a workout, read feedback, or track conversation around a specific activity.

Get all comments on a specific Strava activity
- **explore_segments**: g., "-74.00,40.70,-73.95,40.75" for Manhattan). Optional filters: activity_type ("running" or "riding"), min_cat/max_cat (category 0-5, where 0 is hardest/steepest). Returns segments with name, distance, elevation, grade, and climb category. Use this to discover new training routes, find popular segments in an area, or plan rides/runs in a new city.

Explore and discover Strava segments in a geographic area
- **get_activity_kudos**: Each entry includes athlete name, profile picture, and city. The activityId is the numeric ID from Strava. Use this to see who supported an activity, understand social engagement, or track training partners' interactions.

Get the list of athletes who gave kudos (likes) to a specific activity
- **list_starred_segments**: Each segment includes: name, distance, elevation gain, average grade, activity type, city, country, and the athlete's PR time if any. Use this to review favorite segments, plan training routes, or track progress on key segments over time.

List all segments starred (favorited) by the authenticated athlete


## Installation & Usage

To install and use the **Strava Social** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/strava-social](https://vinkius.com/mcp/strava-social)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
