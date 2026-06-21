# SteamSpy MCP Server

Access Steam market data and game statistics — track owners, playtime, and trending titles directly from your AI agent.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/steamspy)

## Overview
**Category:** data-analytics
**Tools Count:** 7

## Description
Connect to **SteamSpy** to empower your AI agent with deep insights into the Steam gaming ecosystem. Analyze market trends, player behavior, and game performance metrics through natural conversation.

### What you can do

- **Game Analytics** — Fetch detailed statistics for any Steam game, including owner estimates, price, and playtime metrics using its AppID.
- **Market Trends** — Discover the Top 100 games based on recent activity (2 weeks), all-time popularity, or total ownership.
- **Genre & Tag Exploration** — Filter the Steam catalog by specific genres or community tags to identify niche leaders or market gaps.
- **Bulk Data Retrieval** — Access the full SteamSpy database with paginated results to perform large-scale market research.

### How it works

1. Subscribe to this server
2. Enter your SteamSpy API Key (available via SteamSpy's developer portal)
3. Start querying gaming data from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Game Developers** — Research competitors, analyze genre saturation, and benchmark playtime metrics.
- **Market Analysts** — Track the growth of specific tags and monitor the performance of top-tier titles.
- **Gaming Enthusiasts** — Find trending games and deep-dive into the statistics of your favorite franchises.


## Available Tools
- **get_all**: Returns 1,000 entries per page.

Get all games with owner data
- **get_app_details**: Get details for a specific Steam application
- **get_genre**: Get games within a specific genre
- **get_tag**: Get games associated with a specific tag
- **get_top_100_forever**: Get Top 100 games by players since March 2009
- **get_top_100_in_2_weeks**: Get Top 100 games by players in the last two weeks
- **get_top_100_owned**: Get Top 100 games by number of owners


## Installation & Usage

To install and use the **SteamSpy** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/steamspy](https://vinkius.com/mcp/steamspy)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
