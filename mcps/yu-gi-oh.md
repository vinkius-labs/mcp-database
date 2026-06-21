# Yu-Gi-Oh MCP Server

Access the ultimate Yu-Gi-Oh! database — search for cards, explore archetypes, and check set lists directly from your AI agent.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/yu-gi-oh)

## Overview
**Category:** databases
**Tools Count:** 6

## Description
Connect your AI to the most comprehensive **Yu-Gi-Oh!** card database. Perfect for duelists, collectors, and developers looking for instant card data through natural conversation.

### What you can do

- **Card Search** — Find detailed stats, descriptions, and images using fuzzy search or specific filters like ATK, DEF, and Level via `get_card_info`.
- **Archetype Exploration** — List all game archetypes to understand deck themes and synergies using `list_archetypes`.
- **Set Information** — Browse all released card sets with `list_card_sets` and drill down into specific set contents using `get_card_set_info`.
- **Random Discovery** — Pull a random card from the database for inspiration or challenges using `get_random_card`.
- **Database Health** — Check the current version and last update timestamp with `check_db_version` to ensure you have the latest TCG/OCG data.

### How it works

1. Subscribe to this server
2. Enter your API credentials
3. Start querying card data from Claude, Cursor, or any MCP-compatible client

No more manual searching through wikis. Your AI acts as a master duelist with instant access to every card ever printed.

### Who is this for?

- **Players & Deck Builders** — Quickly check card effects, rulings, and legality without leaving your chat.
- **Collectors** — Track set lists and card IDs for inventory management and price checking.
- **Developers** — Integrate card data into your own projects or analysis tools using structured queries.


## Available Tools
- **list_archetypes**: List all card archetypes
- **get_card_info**: Retrieve detailed information for one or multiple cards
- **get_card_set_info**: Get information about a specific card set
- **list_card_sets**: List all Yu-Gi-Oh card sets
- **check_db_version**: Check database version
- **get_random_card**: Caching is disabled for this endpoint.

Get a random Yu-Gi-Oh card


## Installation & Usage

To install and use the **Yu-Gi-Oh** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/yu-gi-oh](https://vinkius.com/mcp/yu-gi-oh)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
