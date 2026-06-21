# SteamSpy MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/steamspy)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [data-analytics](../categories/data-analytics.md)

Access Steam market data and game statistics — track owners, playtime, and trending titles directly from your AI agent.

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


## 💬 Prompt Examples

Here are some examples of how you can interact with the **SteamSpy** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Show me the statistics for Counter-Strike: Global Offensive (AppID 730)."

**🤖 AI Agent:**
> I've retrieved the data for CS:GO (AppID 730). It has an estimated 100,000,000+ owners, with an average playtime of over 30,000 minutes per user. The current price is listed as 0 (Free to Play).

---

**👤 You:**
> "What are the top 100 games by player count in the last two weeks?"

**🤖 AI Agent:**
> Fetching the trending titles... The top games by recent activity include 'Counter-Strike 2', 'Dota 2', and 'PUBG: BATTLEGROUNDS'. Would you like to see the full list or details for a specific one?

---

**👤 You:**
> "List the most popular games with the 'RPG' tag."

**🤖 AI Agent:**
> Searching for top-rated RPGs... I found several highly-owned titles with the 'RPG' tag, including 'Baldur's Gate 3', 'The Witcher 3: Wild Hunt', and 'Elden Ring'.


## ❓ FAQ

**Q: Can I get detailed ownership and playtime statistics for a specific game?**
Yes! Use the `get_app_details` tool with the Steam AppID. It returns owner estimates, average playtime, median playtime, and price information.

**Q: How can I find the most popular games on Steam right now?**
You can use the `get_top_100_in_2_weeks` tool to see which games have the most active players over the last 14 days, or `get_top_100_owned` for the most owned games of all time.

**Q: Is it possible to browse games by specific categories like 'Indie' or 'Strategy'?**
Absolutely. Use the `get_genre` tool for broad categories or the `get_tag` tool for more specific community-defined labels to see top games in those segments.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/steamspy](https://vinkius.com/mcp/steamspy)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **SteamSpy** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `steamspy` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **SteamSpy** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "steamspy": {
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
