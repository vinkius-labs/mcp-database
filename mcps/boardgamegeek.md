# BoardGameGeek MCP Server

Explore the world's largest board game database — search 150,000+ games, view ratings, player counts, complexity, trending titles, user collections and play logs.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/boardgamegeek)

## Overview
**Category:** knowledge-management
**Tools Count:** 10

## Description
Connect your **BoardGameGeek** account to any AI agent and unlock the full analytical power of the world's largest board game database.

### What you can do

- **Smart Game Search** — Find any of 150,000+ board games by name with fuzzy or exact matching, instantly retrieving BGG IDs for deep inspection
- **Deep Game Intelligence** — Fetch comprehensive metadata for any game: year published, player count range, play time, complexity weight, Bayesian rating, user rating, global rank, description and artwork
- **Trending Discovery** — See what's hot right now across board games, RPGs, video games, and industry people
- **User Collections** — Browse any player's full collection with personal ratings, play counts, wishlist and want-to-play status
- **Play History Analytics** — Analyze a user's logged play sessions filtered by date range, revealing play patterns and favorite games
- **Community Engagement** — Access game forums, read discussion threads, rules clarifications and community reviews
- **Guild Exploration** — Discover BGG guilds, their members and community organizing around shared tabletop interests

### How it works

1. Subscribe to this server
2. No API key needed — BoardGameGeek's API is fully open
3. Start exploring board game data from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Board Gamers** — discover new games, compare ratings/complexity, and explore curated collections from veteran players
- **Game Designers & Publishers** — research market positioning, competitive analysis, and community reception for similar titles
- **Content Creators & Reviewers** — gather structured data for videos, articles and podcasts without manually browsing dozens of pages
- **Event Organizers & Café Owners** — find games filtered by player count and duration to curate the perfect game night lineup


## Available Tools
- **get_forum_list**: g. Reviews, Rules, General, Strategy) associated with a specific board game by its BGG ID. Use the returned forum IDs to browse individual threads.

List discussion forums for a board game
- **get_game_plays**: Returns who played, when, and any comments. Useful for gauging a game's active community and recent engagement.

Get recent play logs for a specific board game
- **get_guild**: Guilds are community groups on BGG organized around shared interests.

Get details about a BoardGameGeek guild
- **get_hot_items**: Defaults to "boardgame" type but also supports "rpg", "videogame", "boardgameperson", "boardgamecompany". Ideal for discovering what is popular in the hobby right now.

Get the current trending/hot board games on BoardGameGeek
- **get_thing**: Returns game names, year published, min/max players, playing time, complexity weight, Bayesian/user ratings, rank, description and thumbnail. Use comma-separated IDs for multiple games.

Get detailed info for a board game by BGG ID
- **get_thread**: Useful for reading discussions, rules clarifications, or reviews about a game.

Read a specific forum thread on BoardGameGeek
- **get_user_collection**: Returns all games owned with stats, ratings, play counts, own/want/wishlist status. Optionally filter by subtype or exclude expansions.

Get a BGG user's board game collection
- **get_user_info**: Useful for understanding a user's preferences and social connections on the platform.

Get a BoardGameGeek user profile
- **get_user_plays**: Returns game names, play dates, locations, quantities and comments. Optionally filter by date range using YYYY-MM-DD format.

Get a user's board game play history
- **search_games**: Returns matching games with their BGG IDs, primary names, year published. Use the returned ID with get_thing to fetch full details including ratings, player count and complexity.

Search for board games by name on BoardGameGeek


## Installation & Usage

To install and use the **BoardGameGeek** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/boardgamegeek](https://vinkius.com/mcp/boardgamegeek)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
