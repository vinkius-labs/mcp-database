# SuperHero MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/superhero)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/superhero-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/superhero-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [knowledge-management](../categories/knowledge-management.md)

Access the ultimate comic book database — search characters, compare powerstats, and explore biographies from Marvel, DC, and more.

## Description
Connect to the **SuperHero API** and bring the multiverse to your AI agent. Access comprehensive data on thousands of characters from Marvel, DC, Dark Horse, and other major publishers through natural conversation.

### What you can do

- **Character Search** — Find any hero or villain by name to retrieve their unique ID and basic info.
- **Powerstats Analysis** — Compare intelligence, strength, speed, durability, power, and combat metrics for any character.
- **Biographical Data** — Explore full names, alter egos, aliases, first appearances, and alignment (good/bad).
- **Physical Appearance** — Get precise details on race, height, weight, and eye/hair color.
- **Connections & Work** — Discover group affiliations, relatives, occupations, and bases of operations.
- **Visual Assets** — Retrieve portrait image URLs for character identification.

### How it works

1. Subscribe to this server
2. Enter your SuperHero API Access Token
3. Start querying character data from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Content Creators & Writers** — Quickly verify comic book lore, character facts, and power levels without manual searching.
- **Developers & Gamers** — Integrate rich character metadata and stats into gaming projects or entertainment apps.
- **Comic Book Enthusiasts** — Compare stats and histories across different universes and publishers instantly.


## Available Tools
- **get_appearance**: Get physical appearance statistics for a specific character
- **get_biography**: Get biographical data for a specific character
- **get_character**: Get all information for a specific character by ID
- **get_connections**: Get connections for a specific character
- **get_image**: Get the portrait image URL for a specific character
- **get_powerstats**: Get powerstats for a specific character
- **get_work**: Get work details for a specific character
- **search_characters**: Useful for finding the ID to use in other endpoints.

Search for characters by their name


## 💬 Prompt Examples

Here are some examples of how you can interact with the **SuperHero** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Search for characters named 'Batman' and show me their IDs."

**🤖 AI Agent:**
> I found several matches for 'Batman'. The main Bruce Wayne version is ID 70 (DC Comics). There is also a Terry McGinnis version (ID 71). Which one would you like to explore?

---

**👤 You:**
> "What are the powerstats for character ID 332?"

**🤖 AI Agent:**
> For Hulk (ID 332), the powerstats are: Intelligence: 88, Strength: 100, Speed: 63, Durability: 100, Power: 98, and Combat: 85. He is at maximum level for strength and durability.

---

**👤 You:**
> "Get the full biography and image for character ID 620."

**🤖 AI Agent:**
> Character ID 620 is Spider-Man (Peter Parker). He first appeared in Amazing Fantasy #15 and is published by Marvel Comics. I've also retrieved his portrait image URL for you.


## Installation & Usage

To install and use the **SuperHero** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/superhero](https://vinkius.com/mcp/superhero)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
