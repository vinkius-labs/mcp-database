# Strava Social MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/strava-social)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Explore Strava activities feed, kudos, comments, clubs, and discover new segments.

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


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Strava Social** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Show my recent activities."

**🤖 AI Agent:**
> Recent activities: 1) Morning Ride — 45.2 km, 1h32m, 520m elev, 12 kudos. 2) Easy Run — 8.5 km, 42min, 85m elev, 8 kudos. 3) Recovery Ride — 22 km, 48min, 120m elev, 5 kudos. 4) Tempo Run — 10 km, 38min, 95m elev, 15 kudos.

---

**👤 You:**
> "Explore cycling segments in Manhattan, NYC."

**🤖 AI Agent:**
> Found 25 segments in Manhattan. Top climbs: 1) Cat 1 climb: West Side Highway (2.1 km, 4.2% avg) — 3,420 efforts. 2) Cat 3: Central Park North Hill (0.8 km, 8.1% avg) — 1,890 efforts. 3) Cat 4: Broadway Sprint (1.5 km, 2.1% avg) — 2,150 efforts. Most attempted: Central Park Full Loop (6.2 km).

---

**👤 You:**
> "Show comments on my latest activity."

**🤖 AI Agent:**
> Found 5 comments: 1) Sarah M.: "Great pace on that ride! 💪" 2) Tom K.: "Nice work! How did the new route feel?" 3) Lisa P.: "Solid effort 🚴" 4) Mike R.: "Let's do this route together next week" 5) Anna D.: "Impressive elevation gain!"


## ❓ FAQ

**Q: Can I see who liked my activities?**
Yes! Use the get_activity_kudos tool with any activity ID. It returns the full list of athletes who gave kudos to that activity, including their names, cities, and profile pictures. This helps you understand who's following and supporting your training.

**Q: How can I discover popular segments in a new city?**
Use the explore_segments tool with a bounding box of the area you're interested in. The bounds format is "southwest_lng,southwest_lat,northeast_lng,northeast_lat". For example, "-74.00,40.70,-73.95,40.75" covers Manhattan. You can filter by activity_type ("riding" or "running") and difficulty category (0-5, where 0 is hardest).

**Q: Can I see what my club members have been doing?**
Yes! Use list_club_activities with the club ID. It returns the 30 most recent activities from club members with athlete names, activity types, distances, and dates. Paginate through results to see more. This is great for staying connected with your training group's activities.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/strava-social](https://vinkius.com/mcp/strava-social)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Strava Social** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `strava-social` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Strava Social** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "strava-social": {
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
