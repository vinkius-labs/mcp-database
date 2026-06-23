# BattleMetrics MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/battlemetrics)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [data-analytics](../categories/data-analytics.md)

Global game server tracking and player analytics — monitor servers, search players, and audit bans via AI.

## Description
Empower your AI agent to operate as a real-time intelligence layer over the global gaming server ecosystem with **BattleMetrics**, the industry-standard platform for game server monitoring. By connecting BattleMetrics to your agent, you transform complex server population analytics, player lookups, and ban auditing into natural conversation. Your agent can instantly search across thousands of tracked game servers, identify specific players, analyze population trends, and review ban records without navigating dashboards.

### What you can do

- **Server Discovery** — Search and filter game servers by name, game, or country. View live player counts, rank, IP address, and detailed metadata.
- **Player Lookups** — Search the global player database by name and retrieve full profiles including identifiers, playtime stats, and linked servers.
- **Session Tracking** — View a player's complete session history showing which servers they played on, join/leave times, and duration.
- **Population Analytics** — Retrieve historical player count data for any server to analyze peak hours, activity trends, and growth patterns.
- **Ban Auditing** — List and review bans from your organization, filter by server, and inspect ban reasons, scope, and expiry.
- **Leaderboards** — Access time-based leaderboards for any server to identify the most active players.
- **Game Catalog** — Browse all games tracked by BattleMetrics and get detailed ecosystem statistics.

### How it works

1. Subscribe to this server
2. Enter your BattleMetrics Personal Access Token
3. Start querying game servers, players, and bans through Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Game Server Administrators** — monitor server populations, audit player behavior, and manage bans directly through AI.
- **Community Managers** — track player activity, identify regulars, and review session history for moderation purposes.
- **Esports Analysts** — analyze server population trends, player engagement patterns, and competitive server rankings.
- **Game Developers** — monitor live server health, player retention, and community activity across multiple titles.


## Available Tools (12)
- **get_ban**: Returns the ban reason, banned player identifier, timestamps, expiry date, scope (server-level or organization-wide), and the administrator who issued the ban. Requires appropriate ban:read scope on the API token. Use this after identifying a ban ID from list_bans.

Get details for a specific ban
- **get_game**: Returns details such as the game name, the number of tracked servers and players, and game-specific metadata. Use this to get an overview of a game's ecosystem on BattleMetrics.

Get details about a specific tracked game
- **get_player**: Returns the player name, associated identifiers (Steam, EOS, etc.), time played statistics, linked servers, and recent activity. Use this after identifying a player ID from list_players or session history.

Get detailed profile for a specific player
- **get_server**: Returns the server name, IP address, port, current player count, max players, rank, game details, map, status, and detailed metadata. Use this when the user already has a server ID and wants deep information.

Get detailed information about a specific game server
- **get_server_leaderboard**: Returns player names, IDs, and playtime duration. This is useful for identifying the most active or dedicated players on any tracked game server. Use page_number for pagination.

Get the time-based leaderboard for a game server
- **list_bans**: Each ban includes the ban reason, the banned player identifier, timestamps, expiry, and scope (server-level or organization-wide). Requires appropriate ban:read scope on the API token. Use page_number for pagination and optional server_id to filter bans from a specific server.

List bans in your BattleMetrics organization
- **list_games**: Returns each game's ID, display name, and metadata. Useful for discovering which games are available for server and player queries, and for getting the correct game identifier to use in server filters.

List all games tracked by BattleMetrics
- **list_players**: Use the search parameter to find players by name. Returns player names, IDs, and metadata. Results are paginated — use page_number to navigate. This is a powerful tool for looking up any player across all supported games.

Search and list players across all tracked game servers
- **list_servers**: Use the optional search parameter to find servers by name, or filter by game and country. Returns server name, IP, port, player count, rank, and game type. Results are paginated — use page_number to navigate through results.

List game servers tracked by BattleMetrics
- **get_player_sessions**: Each session shows which server the player was on, when they joined, when they left, and the session duration. Useful for auditing player activity, tracking playtime, or verifying presence on a specific server.

Get session history for a specific player
- **search_servers**: Unlike the basic list_servers tool, this supports granular filtering by server name, game, country, minimum/maximum player count, rank range, and more. Returns matching servers with full metadata including name, IP, port, player count, rank, game type, map, and status. Use this when you need precise filtering to find specific servers. Results are paginated — use page_number to navigate.

Search game servers with advanced filters
- **get_server_player_count_history**: Useful for analyzing population trends, peak hours, and server activity patterns over a given time range. If start and stop are omitted, the API returns recent history. Use ISO 8601 timestamps for the date range.

Get player count history for a game server over time


## 💬 Prompt Examples

Here are some examples of how you can interact with the **BattleMetrics** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Show me the most popular Rust servers in the US right now."

**🤖 AI Agent:**
> I've retrieved the top Rust servers in the US. Here are the most populated ones with their player counts, ranks, and connection details.

---

**👤 You:**
> "Look up the player 'shroud' and show me their recent session history."

**🤖 AI Agent:**
> I found the player 'shroud'. Their recent sessions show activity on 3 different servers in the past week, with a total of 42 hours played. Here are the full session details.

---

**👤 You:**
> "Show me the player count trend for server ID 12345 over the last 7 days."

**🤖 AI Agent:**
> I've pulled the player count history for server 12345. The data shows peak activity at 18:00-22:00 UTC with an average of 87 players, dropping to around 15 during off-peak hours.


## ❓ FAQ

**Q: How do I find a specific game server?**
Use the `list_servers` tool with the search parameter. You can filter by server name, game type (e.g. rust, ark), or country code (e.g. US, DE). The results include server name, IP, player count, and rank. For more advanced filtering (min/max players), use the `search_servers` tool.

**Q: Can I track a player's activity across different servers?**
Yes. Use `list_players` to find the player by name, then `get_player` to view their full profile, and `get_player_sessions` to see their complete session history including which servers they joined, when they connected and disconnected, and for how long.

**Q: What games does BattleMetrics support?**
BattleMetrics tracks hundreds of multiplayer games including Rust, ARK, Minecraft, CS2, Valheim, DayZ, and many more. Use the `list_games` tool to get the complete, up-to-date catalog of all supported games with their identifiers.

**Q: How do I get details about a specific ban?**
First use `list_bans` to find the ban and get its numeric ban ID. Then use `get_ban` with that ID to retrieve the complete ban record including the reason, player identifier, expiry date, scope, and issuing administrator.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/battlemetrics](https://vinkius.com/mcp/battlemetrics)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **BattleMetrics** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `battlemetrics` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **BattleMetrics** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "battlemetrics": {
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
