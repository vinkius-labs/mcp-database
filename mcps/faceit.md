# Faceit MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/faceit)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [data-analytics](../categories/data-analytics.md)

Access competitive gaming data — search players, matches, hubs, tournaments and leaderboards for CS2, Valorant and more.

## Description
Connect to **Faceit** and access the world's largest competitive gaming platform through natural conversation.

### What you can do

- **Player Search** — Find any player by nickname with Faceit level, ELO and game stats
- **Player Stats** — Get detailed CS2/Valorant stats including K/D, win rate, headshot %
- **Match Details** — View match results, scores and individual player performance
- **Hub Info** — Browse community hubs with matches, leaderboards and member info
- **Tournaments** — Search upcoming and ongoing tournaments by game and skill level
- **Games Catalog** — View all games supported on the Faceit platform

### How it works

1. Subscribe to this server
2. Enter your Faceit API Key (free registration at developers.faceit.com)
3. Start exploring competitive gaming data from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Competitive Gamers** — track player stats, check matchmaking results and browse tournaments
- **Team Managers** — analyze player performance, match history and hub leaderboards
- **Content Creators** — access player data, match results and tournament info for content


## Available Tools (12)
- **get_games**: Returns game IDs, names, icons and player counts.

Get all supported games on Faceit
- **get_hub**: Returns hub name, game, player count, rules, settings and organizer info.

Get details for a specific Faceit hub
- **get_hub_leaderboard**: Returns player rankings with nicknames, ELO, Faceit level and position.

Get the leaderboard for a specific hub
- **get_hub_matches**: Returns match IDs, teams, scores, status and timestamps. Filter by type: "all", "upcoming", "ongoing", "past".

Get matches for a specific hub
- **get_match**: Get details for a specific match
- **get_match_stats**: Returns K/D/A, headshot %, K/R ratio, MVP rounds and other per-player performance metrics.

Get player statistics for a specific match
- **get_player**: Returns nickname, avatar, country, Faceit levels for all games, ELO ratings, member_since and game player IDs (Steam, Riot, etc.).

Get detailed profile for a specific Faceit player
- **get_player_bans**: Returns ban type, reason, date and duration.

Get ban history for a player
- **get_player_history**: Returns match IDs, results (win/loss), score, ELO change, date and game. Use game filter to get history for a specific game.

Get match history for a player
- **get_player_stats**: Returns matches played, win rate, K/D ratio, ELO, headshot percentage (CS2), average kills/deaths and current win streak.

Get game-specific stats for a player
- **search_players**: Returns player IDs, nicknames, avatars, Faceit levels, ELO ratings and game stats. Useful for finding any player on the platform.

Search for Faceit players by nickname
- **search_tournaments**: Returns tournament names, IDs, games, skill level requirements, start times, prize pools and registration status.

Search for tournaments on Faceit


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Faceit** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Search for player s1mple on Faceit."

**🤖 AI Agent:**
> Found s1mple: Faceit Level 10, CS2 ELO 2847. Win rate: 68%, K/D: 1.42, Headshot %: 52%. Member since 2016.

---

**👤 You:**
> "Show me upcoming CS2 tournaments."

**🤖 AI Agent:**
> Found 5 upcoming CS2 tournaments: 1) 5v5 Daily Cup (Level 7+, starts 14:00 UTC, $100 prize) — 2) Weekend Warriors (Level 5+, Saturday 18:00, €250 prize) — 3) Pro League Qualifier (Level 8+, Sunday 16:00).

---

**👤 You:**
> "Get the leaderboard for hub abc123."

**🤖 AI Agent:**
> Hub Leaderboard: 1. PlayerOne (ELO 2156, Level 9) — 2. ProGamer42 (ELO 2089, Level 9) — 3. SharpShooter (ELO 2034, Level 8) — 4-10...


## ❓ FAQ

**Q: How do I get a Faceit API key?**
Register at [**developers.faceit.com**](https://developers.faceit.com/) and create an application to get your API key. Free for non-commercial use.

**Q: What games are supported?**
Faceit supports CS2, Valorant, Dota 2, League of Legends, Rainbow Six Siege, Rocket League, PUBG and many more. Use get_games to see the full catalog.

**Q: What is a Faceit level?**
Faceit levels range from 1-10 based on ELO rating. Level 1 = 0-500 ELO, Level 10 = 2001+ ELO. Higher levels indicate more skilled players.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/faceit](https://vinkius.com/mcp/faceit)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Faceit** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `faceit` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Faceit** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "faceit": {
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
