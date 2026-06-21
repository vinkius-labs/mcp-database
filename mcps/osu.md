# Osu! MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/osu)
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


## ❓ FAQ

**Q: Can I calculate the difficulty of a beatmap with specific mods like DoubleTime or HardRock?**
Yes! Use the `get_beatmap_attributes` tool. You can provide the Beatmap ID and an array of mods to get the adjusted difficulty metrics like Star Rating, AR, and OD.

**Q: How do I find my own profile statistics?**
Simply run the `get_me` tool. It will return your public profile data, including your global rank, PP, and accuracy for your primary ruleset.

**Q: Is it possible to search for new beatmapsets by a specific artist?**
Yes, use the `search_beatmapsets` tool with a query string. For example, searching for 'Camellia' will return all relevant beatmapsets associated with that artist.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/osu](https://vinkius.com/mcp/osu)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Osu!** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `osu` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Osu!** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "osu": {
      "url": "https://edge.vinkius.com/[TOKEN]/mcp"
    }
  }
}
```

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
