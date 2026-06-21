# Faceit MCP Server

Access competitive gaming data — search players, matches, hubs, tournaments and leaderboards for CS2, Valorant and more.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/faceit)

## Overview
**Category:** data-analytics
**Tools Count:** 12

## Description
Connect to **Faceit** and access the world's largest competitive gaming platform through natural conversation.

### What you can do

- **Player Search** — Find any player by nickname with Faceit level, ELO and game stats
- **Player Stats** — Get detailed CS2/Valorant stats including K/D, win rate, headshot %
- **Match Details** — View match results, scores and individual player performance
- **Hub Info** — Browse community hubs with matches, leaderboards and member info
- **Tournaments** — Search upcoming and ongoing tournaments by game and skill level
- **Games Catalog** — View all games supported on the Faceit platform

### How it works

1. Subscribe to this server
2. Enter your Faceit API Key (free registration at developers.faceit.com)
3. Start exploring competitive gaming data from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Competitive Gamers** — track player stats, check matchmaking results and browse tournaments
- **Team Managers** — analyze player performance, match history and hub leaderboards
- **Content Creators** — access player data, match results and tournament info for content


## Available Tools
- **get_games**: Returns game IDs, names, icons and player counts.

Get all supported games on Faceit
- **get_hub**: Returns hub name, game, player count, rules, settings and organizer info.

Get details for a specific Faceit hub
- **get_hub_leaderboard**: Returns player rankings with nicknames, ELO, Faceit level and position.

Get the leaderboard for a specific hub
- **get_hub_matches**: Returns match IDs, teams, scores, status and timestamps. Filter by type: "all", "upcoming", "ongoing", "past".

Get matches for a specific hub
- **get_match**: Get details for a specific match
- **get_match_stats**: Returns K/D/A, headshot %, K/R ratio, MVP rounds and other per-player performance metrics.

Get player statistics for a specific match
- **get_player**: Returns nickname, avatar, country, Faceit levels for all games, ELO ratings, member_since and game player IDs (Steam, Riot, etc.).

Get detailed profile for a specific Faceit player
- **get_player_bans**: Returns ban type, reason, date and duration.

Get ban history for a player
- **get_player_history**: Returns match IDs, results (win/loss), score, ELO change, date and game. Use game filter to get history for a specific game.

Get match history for a player
- **get_player_stats**: Returns matches played, win rate, K/D ratio, ELO, headshot percentage (CS2), average kills/deaths and current win streak.

Get game-specific stats for a player
- **search_players**: Returns player IDs, nicknames, avatars, Faceit levels, ELO ratings and game stats. Useful for finding any player on the platform.

Search for Faceit players by nickname
- **search_tournaments**: Returns tournament names, IDs, games, skill level requirements, start times, prize pools and registration status.

Search for tournaments on Faceit


## Installation & Usage

To install and use the **Faceit** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/faceit](https://vinkius.com/mcp/faceit)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
