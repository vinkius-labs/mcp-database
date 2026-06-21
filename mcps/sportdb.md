# SportDB MCP Server

Access live scores, standings, fixtures, and player data across football, basketball, hockey, and tennis from any AI agent.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/sportdb)

## Overview
**Category:** data-analytics
**Tools Count:** 18

## Description
Turn your AI agent into a dedicated sports analyst with **SportDB**. Query real-time match data, historical league tables, and deep player intelligence across multiple sports — all through natural conversation.

### What you can do

- **Live Match Tracking** — Retrieve real-time scores for football, basketball, hockey, and tennis as they happen
- **League Standings** — Fetch full league tables with points, wins, draws, losses, and goal difference for any season
- **Fixture Schedules** — Browse completed and upcoming matches for specific leagues and seasons
- **Match Deep Dive** — Inspect individual matches with lineups, formations, substitutions, and in-game statistics
- **Club Intelligence** — Search for clubs, view profiles with stadium information, and retrieve current squad rosters
- **Player Analytics** — Search players, view career profiles, seasonal statistics, and complete transfer histories

### How it works

1. Subscribe to this server
2. Enter your SportDB API Key from the [SportDB Dashboard](https://dashboard.sportdb.dev)
3. Start querying sports data from Claude, Cursor, or any MCP-compatible client

Your agent navigates the entire competition hierarchy — from country to league to season to match — so you never have to dig through sports websites manually.

### Who is this for?

- **Sports Analysts & Journalists** — instantly pull live scores, standings, and player stats to enrich reporting
- **Fantasy League Managers** — monitor player form, transfer activity, and team performance from your workspace
- **Developers & Data Engineers** — integrate professional-grade multi-sport data into AI-powered applications


## Available Tools
- **get_club_players**: Requires the numeric club ID.

List all players currently registered to a specific club
- **get_club_profile**: Requires the numeric club ID obtained from search results.

Get the full profile of a club by its ID
- **get_competition_seasons**: g., "premier-league"), returns all available seasons. Use this to find the season identifier needed for standings and fixtures queries.

List available seasons for a specific competition
- **get_country_competitions**: g., "england", "spain", "germany"), returns all competitions available in that country. The response includes competition slugs needed to drill deeper into seasons and standings.

List competitions (leagues/cups) available in a specific country for a sport
- **get_fixtures**: Includes dates, teams, scores for completed matches, and upcoming schedule. Requires sport, country_slug, competition_slug, and season.

Get scheduled and completed match fixtures for a season
- **get_match**: Use the match_id obtained from fixtures or live results.

Get detailed information for a specific match by its ID
- **get_match_lineups**: Returns player names and positions for each side.

Get starting lineups and substitutions for a specific match
- **get_match_stats**: Requires a valid match_id.

Get in-match statistics for a specific match
- **get_player_profile**: Requires the numeric player ID obtained from search results.

Get the full profile of a player by their ID
- **get_player_stats**: Requires the numeric player ID.

Get career and seasonal statistics for a specific player
- **get_player_transfers**: Requires the numeric player ID.

Get the complete transfer history of a specific player
- **get_standings**: Requires sport, country_slug, competition_slug, and season (e.g., "2024-2025"). This is the primary tool for answering "who is top of the league" questions.

Get league table standings for a specific season of a competition
- **list_countries**: The sport parameter should be a slug like "football", "basketball", "hockey", or "tennis". Use this as the starting point to navigate the competition hierarchy.

List all countries available for a given sport
- **get_live_basketball**: Use this when the user asks about ongoing basketball games or live NBA/EuroLeague results.

Get live basketball match scores happening right now
- **get_live_football**: Use this when the user asks about ongoing football games, current scores, or live results.

Get live football (soccer) match scores happening right now
- **get_live_hockey**: Use this when the user asks about ongoing hockey games or live NHL/KHL results.

Get live ice hockey match scores happening right now
- **search_clubs**: Returns a list of matching clubs with their IDs and basic metadata. Use this to find a club ID before requesting its profile or player roster.

Search for clubs/teams by name keyword
- **search_players**: Returns matching players with their IDs and basic profile data. Use this to find a player ID before requesting their detailed profile, statistics, or transfer history.

Search for players by name keyword


## Installation & Usage

To install and use the **SportDB** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/sportdb](https://vinkius.com/mcp/sportdb)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
