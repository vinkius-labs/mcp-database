# Apex Legends MCP Server

Track Apex Legends player stats, match history, leaderboards, and server status directly from your AI agent.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/apex-legends)

## Overview
**Category:** data-analytics
**Tools Count:** 10

## Description
Connect your AI agent to the **Apex Legends API** to access real-time game data, player performance metrics, and server health. This server provides a comprehensive suite of tools for competitive analysis and game tracking.

### What you can do

- **Player Statistics** — Retrieve detailed combat metrics, rank data, and legend-specific trackers using `get_player_stats_by_name` or `get_player_stats_by_uid`.
- **Match History** — Access recent match results and manage legacy tracking via `get_match_history` and `manage_legacy_match_history`.
- **Competitive Insights** — Check the current global leaderboards with `get_leaderboard` and see the RP/AP needed for Apex Predator rank with `get_predator_requirements`.
- **Live Game Data** — Stay updated with `get_map_rotation` for current and upcoming maps, and monitor connectivity with `get_server_status`.
- **Identity Mapping** — Convert usernames to UIDs or fetch Origin-specific identifiers using `get_origin_uid` and `get_name_to_uid`.

### How it works

1. Subscribe to this server
2. Enter your Apex Legends API Key
3. Start querying live game data from Claude, Cursor, or any MCP client

### Who is this for?

- **Competitive Players** — Track your progress and rank requirements without leaving your workspace.
- **Data Analysts** — Gather player and match data for performance reporting and meta analysis.
- **Community Managers** — Monitor server status and map rotations to keep players informed.


## Available Tools
- **get_leaderboard**: Updates every 6 hours.

Get top 500 players for specific statistics
- **manage_legacy_match_history**: Action can be info, get, add, or delete.

Manage legacy match history tracking
- **get_map_rotation**: Get current and next maps for various game modes
- **get_match_history**: Must make a /bridge request every 4 mins to collect data.

Get new match history for a player
- **get_name_to_uid**: Get a player UID from their name across multiple platforms
- **get_origin_uid**: Get a player UID from their name (PC only)
- **get_player_stats_by_name**: For PC, use Origin account name.

Get player statistics by name and platform
- **get_player_stats_by_uid**: Recommended for repeated queries.

Get player statistics by UID
- **get_predator_requirements**: Get RP/AP needed for Apex Predator rank
- **get_server_status**: Get current server status for Apex Legends


## Installation & Usage

To install and use the **Apex Legends** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/apex-legends](https://vinkius.com/mcp/apex-legends)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
