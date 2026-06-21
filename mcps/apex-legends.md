# Apex Legends MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/apex-legends)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [data-analytics](../categories/data-analytics.md)

Track Apex Legends player stats, match history, leaderboards, and server status directly from your AI agent.

## Description
Connect your AI agent to the **Apex Legends API** to access real-time game data, player performance metrics, and server health. This server provides a comprehensive suite of tools for competitive analysis and game tracking.

### What you can do

- **Player Statistics** — Retrieve detailed combat metrics, rank data, and legend-specific trackers using `get_player_stats_by_name` or `get_player_stats_by_uid`.
- **Match History** — Access recent match results and manage legacy tracking via `get_match_history` and `manage_legacy_match_history`.
- **Competitive Insights** — Check the current global leaderboards with `get_leaderboard` and see the RP/AP needed for Apex Predator rank with `get_predator_requirements`.
- **Live Game Data** — Stay updated with `get_map_rotation` for current and upcoming maps, and monitor connectivity with `get_server_status`.
- **Identity Mapping** — Convert usernames to UIDs or fetch Origin-specific identifiers using `get_origin_uid` and `get_name_to_uid`.

### How it works

1. Subscribe to this server
2. Enter your Apex Legends API Key
3. Start querying live game data from Claude, Cursor, or any MCP client

### Who is this for?

- **Competitive Players** — Track your progress and rank requirements without leaving your workspace.
- **Data Analysts** — Gather player and match data for performance reporting and meta analysis.
- **Community Managers** — Monitor server status and map rotations to keep players informed.


## Available Tools
- **get_leaderboard**: Updates every 6 hours.

Get top 500 players for specific statistics
- **manage_legacy_match_history**: Action can be info, get, add, or delete.

Manage legacy match history tracking
- **get_map_rotation**: Get current and next maps for various game modes
- **get_match_history**: Must make a /bridge request every 4 mins to collect data.

Get new match history for a player
- **get_name_to_uid**: Get a player UID from their name across multiple platforms
- **get_origin_uid**: Get a player UID from their name (PC only)
- **get_player_stats_by_name**: For PC, use Origin account name.

Get player statistics by name and platform
- **get_player_stats_by_uid**: Recommended for repeated queries.

Get player statistics by UID
- **get_predator_requirements**: Get RP/AP needed for Apex Predator rank
- **get_server_status**: Get current server status for Apex Legends


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Apex Legends** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is the current map rotation for Battle Royale?"

**🤖 AI Agent:**
> I'll check that for you. Currently, the map is 'World's Edge' with 45 minutes remaining. The next map in rotation will be 'Storm Point'.

---

**👤 You:**
> "Get the stats for player 'Genburten' on PC."

**🤖 AI Agent:**
> Fetching stats for Genburten... Found! They are currently at Apex Predator rank with 25,400 RP. Their most played legend recently is Horizon with 15,000+ kills tracked.

---

**👤 You:**
> "Show me the top 5 players on the global leaderboard for Wraith kills."

**🤖 AI Agent:**
> Accessing the leaderboard... The top 5 Wraith players globally are: 1. PlayerA (210k kills), 2. PlayerB (195k kills), 3. PlayerC (188k kills), 4. PlayerD (182k kills), 5. PlayerE (175k kills).


## ❓ FAQ

**Q: How can I check if the Apex Legends servers are currently down?**
You can use the `get_server_status` tool. It provides real-time connectivity data for various regions and platforms to confirm if there are any ongoing outages.

**Q: Is it possible to see how many points I need to reach Apex Predator rank?**
Yes! The `get_predator_requirements` tool returns the current RP/AP threshold required to enter the top 750 (Predator) rank on each platform.

**Q: Can I track my match history automatically?**
You can use `get_match_history` for recent data or `manage_legacy_match_history` to add your UID to the tracking system. Note that some tracking features require periodic bridge requests.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/apex-legends](https://vinkius.com/mcp/apex-legends)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Apex Legends** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `apex-legends` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Apex Legends** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "apex-legends": {
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
