# Open Brewery DB MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/open-brewery-db-alternative)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/open-brewery-db-alternative-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/open-brewery-db-alternative-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [business-intelligence](../categories/business-intelligence.md)

Search and discover craft breweries worldwide — find locations, types, and contact info via AI.

## Description
Connect **Open Brewery DB**, the largest open-source brewery database, to any AI agent and search, discover, and explore craft breweries worldwide through natural language.

### What you can do

- **Brewery Search** — Search 30,000+ breweries worldwide by name, city, state, or country
- **Type Filtering** — Filter by brewery type: micro, nano, regional, brewpub, large, planning, and more
- **Location Discovery** — Find breweries near you by geographic coordinates or postal code
- **Autocomplete** — Get brewery name suggestions for type-ahead search
- **Contact Details** — Retrieve addresses, phone numbers, and website URLs for any brewery
- **Geographic Data** — Access latitude/longitude coordinates for mapping and distance calculations

### How it works

1. Subscribe to this server
2. No API key required — Open Brewery DB is free and open
3. Start discovering breweries from Claude, Cursor, or any MCP-compatible client


## Available Tools
- **autocomplete_breweries**: Useful for type-ahead search or finding breweries by partial name.

Autocomplete brewery names
- **get_breweries_by_ids**: Get multiple breweries by their IDs
- **get_brewery**: Get a single brewery by ID
- **get_breweries_by_city**: Results can be paginated and sorted.

Get breweries by city
- **get_breweries_by_country**: Results can be paginated and sorted.

Get breweries by country
- **get_breweries_by_postal**: Supports 5-digit ZIP or ZIP+4 format.

Get breweries by postal code
- **get_breweries_by_state**: Use the full state name, not abbreviation.

Get breweries by state
- **get_breweries_by_type**: Types include: micro (small craft), nano (very small), regional (regional craft), brewpub (brewery + restaurant), large (major brewery), planning, contract, proprietor, closed.

Get breweries by type
- **get_nearby_breweries**: Results are sorted by distance.

Get breweries near a location
- **list_breweries**: Supports filtering by city, state, country, postal code, and brewery type. Results can be sorted and paginated.

List breweries with filters
- **search_breweries**: Matches against name, city, state, and other fields. Results are paginated.

Search breweries by name or location


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Open Brewery DB** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Find microbreweries in Portland, Oregon."

**🤖 AI Agent:**
> Found 47 microbreweries in Portland, Oregon. Top results include 'Breakside Brewery', 'Cascade Brewing', and 'Hair of the Dog Brewing'. Would you like addresses and websites for any of these?

---

**👤 You:**
> "What brewpubs are near downtown Denver?"

**🤖 AI Agent:**
> Found 12 brewpubs within 5 miles of downtown Denver (39.7392, -104.9903). Nearest: 'Wynkoop Brewing Company' at 1634 18th St, Denver. Also nearby: 'Great Divide Brewing' and 'Denver Beer Co.'.

---

**👤 You:**
> "Search for breweries with 'dog' in the name."

**🤖 AI Agent:**
> Found 8 breweries with 'dog' in the name including 'Hair of the Dog Brewing' (Portland, OR), 'Pug Runner Brewing' (Denver, CO), and 'Barking Dog Brewing' (Austin, TX).


## Installation & Usage

To install and use the **Open Brewery DB** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/open-brewery-db-alternative](https://vinkius.com/mcp/open-brewery-db-alternative)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
