# Movie Watchlist Analyzer MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/movie-watchlist-analyzer)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [entertainment](../categories/entertainment.md)

Analyze movie watchlists to get total counts, genre distributions, and decade breakdowns.

## Description
This MCP server provides tools to analyze the composition and integrity of movie watchlists. Use `get_watchlist_summary` to find the total and unique movie counts across multiple lists, `get_genre_distribution` to see how genres are spread, and `get_decade_breakdown` to view the temporal distribution of releases. You can also use `validate_watchlist_completeness` to ensure all entries have the necessary title and year information.


## Available Tools (4)
- **get_watchlist_summary**: Provides a high-level overview of the total number of movies in a watchlist
- **validate_watchlist_completeness**: Checks if a watchlist contains any entries missing critical information (title or year)
- **get_decade_breakdown**: Analyzes the temporal distribution of movies by their release decade
- **get_genre_distribution**: You can optionally filter by specific genres.

Answers how many movies in a watchlist belong to specific genres


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Movie Watchlist Analyzer** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "How many unique movies are in watchlists 'wl-123' and 'wl-456'?"

**🤖 AI Agent:**
> There are 45 unique movies across those two watchlists.

---

**👤 You:**
> "What is the genre distribution for watchlist 'action-fans'?"

**🤖 AI Agent:**
> The watchlist contains 12 Action movies, 5 Sci-Fi movies, and 3 Thriller movies.

---

**👤 You:**
> "Is my watchlist 'my-favorites' complete?"

**🤖 AI Agent:**
> Yes, the watchlist is complete with all movies having titles and release years.


## ❓ FAQ

**Q: How can I see the total number of movies in my lists?**
You can use the `get_watchlist_summary` tool by providing the IDs of the watchlists you want to analyze.

**Q: Can I check if my watchlist is missing any data?**
Yes, the `validate_watchlist_completeness` tool checks if any movies are missing a title or a release year.

**Q: How do I see which decades my movies were released in?**
Use the `get_decade_breakdown` tool to get a count of movies grouped by their release decade.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/movie-watchlist-analyzer](https://vinkius.com/en/ai-agent-connect/movie-watchlist-analyzer)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Movie Watchlist Analyzer** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `movie-watchlist-analyzer` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Movie Watchlist Analyzer** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "movie-watchlist-analyzer": {
      "url": "https://edge.vinkius.com/[TOKEN]/mcp"
    }
  }
}
```

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius connector registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
