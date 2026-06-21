# Osu! MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/osu)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/osu-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/osu-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [audio-music](../categories/audio-music.md)

Access Osu! player profiles, beatmap data, scores, and community discussions directly through your AI agent.

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


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Osu!** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Show me my Osu! profile and current rankings."

**🤖 AI Agent:**
> I've retrieved your profile. You are currently Rank #12,450 globally with 5,200 PP and 98.5% accuracy. Would you like to see your top performances?

---

**👤 You:**
> "What are the top scores for beatmap ID 1234567?"

**🤖 AI Agent:**
> Fetching the leaderboard for beatmap 1234567... The #1 score is held by 'PlayerOne' with 1,200,340 points and a 99.8% Hidden+HardRock run.

---

**👤 You:**
> "Calculate the difficulty of beatmap 987654 with DoubleTime."

**🤖 AI Agent:**
> With DoubleTime applied, beatmap 987654 increases from 5.2 stars to 7.4 stars. The Approach Rate (AR) is now 10.3 and the BPM has increased to 270.


## Installation & Usage

To install and use the **Osu!** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/osu](https://vinkius.com/mcp/osu)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
