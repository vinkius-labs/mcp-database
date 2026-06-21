# Chess.com Global Intelligence MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/chesscom-global-intelligence)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [education](../categories/education.md)

The definitive server for Chess.com — track player ratings, historical games, and daily puzzles via AI.

## Description
Equip your AI agent with deep intelligence from the world's leading chess platform via **Chess.com Global Intelligence**. This high-performance server provides unprecedented access to the official Chess.com database, allowing your agent to instantly retrieve real-time player ratings (Blitz, Bullet, Rapid), audit comprehensive match histories (PGN), and identify top players globally across all titled ranks (GM, IM, FM). Whether you are analyzing a grandmaster's recent performance, solving the daily featured tactic, or researching club metadata, your agent acts as a professional chess analyst through natural conversation.

### What you can do

- **Player Auditing** — Retrieve precise ELO ratings, win/loss statistics, and public profile metadata for any account
- **Game Research** — Access complete monthly archives of historical games for technical analysis and opening research
- **Tactical Intelligence** — Fetch the official daily chess puzzle or retrieve random tactics for training and improvement
- **Global Rankings** — List and query leaderboards for all major formats and identify titled players by region or rank

### How it works

1. Subscribe to this server
2. No API key required for public discovery access
3. Start managing your chess intelligence from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Chess Analysts & Coaches** — instantly retrieve player histories and ratings for technical reporting and scouting
- **Competitive Players** — monitor your own progress, analyze opponents, and stay updated on global leaderboards
- **Content Creators** — retrieve high-integrity match data and daily puzzles for reporting and community engagement


## Available Tools
- **get_player_stats**: Get ratings and statistics for a player
- **list_active_streamers**: List active Chess.com streamers
- **list_titled_players**: List players with a specific title (GM, IM, etc)
- **get_tournament_metadata**: Get details for a specific tournament
- **get_player_game_archives**: List available monthly game archives for a player
- **get_chess_club_details**: Get metadata for a specific chess club
- **get_country_details_chess**: com identifier using a 2-letter ISO code.

Get details for a specific country by ISO code
- **get_global_leaderboards**: com.

Get current top player rankings
- **get_player_monthly_games**: Get games played by a user in a specific month
- **get_player_profile**: Get basic information about a Chess.com player
- **get_daily_chess_puzzle**: com.

Get the official daily chess puzzle
- **get_random_chess_puzzle**: com database for tactical training.

Get a random chess tactic/puzzle


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Chess.com Global Intelligence** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Analyze the current ratings and winrate for 'MagnusCarlsen'."

**🤖 AI Agent:**
> Inspecting Grandmaster stats... Magnus Carlsen is currently rated 2890 in Blitz and 2810 in Rapid. He has a dominant winrate across all formats. Would you like to see his best historical rating or his last 5 match results?

---

**👤 You:**
> "Show me today's daily chess puzzle and its title."

**🤖 AI Agent:**
> Retrieving the daily tactic... Today's puzzle is titled 'Deflection in the Endgame'. I have the official URL and the board image preview for you. Shall I check for a random training puzzle as well?

---

**👤 You:**
> "List the top 5 players in the global Blitz leaderboard."

**🤖 AI Agent:**
> Running leaderboard query... The top 5 Blitz players are currently MagnusCarlsen, Hikaru, Firouzja2003, NihalSarin, and DanielNaroditsky. All hold the GM title. Would you like to see the Rapid or Bullet rankings?


## ❓ FAQ

**Q: Can my AI automatically find the current ratings for a specific Grandmaster like Magnus Carlsen?**
Yes! Use the `get_player_stats` tool with the username. Your agent will respond with the current and best ratings for Blitz, Bullet, and Rapid formats, along with their recent win/loss record.

**Q: Is it possible to retrieve all games played by a user in a specific month for technical analysis?**
Absolutely. First use `get_player_game_archives` to see available periods, then run `get_player_monthly_games` for the target year and month. It will return the complete PGN data for all matches in that window.

**Q: Does the integration permit listing all active Grandmasters (GMs) on the platform?**
Yes. The `list_titled_players` action allows your agent to fetch the complete list of usernames for any official title, including GM, WGM, IM, and FM, directly from the platform.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/chesscom-global-intelligence](https://vinkius.com/mcp/chesscom-global-intelligence)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Chess.com Global Intelligence** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `chesscom-global-intelligence` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Chess.com Global Intelligence** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "chesscom-global-intelligence": {
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
