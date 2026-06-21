# Yu-Gi-Oh MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/yu-gi-oh)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/yu-gi-oh-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/yu-gi-oh-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [databases](../categories/databases.md)

Access the ultimate Yu-Gi-Oh! database — search for cards, explore archetypes, and check set lists directly from your AI agent.

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


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Yu-Gi-Oh** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Search for card info on 'Blue-Eyes White Dragon'."

**🤖 AI Agent:**
> I've found the data for 'Blue-Eyes White Dragon'. It's a Level 8 LIGHT Dragon Normal Monster with 3000 ATK and 2500 DEF. It is one of the most iconic cards in the game.

---

**👤 You:**
> "List all Yu-Gi-Oh card sets available."

**🤖 AI Agent:**
> Fetching card sets... I've retrieved a list of all sets, including classics like 'Legend of Blue Eyes White Dragon' (LOB) and newer releases like 'Phantom Nightmare' (PHNI).

---

**👤 You:**
> "Give me a random Yu-Gi-Oh card."

**🤖 AI Agent:**
> Drawing a random card... You got 'Pot of Greed'! It's a Spell Card that allows you to draw 2 cards from your deck.


## Installation & Usage

To install and use the **Yu-Gi-Oh** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/yu-gi-oh](https://vinkius.com/mcp/yu-gi-oh)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
