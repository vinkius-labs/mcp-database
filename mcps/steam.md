# Steam MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/steam)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [industry-titans](../categories/industry-titans.md)

Access Steam gaming data — player profiles, owned games, achievements, and stats via AI.

## Description
Connect the **Steam Web API** to any AI agent and retrieve gaming data including player profiles, game libraries, achievements, and statistics through natural language.

### What you can do

- **Player Profiles** — Retrieve public profile information including avatars, status, and account creation date
- **Game Library** — List all games owned by a user with playtime statistics
- **Recent Activity** — Check games played in the last 2 weeks with detailed session times
- **Achievement Tracking** — View achievement unlock status and timestamps for any game
- **Player Statistics** — Access in-game stats and performance metrics for specific titles
- **Steam Level & Badges** — Check user level, equipped badges, and community progress
- **App News** — Retrieve recent news articles and updates for any Steam app

### How it works

1. Subscribe to this server
2. Enter your Steam Web API Key
3. Start querying Steam data from Claude, Cursor, or any MCP-compatible client


## Available Tools (10)
- **get_app_list**: Get complete list of Steam apps
- **get_badge_progress**: Get community badge progress for a user
- **get_app_news**: Get news articles for a Steam app
- **get_owned_games**: Get list of games owned by a Steam user
- **get_player_achievements**: Get achievement progress for a player in a specific game
- **get_player_badges**: Get badges equipped by a Steam user
- **get_player_summaries**: Get profile information for Steam users
- **get_recently_played_games**: Get games recently played by a Steam user
- **get_steam_level**: Get the Steam level of a user
- **get_user_stats_for_game**: Get user's statistics for a specific game


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Steam** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Show me the profile of Steam user 76561197960287930."

**🤖 AI Agent:**
> Player 'Robin' is currently online. Account created in 2003, currently at Steam Level 80. Profile is public with avatar and location visible.

---

**👤 You:**
> "What games does user 76561197960287930 own and how much have they played?"

**🤖 AI Agent:**
> This user owns 347 games. Top played: Counter-Strike 2 (257 hours), Dota 2 (833 hours), Team Fortress 2 (142 hours). Would you like details on any specific game?

---

**👤 You:**
> "Get recent news updates for Cyberpunk 2077 (App ID 1091500)."

**🤖 AI Agent:**
> Found 3 recent news articles for Cyberpunk 2077. Latest: 'Update 2.1 — Now Available' released yesterday with new features and bug fixes.


## ❓ FAQ

**Q: How do I get a Steam Web API Key?**
Visit [**Steam Web API Key page**](https://steamcommunity.com/dev/apikey) while logged into your Steam account, agree to the terms, and you'll receive a unique key.

**Q: Can I check someone's game achievements?**
Yes! Use `get_player_achievements` with the user's Steam ID and the game's App ID. The user's profile and achievements must be public.

**Q: Is playtime data available for all games?**
Yes. The `get_owned_games` endpoint returns `playtime_forever` in minutes for each game. Recent playtime (2 weeks) is available via `get_recently_played_games`.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/steam](https://vinkius.com/mcp/steam)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Steam** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `steam` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Steam** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "steam": {
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
