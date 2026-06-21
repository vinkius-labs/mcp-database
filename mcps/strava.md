# Strava MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/strava)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [industry-titans](../categories/industry-titans.md)

Manage activities, athlete stats, and routes on Strava with AI agents.

## Description
Connect your **Strava** account to any AI agent to automate your athletic performance tracking and activity orchestration. Strava provides a premier platform for athletes to track their progress, and this integration allows you to retrieve activity metadata, monitor athlete statistics, and explore routes through natural conversation.

### What you can do

- **Activity & Workout Orchestration** — List all your athletic activities and retrieve detailed metadata, including distance, heart rate, and elevation programmatically.
- **Athlete Performance Monitoring** — Access and monitor your athlete statistics and profile metadata to track your progress over time directly from the AI interface.
- **Route & Segment Intelligence** — List available routes and starred segments to ensure your training paths are always synchronized via natural language.
- **Club & Social Insight** — Access and monitor the clubs you belong to to maintain a clear overview of your athletic community engagement.
- **Data Management** — Create and update activities programmatically to ensure your training log is always current and accurate using simple AI commands.

### How it works

1. Subscribe to this server
2. Enter your Strava Access Token (OAuth2) from your developer settings
3. Start managing your athletic data from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Athletes & Fitness Enthusiasts** — quickly retrieve recent workout details and monitor performance stats without switching apps.
- **Coaches & Trainers** — automate the retrieval of athlete activity logs and monitor training progress via natural conversation.
- **Data Analysts** — streamline the retrieval of workout metadata and monitor segment performance directly within the chat.


## Available Tools
- **create_manual_activity**: Add manual workout
- **get_activity_details**: Get activity info
- **get_athlete_profile**: Get your info
- **get_route_details**: Get route info
- **get_segment_details**: Get segment info
- **get_athlete_statistics**: Check totals
- **list_athlete_activities**: List your activities
- **list_athlete_clubs**: List joined clubs
- **list_athlete_routes**: List your routes
- **list_starred_segments**: List favorite segments
- **test_strava_auth**: Verify API key
- **modify_activity**: Update workout info


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Strava** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List my last 5 activities on Strava."

**🤖 AI Agent:**
> I've retrieved your recent activities. Your last 5 workouts include a 'Morning Run' (5.2 km), 'Evening Cycle' (20.5 km), and three others. Would you like the detailed stats for the run?

---

**👤 You:**
> "Show me my training summary for the past week with distance, elevation, and heart rate zones."

**🤖 AI Agent:**
> Weekly training summary (May 12-18). 6 activities logged. Running (3): 28.4 km total, 342m elevation, avg pace 5:12/km, avg HR 152 bpm. Cycling (2): 89.6 km, 890m elevation, avg speed 28.4 km/h, avg HR 142 bpm. Swimming (1): 2.4 km, 45 minutes, avg pace 1:52/100m. Total distance: 120.4 km. Total time: 8h 23m. Calories: 5,670. HR zones: Zone 1 (12%), Zone 2 (34%), Zone 3 (28%), Zone 4 (18%), Zone 5 (8%). Training load: 4.2/5 (optimal). Fitness trend: +3% vs last week.

---

**👤 You:**
> "Compare my running performance this month versus last month with pace and distance trends."

**🤖 AI Agent:**
> Running comparison: May vs April. May (so far): 12 runs, 98.4 km, avg pace 5:08/km, best pace 4:32/km, elevation 1,230m. April: 14 runs, 112 km, avg pace 5:22/km, best pace 4:45/km, elevation 980m. Improvements: avg pace -14 sec/km (2.7% faster), best pace -13 sec/km. On track to exceed April distance (projected 118 km). Longest run: May 10.2 km vs April 8.8 km. Consistency: May avg 3.2 runs/week vs April 3.5. Heart rate efficiency improved: same pace at 5 bpm lower avg HR.


## ❓ FAQ

**Q: How do I find my Strava Access Token?**
Log in to [**Strava Developers**](https://www.strava.com/settings/api), create an API application, and you will find your Access Token in the settings. Note that you may need to use the OAuth flow to generate a long-lived or refreshed token.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/strava](https://vinkius.com/mcp/strava)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Strava** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `strava` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Strava** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "strava": {
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
