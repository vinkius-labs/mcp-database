# Cartola FC (Fantasy Football) MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/cartola-fc-fantasy-football)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/cartola-fc-fantasy-football-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/cartola-fc-fantasy-football-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [data](../categories/data.md)

The definitive server for Cartola FC — track scouts, player values, and live scores for Brasileirão Série A.

## Description
Transform your AI agent into a professional Cartola FC strategist with this dedicated server. Designed for the highly competitive Brazilian fantasy game, this integration provides deep access to the Globo database, allowing your agent to audit player scouts, track market status, and retrieve live scoring updates for the Brasileirão Série A. Whether you are hunting for high-value bargains or monitoring the most selected players of the round, your agent acts as a dedicated fantasy scout through natural conversation.

### What you can do

- **Market Auditing** — Check live market status, round deadlines, and official game news in real-time
- **Scout Analysis** — Retrieve granular performance data including tackles, passes, and goal involvements for any athlete
- **Selection Intelligence** — List the most popular players of the round and track 'Probable' lineups to avoid zero-pointers
- **League & Team Tracking** — Search for public/private leagues and audit individual user team lineups and historical performance

### How it works

1. Subscribe to this server
2. No API key required for public market access
3. Start managing your Cartola strategy from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Fantasy Strategists** — perform deep statistical audits to optimize your team's value and points yield
- **Data Journalists** — instantly retrieve round highlights and top performing players for technical reporting
- **Community Managers** — automate the retrieval of league rankings and highlights for your fantasy group


## Available Tools
- **list_top_average_players**: List players with the highest season averages
- **list_cheap_players**: List players with low prices (Bargains)
- **list_players_by_club**: List all players from a specific club
- **list_clubs**: List all club names and IDs
- **search_leagues**: Search for public or private leagues by name
- **list_round_scorers**: Get real-time scores for the current round
- **list_players_by_position**: List players by position (GK, DEF, MID, FWD)
- **list_probable_players**: List players with "Probable" status
- **search_players**: Search for players by nickname
- **get_market_status**: Check if the Cartola FC market is open
- **get_user_team_by_slug**: Retrieve details for a specific user team by slug
- **list_top_scaled_players**: List the most selected players for the current round


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Cartola FC (Fantasy Football)** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all 'Probable' players from Flamengo for this round."

**🤖 AI Agent:**
> I've filtered the market data for Flamengo (ID: 262). I found 8 players currently marked as 'Probable', including Hulk and Arrascaeta. Would you like to see their prices and season averages?

---

**👤 You:**
> "Who are the top 5 most selected players in Cartola FC right now?"

**🤖 AI Agent:**
> Running the highlights query... The most selected player is 'Player X' with over 1.2 million selections. I have the full top 5 list with their club details. Shall I provide the summary?

---

**👤 You:**
> "Find all defenders priced below 10 cartoletas with an average above 4.0."

**🤖 AI Agent:**
> Inspecting the market... I found 4 defenders matching your criteria, including 'Defender Y' (Price: 8.5, Avg: 4.8). Would you like to see their specific scouts for the last match?


## Installation & Usage

To install and use the **Cartola FC (Fantasy Football)** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/cartola-fc-fantasy-football](https://vinkius.com/mcp/cartola-fc-fantasy-football)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
