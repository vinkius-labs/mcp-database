# PunkAPI MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/punkapi)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/punkapi-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/punkapi-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Explore BrewDog's beer catalog — search by name, style, ABV, IBU, hops, food pairing and get random beer suggestions.

## Description
Connect to **PunkAPI** and explore BrewDog's DIY Dog beer catalog through natural conversation — completely free, no API key needed.

### What you can do

- **Beer Search** — Search beers by name, style, ABV, IBU, hops, yeast, malts and food pairing
- **Random Beers** — Get random beer suggestions for discovery
- **Beer Details** — Get full details including ingredients, brewing tips and food pairings
- **Filter by ABV** — Find session beers (low ABV) or strong beers (high ABV)
- **Filter by IBU** — Find mild or bitter beers based on preference
- **Food Pairing** — Find beers that pair well with specific foods
- **Hop Varieties** — Search beers by specific hop varieties

### How it works

1. Subscribe to this server
2. No API key needed — start searching immediately
3. Explore craft beers from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Beer Enthusiasts** — discover new beers, find beers by style and explore food pairings
- **Brewers** — research hop varieties, malt types and brewing recipes
- **Restaurants** — find beers that pair well with specific menu items


## Available Tools
- **get_all_beers**: Supports searching by name, ABV range, IBU range, EBC (color), malts, hops, yeast, food pairing and brewing date range. Returns beer names, descriptions, ABV, IBU, ingredients and food pairing suggestions. Pagination supported with page and per_page parameters.

Search BrewDog beers with filters
- **get_beer_by_id**: Returns name, description, ABV, IBU, EBC, first brewed date, tagline, ingredients (malts, hops, yeast), food pairing suggestions, brewers tips and description.

Get a specific beer by ID
- **get_beers_by_abv**: Use abv_gt for minimum ABV and abv_lt for maximum ABV. Useful for finding session beers (low ABV) or strong beers (high ABV).

Search beers by ABV (alcohol by volume) range
- **get_beers_by_food**: Common pairings include: "cheese", "burger", "spicy", "dessert", "chicken", "fish", "pork", "bbq", "chocolate", "fruit". Returns matching beers with their food pairing suggestions.

Search beers by food pairing suggestion
- **get_beers_by_hops**: Common hops include: "Cascade", "Citra", "Mosaic", "Amarillo", "Simcoe", "Galaxy", "Chinook", "Centennial". Returns matching beers with full hop ingredient details.

Search beers by hop variety
- **get_beers_by_ibu**: Low IBU (<20) = mild, Medium IBU (20-40) = balanced, High IBU (40-60) = bitter, Very High IBU (>60) = very bitter. Useful for finding beers matching bitterness preference.

Search beers by IBU (International Bitterness Units) range
- **get_beers_by_style**: Common styles include: "American IPA", "Scottish Ale", "Belgian IPA", "English IPA", "Porter", "Stout", "Lager", "Pilsner", "Wheat Beer", "Sour". Returns beer names, ABV, IBU and descriptions.

Search beers by style
- **get_random_beer**: Useful for discovering new beers. Can return 1-25 random beers at once.

Get random beer(s) from the catalog


## 💬 Prompt Examples

Here are some examples of how you can interact with the **PunkAPI** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Give me a random beer suggestion."

**🤖 AI Agent:**
> Punk IPA (5.4% ABV, 35 IBU) — A post-modern classic. Juicy, tropical and citrusy with Cascade, Amarillo and Centennial hops. Pairs well with spicy Indian food.

---

**👤 You:**
> "Find me beers that pair well with cheese."

**🤖 AI Agent:**
> Found 15 beers that pair with cheese including: Dead Pony Club (light, session), 5AM Saint (amber ale), Hardcore IPA (strong IPA), Tokyo Rising (dark, intense).

---

**👤 You:**
> "Show me all BrewDog IPAs."

**🤖 AI Agent:**
> Found 20+ IPAs including: Punk IPA (5.4%, classic), Elvis Juice (6.5%, grapefruit), Hazy Jane (5%, New England style), Punk AF (0.5%, non-alcoholic), Lost Lager (4.5%). Each with full hop profiles and food pairings.


## Installation & Usage

To install and use the **PunkAPI** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/punkapi](https://vinkius.com/mcp/punkapi)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
