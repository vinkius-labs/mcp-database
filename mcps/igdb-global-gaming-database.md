# IGDB Global Gaming Database MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/igdb-global-gaming-database)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [artificial-intelligence](../categories/artificial-intelligence.md)

The world's most comprehensive gaming database — audit titles, platforms, age ratings, and more via AI.

## Description
Empower your AI agent with the ultimate gaming intelligence via **IGDB**. This unified server provides access to the complete IGDB ecosystem, allowing your agent to search for thousands of titles, audit franchises, and retrieve detailed metadata for platforms, release dates, and artworks. Additionally, it includes deep support for industry taxonomy, including official genres, themes, keywords, and global age rating systems (ESRB, PEGI). Whether you are conducting market research, organizing a catalog, or managing a personal collection, your agent acts as a real-time gaming historian and analyst, providing precise data through natural conversation.

### What you can do

- **Comprehensive Discovery** — Search for video games and retrieve detailed metadata, including summaries, ratings, and first release dates
- **Taxonomy & Metadata** — Query official genres, platforms, and thematic tags to understand industry categorization
- **Content Safety Auditing** — Retrieve age ratings and content descriptions to verify maturity levels across different regions
- **Visual & Franchise Assets** — Fetch high-quality artworks, covers, and complete franchise or collection histories

### How it works

1. Subscribe to this server
2. Enter your IGDB Client ID and Access Token
3. Start managing your gaming intelligence from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Game Developers & Studios** — monitor industry trends, franchise history, and competitive benchmarks without manual browsing
- **Market Researchers** — audit platform distributions, age ratings, and genre trends across thousands of titles
- **Curators & Collectors** — automate the retrieval of metadata and high-quality artwork for gaming catalogs


## Available Tools
- **get_artworks**: Get official artworks for a game
- **list_collections**: Get details for a game collection or series
- **search_covers**: Get cover art for a game
- **list_release_dates**: Get release dates for a game
- **get_franchise**: Get details for a game franchise
- **get_game**: Get full details for a specific game ID
- **search_games**: Search for video games on IGDB
- **list_age_ratings**: List common age ratings
- **list_genres**: g., RPG, Shooter) available in the IGDB database.

List common game genres
- **list_keywords**: List descriptive keywords
- **list_platforms**: g., PS5, Xbox, PC) and their abbreviations.

List gaming platforms
- **list_themes**: List game themes


## 💬 Prompt Examples

Here are some examples of how you can interact with the **IGDB Global Gaming Database** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Search for the game 'Elden Ring' and provide its community rating and summary."

**🤖 AI Agent:**
> I've fetched Elden Ring's metadata. It has an exceptional community rating of 94% and is described as an action RPG developed by FromSoftware. Would you like to see the full list of platforms it was released on?

---

**👤 You:**
> "What are the official age ratings for 'Grand Theft Auto V' globally?"

**🤖 AI Agent:**
> Running the rating query... I've retrieved the data for GTA V. It is rated 'M' by ESRB in North America and '18' by PEGI in Europe due to intense violence and mature content. Would you like the specific content descriptors for these ratings?

---

**👤 You:**
> "List all games included in 'The Witcher' franchise."

**🤖 AI Agent:**
> Inspecting the franchise timeline... The Witcher series includes the three main RPG titles, the Gwent spin-off, and several expansions. Notable GIDs include 1942 for the original and 492 for Wild Hunt. Would you like the summaries for each entry?


## ❓ FAQ

**Q: Can my AI automatically find high-resolution artwork just by providing a game name?**
Yes! Your agent can use `search_games` to find the unique ID and then run `get_artworks` or `search_covers` to retrieve multiple high-resolution image URLs directly from the IGDB cloud in seconds.

**Q: How do I easily check if a game is suitable for certain age groups in different regions?**
Simply ask the agent to run the `list_age_ratings` tool. It will compile data from global systems like ESRB, PEGI, and CERO, providing precise content descriptors and rating levels for the target title.

**Q: Does the integration permit listing all games within a specific franchise or collection?**
Yes. Tools like `get_franchise` and `list_collections` allow your agent to retrieve the entire historical timeline of a series, grouping related titles and spin-offs under their structural parent IDs.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/igdb-global-gaming-database](https://vinkius.com/mcp/igdb-global-gaming-database)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **IGDB Global Gaming Database** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `igdb-global-gaming-database` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **IGDB Global Gaming Database** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "igdb-global-gaming-database": {
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
