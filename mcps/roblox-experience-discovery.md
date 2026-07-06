# Roblox Experience Discovery MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/roblox-experience-discovery)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [industry-titans](../categories/industry-titans.md)

The definitive server for Roblox experiences — search games, track live players, and discover trends via AI.

## Description
Equip your AI agent with the pulse of the world's largest user-generated gaming platform via **Roblox Experience Discovery**. This server provides deep access to the official Roblox Games database, allowing your agent to instantly identify trending experiences, monitor live player counts, audit community voting stats, and retrieve high-resolution thumbnails for thousands of universes. Whether you are a developer researching market gaps or a gamer looking for the next viral hit like Blox Fruits, your agent acts as a professional Roblox analyst through natural conversation.

### What you can do

- **Comprehensive Discovery** — Search for Roblox experiences using keywords and retrieve live metadata including player counts and creators
- **Deep Auditing** — Fetch detailed metadata for specific universe IDs, including creation dates, descriptions, and technical root place IDs
- **Community Intelligence** — Access official voting statistics (likes/dislikes) to quantify the community sentiment for any title
- **Visual Retrieval** — Retrieve official icons and thumbnails to identify the visual identity of games in seconds

### How it works

1. Subscribe to this server
2. No API key required for public discovery access
3. Start managing your Roblox intelligence from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Game Researchers** — instantly monitor the hype and player base of specific genres and titles
- **Content Creators** — identify trending experiences and new updates for technical reporting and videos
- **Gamers & Parents** — track the popularity and community rating of experiences with micro-metric precision


## Available Tools (8)
- **get_game_servers**: Use the Place ID.

List active public servers for a game
- **get_game_votes**: Get like/dislike stats for an experience
- **get_game_sorts**: List available game sort categories
- **search_roblox_games**: Search for Roblox experiences by keyword
- **get_game_badges**: List badges associated with an experience
- **get_game_details**: Get comprehensive details for an experience
- **get_game_icons**: Get the official icon for a game
- **get_game_media**: Get promotional images and videos for a game


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Roblox Experience Discovery** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Identify the top trending games on Roblox right now and show their player counts."

**🤖 AI Agent:**
> Retrieving global sorts... I've identified the current top experiences including 'Blox Fruits' (540k+ players) and 'Adopt Me!'. I also found high momentum in several new simulator titles. Would you like the detailed voting stats for these games?

---

**👤 You:**
> "Search for Roblox experiences matching the keyword 'Tycoon'."

**🤖 AI Agent:**
> Running the game search for 'Tycoon'... I found 20 matching experiences. The most popular is 'Restaurant Tycoon 2' with 45k players online. I also identified 'Supermarket Tycoon'. Shall I provide the creator details for the top results?

---

**👤 You:**
> "Get full metadata and the creation date for universe ID '123456789'."

**🤖 AI Agent:**
> Inspecting universe metadata... Universe ID '123456789' was created on 2021-05-12. It has reached over 1 billion visits and is currently active. I also have the root place ID and technical description. Would you like to see the official icon URL?


## ❓ FAQ

**Q: Can my AI automatically find the live player count for a specific Roblox game?**
Yes! Use the `search_roblox_games` tool. Your agent will retrieve real-time data from the Roblox backend, showing exactly how many users are currently active in that experience.

**Q: How do I check the community rating (likes/dislikes) for a universe?**
Simply provide the Universe ID to the agent and ask for voting stats. It will run the `get_game_votes` action to retrieve the official percentage of upvotes and downvotes directly from the track.

**Q: Does the integration permit listing trending games globally?**
Yes. The `get_game_sorts` tool allows your agent to fetch current global categories like 'Top Rated', 'Popular', and 'Trending' to identify high-momentum titles in seconds.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/roblox-experience-discovery](https://vinkius.com/mcp/roblox-experience-discovery)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Roblox Experience Discovery** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `roblox-experience-discovery` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Roblox Experience Discovery** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "roblox-experience-discovery": {
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
