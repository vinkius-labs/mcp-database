# Punk MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/punk)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/punk-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/punk-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [developer-tools](../categories/developer-tools.md)

Explore the BrewDog beer catalog — search by ingredients, food pairings, and technical specs like ABV or IBU.

## Description
Access the complete **BrewDog** beer library through the Punk API. This MCP server allows your AI agent to act as a digital sommelier or brewing consultant.

### What you can do

- **Advanced Search** — Filter the catalog by ABV (alcohol by volume), IBU (bitterness), or EBC (color) using precise ranges.
- **Ingredient Analysis** — Search for beers containing specific hops, malts, or yeast strains to understand flavor profiles.
- **Food Pairing** — Get instant recommendations for beers that complement specific dishes or cuisines.
- **Detailed Specs** — Retrieve full recipes, brewing tips, and technical measurements for any beer in the database.
- **Random Discovery** — Let the agent suggest a surprise brew from the extensive collection.

### How it works

1. Subscribe to this server
2. Enter 'OPEN' in the token field (this is a public API)
3. Start exploring recipes and pairings from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Homebrewers** — quickly look up hop profiles and malt bills without leaving your research notes
- **Foodies & Chefs** — find the perfect craft beer to pair with your latest recipe
- **App Developers** — test beer-related data structures and API responses in a conversational environment


## Available Tools
- **get_beer**: Get a single beer by ID
- **list_beers**: Supports pagination and filtering by ABV, IBU, EBC, ingredients, and food pairings.

List beers from the BrewDog catalog
- **get_random_beer**: Get a random beer


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Punk** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List some beers that go well with spicy curry."

**🤖 AI Agent:**
> I've searched the BrewDog catalog for you. Based on your request for spicy curry, I recommend 'Punk IPA' (ID: 192) and 'Jack Hammer' (ID: 37). Both have the bitterness and hop profile to balance the heat. Would you like the full details for one of these?

---

**👤 You:**
> "Show me the details for beer with ID 192."

**🤖 AI Agent:**
> Fetching details for ID 192... This is 'Punk IPA', a Post Modern Classic with 5.6% ABV. It features Chinook, Ahtanum, and Nelson Sauvin hops. It pairs perfectly with spicy meat pizza or burger. Would you like the brewing method details?

---

**👤 You:**
> "Give me a random beer recommendation with an ABV higher than 6%."

**🤖 AI Agent:**
> I'll find a strong random brew for you... I've selected 'Hardcore IPA' (ID: 15). It has a powerful 9.2% ABV and 125 IBU. It's an explicit imperial ale with a massive hop hit. Does this sound like what you're looking for?


## Installation & Usage

To install and use the **Punk** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/punk](https://vinkius.com/mcp/punk)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
