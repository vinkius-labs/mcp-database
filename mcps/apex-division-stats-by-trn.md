# Apex & Division Stats by TRN MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/apex-division-stats-by-trn)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [data-analytics](../categories/data-analytics.md)

Deep gaming analytics — player profiles, per-legend breakdowns, match history, and global leaderboards for Apex Legends and Division 2 via AI.

## Description
Transform your AI agent into a professional esports analyst with **Apex & Division Stats by TRN**, powered by the official Tracker Network API. This server gives your agent real-time access to the TRN database — the same data powering tracker.gg, trusted by millions of competitive gamers worldwide.

### What you can do

- **Player Profiling** — Retrieve lifetime stats (K/D, kills, wins, damage, headshots, rank tier) for any Apex Legends or Division 2 player across Origin, PSN, and Xbox
- **Legend Breakdown** — Analyze per-legend performance to identify a player's main, playstyle, and strongest picks
- **Match History** — Review recent play sessions with aggregated stats to track performance trends over time
- **Global Leaderboards** — Access world rankings by stat category (Kills, RankScore, Damage, Level) to benchmark players against the global elite
- **PvP Intelligence** — Deep-dive into Division 2 Dark Zone and Conflict stats including rogue kills, extractions, and DZ rank
- **Cross-Game Search** — Find any player across the entire TRN ecosystem by username

### How it works

1. Subscribe to this server
2. Enter your TRN API Key from the [**Tracker Network Developer Portal**](https://tracker.gg/developers)
3. Start analyzing player performance from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Esports Scouts & Teams** — perform data-driven player evaluations across platforms for recruitment and roster decisions
- **Competitive Gamers** — track your own improvement with per-legend stats, session trends, and leaderboard positioning
- **Content Creators & Streamers** — pull real-time stats during broadcasts or for video research
- **Data Journalists** — access high-integrity gaming data for articles, rankings, and competitive analysis
- **Coaches & Analysts** — identify strengths, weaknesses, and meta trends from granular player data


## Available Tools
- **get_apex_leaderboard**: ) on the specified platform.

Get global Apex Legends rankings by stat category
- **get_apex_legend_breakdown**: ) — kills, damage, wins per legend. Essential for identifying main legend and playstyle.

Get per-legend performance breakdown for an Apex player
- **get_apex_match_history**: Useful for tracking recent performance trends.

Get recent match sessions for an Apex player
- **get_apex_game_metadata**: Useful as reference data.

Get current Apex Legends game metadata
- **get_apex_player_profile**: Get comprehensive Apex Legends stats for a player
- **get_division2_player_profile**: Get comprehensive stats for a Division 2 agent
- **get_division2_pvp_stats**: Get PvP-specific stats for a Division 2 agent
- **get_division2_match_history**: Get recent play sessions for a Division 2 agent
- **search_player**: Returns matching accounts with platform links and game associations.

Search for a player across the Tracker Network ecosystem


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Apex & Division Stats by TRN** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Show me the full Apex Legends stats for 'ImperialHal' on Origin."

**🤖 AI Agent:**
> ImperialHal is currently at Predator rank with over 52,000 lifetime kills, a 4.8 K/D ratio, and 2,100 wins. His top legends are Wraith and Horizon. Would you like to see the per-legend breakdown or his recent match history?

---

**👤 You:**
> "Compare the legend stats of two players: 'Player1' and 'Player2' on PSN."

**🤖 AI Agent:**
> I've pulled the per-legend breakdowns for both players. Player1 mains Octane with 8,200 kills and 45% headshot rate, while Player2 focuses on Lifeline with superior win rates. Player1 has 15% more total damage but Player2 has a higher K/D across all legends.

---

**👤 You:**
> "Who are the top 5 Apex players worldwide by RankScore on PC?"

**🤖 AI Agent:**
> Here's the current global leaderboard for RankScore on Origin:
1. Player_A — 48,200 RP
2. Player_B — 47,800 RP
3. Player_C — 47,100 RP
4. Player_D — 46,500 RP
5. Player_E — 46,200 RP
Would you like detailed profiles for any of these players?


## ❓ FAQ

**Q: Which games are supported?**
The official TRN public API supports **Apex Legends** and **The Division 2**. For Apex: full profile stats, per-legend breakdowns, match history, and global leaderboards. For Division 2: PvE/PvP stats, Dark Zone details, and session history.

**Q: Can I see per-legend stats like kills on Wraith or damage on Octane?**
Yes! Use `get_apex_legend_breakdown` to get performance data for each individual legend — kills, damage, wins, and more. This is perfect for identifying a player's main and comparing legend-specific performance.

**Q: How do I track a player's recent performance over time?**
Use `get_apex_match_history` or `get_division2_match_history` to retrieve grouped play sessions with aggregated stats. Each session shows kills, damage, placements, and XP — making it easy to spot improvement trends or slumps.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/apex-division-stats-by-trn](https://vinkius.com/mcp/apex-division-stats-by-trn)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Apex & Division Stats by TRN** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `apex-division-stats-by-trn` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Apex & Division Stats by TRN** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "apex-division-stats-by-trn": {
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
