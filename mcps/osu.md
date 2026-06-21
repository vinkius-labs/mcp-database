# Osu! MCP Server

Access Osu! player profiles, beatmap data, scores, and community discussions directly through your AI agent.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/osu)

## Overview
**Category:** audio-music
**Tools Count:** 13

## Description
Connect your **Osu!** account to any AI agent to explore the rhythm game's vast ecosystem through natural conversation. This server provides deep integration with the Osu! API v2, allowing for comprehensive data retrieval and analysis.

### What you can do

- **Player Profiles** — Retrieve detailed public profile information for the authenticated user, including stats and rankings.
- **Beatmap Exploration** — Search for beatmapsets, lookup specific beatmaps by ID or hash, and browse curated beatmap packs.
- **Performance Analysis** — Calculate difficulty attributes for beatmaps with specific mod combinations and rulesets.
- **Leaderboards & Scores** — Fetch top scores for any beatmap or check a specific user's performance on a target map.
- **Community Insights** — Access beatmapset discussions, posts, and votes to stay updated on mapping trends and feedback.

### How it works

1. Subscribe to this server
2. Enter your Osu! Personal Access Token
3. Start querying player stats and beatmap data from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Competitive Players** — Quickly check your stats, top scores, and analyze map difficulty with different mods without leaving your workflow.
- **Mappers & Modders** — Inspect discussion posts and votes on beatmapsets to manage feedback and community interaction.
- **Data Enthusiasts** — Extract beatmap attributes and scoring data for analysis or performance tracking.


## Available Tools
- **get_beatmap_attributes**: Get beatmap attributes
- **get_beatmap_pack**: Get a specific beatmap pack
- **list_beatmap_packs**: Get beatmap packs
- **get_beatmap_scores**: Get scores for a beatmap
- **get_beatmapset**: Get a beatmapset
- **list_discussion_posts**: Get beatmapset discussion posts
- **list_discussion_votes**: Get beatmapset discussion votes
- **list_discussions**: Get beatmapset discussions
- **get_favourites**: Get user beatmapset favourites
- **lookup_beatmap**: Lookup a beatmap
- **get_me**: Requires identify scope.

Get own user data
- **search_beatmapsets**: Search beatmapsets
- **get_user_beatmap_score**: Get a user's score on a beatmap


## Installation & Usage

To install and use the **Osu!** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/osu](https://vinkius.com/mcp/osu)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
