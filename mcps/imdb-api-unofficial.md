# IMDB API (Unofficial) MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/imdb-api-unofficial)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [data-management](../categories/data-management.md)

Search movies and TV shows — audit ratings, cast, and metadata via IA.

## Description
Empower your AI agent to orchestrate your entire cinematic research and media auditing workflow with the **IMDB API (Unofficial)**, the comprehensive source for global film and television metadata. By connecting this IMDB intelligence to your agent, you transform complex movie searches into a natural conversation. Your agent can instantly search for titles, audit audience ratings, and retrieve detailed cast metadata without you ever touching a film database. Whether you are conducting industry research or managing local viewing constraints, your agent acts as a real-time cinematic consultant, ensuring your data is always comprehensive and up-to-the-minute.

### What you can do

- **Title Auditing** — Search for thousands of movies and TV shows by keyword and retrieve detailed metadata, including years and genres.
- **Rating Oversight** — Audit audience ratings for any title to understand the current industry lead in cinematic reception instantly.
- **Cast Discovery** — Retrieve full cast and crew lists for specific titles to assist in deep-dive filmography classification.
- **Metadata Intelligence** — Retrieve unique IMDB identifiers (ttIDs) and synopsis details to assist in professional media auditing.
- **Operational Monitoring** — Check API status to ensure your cinematic research workflow is always operational.

### How it works

1. Subscribe to this server
2. Enter your Unofficial IMDB API Key
3. Start managing your cinematic intelligence through Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Film Critics & Journalists** — monitor movie trends and retrieve official metadata straight from your workflow.
- **Media Researchers** — verify cast details and audit genre patterns without manual searching.
- **Entertainment Leads** — perform rapid audits of cinematic markers and identify relevant media themes through natural language.
- **Operations Leads** — automate media data querying to orchestrate cross-functional creative teams smoothly.


## Available Tools (4)
- **check_api_status**: Check if the IMDB service is operational
- **get_imdb_cast_details**: Get the full cast and crew list for a specific IMDB title
- **get_imdb_movie_details**: g., tt1234567).

Get full metadata and synopsis for a specific IMDB title by ID
- **search_imdb_movies**: Search for movies and TV shows on IMDB


## 💬 Prompt Examples

Here are some examples of how you can interact with the **IMDB API (Unofficial)** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Search for 'Inception' using IMDB."

**🤖 AI Agent:**
> I've retrieved the details for Inception! It was released in 2010 and has a rating of 8.8/10. Would you like the full cast list or the technical metadata for this title?

---

**👤 You:**
> "Show the cast for movie with ID 'tt0111161' (The Shawshank Redemption)."

**🤖 AI Agent:**
> I've identified the cast for The Shawshank Redemption! Notable actors include Tim Robbins as Andy Dufresne and Morgan Freeman as Ellis Boyd 'Red' Redding. I can provide the full list of crew metadata if you'd like.

---

**👤 You:**
> "Search for TV shows about 'space' on IMDB."

**🤖 AI Agent:**
> I've identified several space-themed series! Notable entries include 'The Expanse' and 'Star Trek'. I can provide the ratings and synopsis metadata for each of these titles to assist in your research.


## ❓ FAQ

**Q: How do I find my IMDB API Key?**
Register for an account at the [**imdbapi.dev portal**](https://imdbapi.dev/), and you will find your API Key in your dashboard after subscription. Copy and paste it below.

**Q: Does it support TV series?**
Yes. The API provides metadata and ratings for both movies and television series indexed in the IMDB database.

**Q: Can the agent show the full cast list?**
Yes. Use the `get_imdb_cast_details` tool providing a title ID to retrieve the list of all actors and their roles.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/imdb-api-unofficial](https://vinkius.com/mcp/imdb-api-unofficial)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **IMDB API (Unofficial)** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `imdb-api-unofficial` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **IMDB API (Unofficial)** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "imdb-api-unofficial": {
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
