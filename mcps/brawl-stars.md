# Brawl Stars MCP Server

Access real-time Brawl Stars data — track player stats, battle logs, club rankings, and event rotations directly from your AI agent.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/brawl-stars)

## Overview
**Category:** data-analytics
**Tools Count:** 10

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


## Installation & Usage

To install and use the **Brawl Stars** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/brawl-stars](https://vinkius.com/mcp/brawl-stars)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
