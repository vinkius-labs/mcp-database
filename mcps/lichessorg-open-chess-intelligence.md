# Lichess.org Open Chess Intelligence MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/lichessorg-open-chess-intelligence)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/lichessorg-open-chess-intelligence-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/lichessorg-open-chess-intelligence-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [artificial-intelligence](../categories/artificial-intelligence.md)

The definitive server for Lichess.org — monitor live broadcasts, analyze player stats, and solve puzzles via AI.

## Description
Equip your AI agent with the most transparent and real-time chess intelligence via **Lichess.org Open Chess Intelligence**. This high-performance server provides deep access to the world's leading open-source chess platform, allowing your agent to instantly retrieve real-time player metadata, monitor official tournament broadcasts with technical move lists, and identify elite players currently live on Lichess TV. Whether you are performing technical scouting, auditing recent player activity, or following a major global championship broadcast, your agent acts as a dedicated chess data engineer and analyst through natural conversation.

### What you can do

- **Real-time Monitoring** — Follow live matches on Lichess TV or official tournament broadcasts with sub-second technical updates
- **Comprehensive Auditing** — Retrieve detailed player profiles, ratings for all variants, and chronological activity logs
- **Match Intelligence** — Fetch complete post-game statistics and PGN data for recent matches to analyze tactical patterns
- **Community Insights** — Search for team memberships and monitor live streamers to understand the global social chess graph

### How it works

1. Subscribe to this server
2. (Optional) Enter your Lichess Personal Access Token for higher rate limits
3. Start managing your chess intelligence from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Technical Analysts** — perform deep audits of match history and PGN data for professional-grade reporting
- **Chess Students** — solve daily puzzles and analyze broadcasted master games to improve tactical skills
- **Tournament Organizers** — monitor player status and ongoing transmissions to orchestrate e-sports events


## Available Tools
- **get_daily_puzzle**: Get the Lichess puzzle of the day
- **get_leaderboards**: Get top player rankings for all variants
- **get_player_data**: Get public data for a Lichess player
- **get_tv_channels**: ).

See who is playing live on Lichess TV
- **get_team_members**: List members of a Lichess team
- **get_user_activity**: Get recent activity log for a player
- **get_user_games**: Get match history for a player
- **get_users_online_status**: Check if multiple users are online
- **list_broadcasts**: List ongoing official tournament broadcasts
- **list_live_streamers**: List chess streamers currently live


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Lichess.org Open Chess Intelligence** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Check which Grandmasters are currently playing live on Lichess TV."

**🤖 AI Agent:**
> Retrieving Lichess TV channels... I've identified that GM Magnus Carlsen is currently live in the Blitz channel, and GM Hikaru Nakamura is playing in the Bullet channel. Would you like to see the real-time board status for either match?

---

**👤 You:**
> "Retrieve the last 5 games for player 'UserX' and provide the PGN links."

**🤖 AI Agent:**
> Inspecting match history for UserX... I've retrieved 5 recent matches, including a victory against an IM. I have the technical results and the direct PGN download links for each. Shall I perform a move-by-move analysis for any of them?

---

**👤 You:**
> "Analyze the ongoing official broadcast for the 'Candidates Tournament 2024'."

**🤖 AI Agent:**
> Accessing official broadcast feed... The Candidates Tournament is currently live. I've identified 4 active boards. On Board 1, Nepomniachtchi has a slight technical advantage (+0.8) according to Stockfish analysis. Would you like the full move sequence for this game?


## Installation & Usage

To install and use the **Lichess.org Open Chess Intelligence** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/lichessorg-open-chess-intelligence](https://vinkius.com/mcp/lichessorg-open-chess-intelligence)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
