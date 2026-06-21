# Chess.com Global Intelligence MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/chesscom-global-intelligence)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/chesscom-global-intelligence-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/chesscom-global-intelligence-mcp)
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


## Installation & Usage

To install and use the **Chess.com Global Intelligence** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/chesscom-global-intelligence](https://vinkius.com/mcp/chesscom-global-intelligence)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
