# Brawl Stars MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/brawl-stars)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/brawl-stars-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/brawl-stars-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [data-analytics](../categories/data-analytics.md)

Access real-time Brawl Stars data — track player stats, battle logs, club rankings, and event rotations directly from your AI agent.

## Description
Connect your **Brawl Stars** API key to any AI agent and dive deep into game analytics through natural conversation.

### What you can do

- **Player Profiles** — Fetch detailed stats, trophy counts, and brawler levels for any player tag using `get_player`.
- **Battle Logs** — Analyze the last 25 matches via `get_player_battlelog` to understand performance and meta trends.
- **Club Insights** — Inspect club details and member lists with `get_club` and `get_club_members` to manage your community.
- **Global Rankings** — Query leaderboards for players, clubs, and specific brawlers globally or by country using `get_player_rankings` and `get_brawler_rankings`.
- **Game Meta** — List all available brawlers with `list_brawlers` and check the current event rotation for active maps using `get_event_rotation`.

### How it works

1. Subscribe to this server
2. Enter your Brawl Stars API Key
3. Start querying game data from Claude, Cursor, or any MCP-compatible client

No more manual searching for player tags or checking the app for map rotations. Your AI acts as your personal game analyst and scout.


## Available Tools
- **get_brawler_rankings**: Get brawler-specific rankings
- **get_brawler**: Get information about a specific brawler
- **list_brawlers**: List all available brawlers
- **get_club_members**: Get a list of club members
- **get_club_rankings**: Get club rankings for a country or globally
- **get_club**: Get club details
- **get_event_rotation**: Get the current event rotation
- **get_player_battlelog**: Get the last 25 battles for a player
- **get_player_rankings**: Get player rankings for a country or globally
- **get_player**: Get player profile and statistics


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Brawl Stars** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Get the profile and stats for player tag #2P0GV9LU."

**🤖 AI Agent:**
> I've retrieved the profile for player #2P0GV9LU. They currently have 32,450 trophies, belong to the club 'Brawl Stars Pro', and their highest trophies ever reached was 34,000. Would you like to see their most played brawlers?

---

**👤 You:**
> "Show me the current global club rankings."

**🤖 AI Agent:**
> Fetching global club rankings... The top 3 clubs currently are: 1. 'Nova Esports' (2.5M trophies), 2. 'Tribe Gaming' (2.4M trophies), and 3. 'SK Gaming' (2.35M trophies). Would you like to see the member list for any of these?

---

**👤 You:**
> "What are the active maps and events right now?"

**🤖 AI Agent:**
> Checking event rotation... Currently active: Gem Grab on 'Hard Rock Mine', Solo Showdown on 'Feast or Famine', and Brawl Ball on 'Pinhole Punt'. New events will rotate in 4 hours. Should I check the upcoming maps as well?


## Installation & Usage

To install and use the **Brawl Stars** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/brawl-stars](https://vinkius.com/mcp/brawl-stars)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
