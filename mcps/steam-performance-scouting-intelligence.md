# Steam Performance & Scouting Intelligence MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/steam-performance-scouting-intelligence)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

The definitive server for professional Steam scouting — analyze player performance, achievements, and technical game stats via AI.

## Description
Transform your AI agent into a professional e-sports scout and performance analyst via **Steam Performance & Scouting Intelligence**. This server provides high-precision access to official game statistics and user achievements, allowing your agent to audit player skill levels, track technical milestones, and identify high-performance benchmarks across thousands of Steam titles. Whether you are a coach analyzing a pro-player's history or an analytical gamer monitoring your own progress, your agent acts as a dedicated technical scout through natural conversation.

### What you can do

- **Technical Scouting** — Retrieve granular in-game statistics including kills, technical objectives, and class-specific playtime
- **Achievement Auditing** — Track individual player achievements and compare them against global rarity percentages to quantify skill
- **Server Intelligence** — Fetch real-time status and metadata for dedicated game servers via IP address
- **Roster & Ban Monitoring** — Audit user levels, badges, and official ban statuses (VAC/Game) to ensure integrity in competitive environments

### How it works

1. Subscribe to this server
2. Enter your Steam Web API Key
3. Start managing your technical scouting intelligence from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **E-sports Coaches & Scouts** — instantly audit player profiles and technical histories for recruitment and tactical analysis
- **Competitive Gamers** — monitor your performance trends and achievement rarities to optimize your gameplay
- **Tournament Organizers** — automate integrity checks including VAC bans and server availability directly from your workflow


## Available Tools
- **get_player_badges**: List all community badges earned by a player
- **get_friend_list**: Requires the user profile to be public.

Get the friend list of a Steam user
- **get_game_schema**: Get the full stats and achievements schema for a game
- **get_global_achievement_percentages**: Get global unlock percentages for all achievements in a game
- **get_owned_games**: List all games owned by a player with playtime
- **get_player_achievements**: Get achievement unlock status for a user in a game
- **get_player_bans**: Check VAC, community, and economy ban status
- **get_player_profile**: Get Steam profile info for one or more players
- **get_recently_played_games**: List games played in the last 2 weeks
- **get_steam_level**: Get the Steam level of a player
- **get_user_game_stats**: ) tracked by Steam for a user in a given game.

Get raw gameplay stats for a user in a specific game


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Steam Performance & Scouting Intelligence** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Audit the technical performance of player '7656119803...' in Deadlock."

**🤖 AI Agent:**
> Retrieving technical scouts... I've fetched the stats for Deadlock. This player has an average soul-per-minute of 450 and a 65% winrate with 'Hero X'. I also have the breakdown of their damage contribution. Would you like to see their last 5 match outcomes?

---

**👤 You:**
> "Check for active VAC bans on SteamID '7656119803...'."

**🤖 AI Agent:**
> Running integrity check... The account '7656119803...' is currently in good standing. No active VAC, community, or trade bans were detected. I have the full ban history report. Shall I also check their account level and badges?

---

**👤 You:**
> "Compare the achievement rarity for 'Elden Ring' between my account and global stats."

**🤖 AI Agent:**
> Inspecting achievements... You have unlocked 'Achievement A', which only 2.5% of players globally possess. However, you are missing 'Achievement B', which 15% have already completed. Would you like the full technical list of missing achievements?


## ❓ FAQ

**Q: Can my AI automatically analyze technical stats for a specific game like Deadlock?**
Yes! By using tools like `get_user_game_stats` and `get_game_schema`, your agent can retrieve the full list of technical counters (souls, damage, objectives) recorded by the Steam backend for that specific title.

**Q: How do I check if a player has any active bans before inviting them to a tournament?**
Use the `get_player_bans` tool. Your agent will instantly retrieve the official status for VAC bans, community bans, and economy bans, ensuring the integrity of your competitive event.

**Q: Does the integration allow comparing performance between two different players?**
Yes. The `get_user_game_stats` action retrieves data for multiple SteamIDs and compiles a side-by-side comparison of their technical metrics, allowing the agent to identify who has higher efficiency in specific areas.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/steam-performance-scouting-intelligence](https://vinkius.com/mcp/steam-performance-scouting-intelligence)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Steam Performance & Scouting Intelligence** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `steam-performance-scouting-intelligence` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Steam Performance & Scouting Intelligence** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "steam-performance-scouting-intelligence": {
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
