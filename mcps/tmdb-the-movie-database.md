# TMDB (The Movie Database) MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/tmdb-the-movie-database)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [knowledge-management](../categories/knowledge-management.md)

Access movie, TV show, and actor data — search, discover, and retrieve detailed metadata directly from any AI agent.

## Description
Connect your AI agent to **The Movie Database (TMDB)** to access a world of cinematic information through natural conversation.

### What you can do

- **Search & Discover** — Find movies and TV shows using text search or advanced filters like genres, ratings, and release dates via `search_movies` and `discover_movies`.
- **Deep Metadata** — Fetch comprehensive details for movies, TV series, specific seasons, and individual episodes using `get_movie_details`, `get_tv_details`, and `get_tv_episode_details`.
- **Cast & Crew** — Retrieve detailed biographies and filmographies for actors and production members with `get_person_details`.
- **Certifications & Config** — Access official movie/TV certifications and system configurations to understand regional content ratings.
- **Account Management** — Manage guest sessions and retrieve account-specific details for personalized interactions.

### How it works

1. Subscribe to this server
2. Enter your TMDB API Read Access Token (v4)
3. Start exploring the world of cinema from Claude, Cursor, or any MCP-compatible client

No more manual searching through browser tabs to find release dates or cast lists. Your AI acts as a dedicated film buff and database researcher.


## Available Tools
- **get_account_details**: Get TMDB account details
- **get_configuration**: Get TMDB API configuration
- **discover_movies**: Discover movies by filters
- **create_guest_session**: Create a new guest session
- **get_movie_certifications**: Get movie certifications
- **get_movie_details**: Get details for a specific movie
- **get_person_details**: Get details for a specific person
- **create_request_token**: Create a new request token
- **search_movies**: Search for movies by text
- **get_tv_certifications**: Get TV certifications
- **get_tv_details**: Get details for a specific TV series
- **get_tv_episode_details**: Get details for a specific TV episode
- **get_tv_season_details**: Get details for a specific TV season


## 💬 Prompt Examples

Here are some examples of how you can interact with the **TMDB (The Movie Database)** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Search for the movie 'Inception'."

**🤖 AI Agent:**
> I found 'Inception' (1999) with ID 27205. It's a sci-fi masterpiece directed by Christopher Nolan. Would you like to see the full details or the cast list?

---

**👤 You:**
> "Discover top-rated horror movies from 2023."

**🤖 AI Agent:**
> I've filtered the database for 2023 horror movies. Notable titles include 'Talk to Me' and 'When Evil Lurks'. Would you like the specific details for any of these?

---

**👤 You:**
> "Get the details for season 1 of the TV show with ID 1399."

**🤖 AI Agent:**
> Fetching details for 'Game of Thrones' (ID: 1399) Season 1. It consists of 10 episodes, starting with 'Winter Is Coming'. Should I provide the summary for the first episode?


## ❓ FAQ

**Q: Can I filter movies by specific genres and ratings?**
Yes! Use the `discover_movies` tool. You can provide genre IDs in `with_genres` and use other filters like `sort_by` to find highly-rated content.

**Q: How do I get information about a specific actor?**
Use the `get_person_details` tool with the person's unique ID. It will return their biography, place of birth, and other metadata.

**Q: Can I see the episodes of a specific TV season?**
Absolutely. Use `get_tv_season_details` by providing the `series_id` and the `season_number`. It will list all episodes in that season.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/tmdb-the-movie-database](https://vinkius.com/mcp/tmdb-the-movie-database)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **TMDB (The Movie Database)** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `tmdb-the-movie-database` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **TMDB (The Movie Database)** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "tmdb-the-movie-database": {
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
