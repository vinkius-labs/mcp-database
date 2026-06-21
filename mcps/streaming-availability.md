# Watchmode Streaming Availability MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/streaming-availability)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/streaming-availability-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/streaming-availability-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [content-management](../categories/content-management.md)

Find where to watch any movie or TV show — search streaming availability across Netflix, Disney+, HBO Max, and 200+ platforms directly from your AI agent.

## Description
Connect your AI agent to **Watchmode**, the most accurate streaming availability metadata API. This MCP provides 8 tools to search, discover, and analyze where movies and TV shows are available to stream, rent, or buy across 200+ platforms in multiple regions.

### What you can do

- **Title Search** — Look up any movie or TV show by name to get Watchmode IDs and basic metadata
- **Full Details + Sources** — Retrieve comprehensive metadata (plot, ratings, genres) with all streaming sources and deep links in a single call
- **Availability Lookup** — Find exactly which platforms host a title: subscription, rent, buy, or free
- **Platform Discovery** — List all streaming services available in a specific country or region
- **Cast & Crew** — Access actors, directors, and writers for any title
- **Genre Catalog** — Browse all available genres for filtering
- **New Releases** — Track recently added titles across streaming platforms

### How it works

1. Subscribe to this server
2. Go to [**api.watchmode.com/requestApiKey**](https://api.watchmode.com/requestApiKey/) and request a free API key
3. No credit card required — the free plan includes 1,000 requests/month
4. Paste your API key into the field below
5. Start discovering where to watch your favorite content

### Who is this for?

- **Cinephiles & TV Fans** — instantly find where any title is streaming in your country
- **Entertainment Apps** — integrate real-time availability data into content discovery engines
- **Global Users** — check availability across different regions with a single query
- **Content Researchers** — verify legal access points for movies and series across platforms


## Available Tools
- **get_title_cast**: Get the cast and crew for a title
- **get_title_details**: Get full details and streaming sources for a title
- **get_title_sources**: Get all streaming sources where a title is available
- **list_genres**: List all available genres
- **list_releases**: List recently added or upcoming titles on streaming platforms
- **list_sources**: ) optionally filtered by country.

List all streaming services available in a region
- **list_titles**: Filter by type, streaming source, and region.

Browse a catalog of titles with filters
- **search_titles**: Returns matching titles with basic metadata.

Search for a movie or TV show by name


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Watchmode Streaming Availability** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Where can I watch 'The Last of Us'?"

**🤖 AI Agent:**
> I searched Watchmode and found 'The Last of Us' (TV Series). It's currently available for streaming on Max (HBO), and available for purchase on Apple TV and Amazon Prime Video. Want me to get the direct links?

---

**👤 You:**
> "List all streaming platforms available in Brazil."

**🤖 AI Agent:**
> I found 45+ streaming services available in Brazil, including Netflix, Disney+, Max, Amazon Prime Video, Globoplay, Apple TV+, and Paramount+. Would you like to search for a specific title on any of these?

---

**👤 You:**
> "Get the full cast of 'Oppenheimer'."

**🤖 AI Agent:**
> Here's the cast of 'Oppenheimer': Cillian Murphy as J. Robert Oppenheimer, Emily Blunt as Kitty Oppenheimer, Robert Downey Jr. as Lewis Strauss, Matt Damon as Leslie Groves. Directed by Christopher Nolan. Want to see where it's streaming?


## Installation & Usage

To install and use the **Watchmode Streaming Availability** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/streaming-availability](https://vinkius.com/mcp/streaming-availability)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
