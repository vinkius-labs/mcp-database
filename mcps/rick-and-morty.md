# Rick and Morty MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/rick-and-morty)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/rick-and-morty-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/rick-and-morty-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [artificial-intelligence](../categories/artificial-intelligence.md)

Explore characters, locations, and episodes from the Rick and Morty universe via AI.

## Description
Connect the **Rick and Morty API** to any AI agent and explore the complete show database including all characters, locations across dimensions, and every episode with air dates and character appearances through natural language.

### What you can do

- **Character Database** — Search and retrieve detailed info on 200+ characters including status, species, origin, and location
- **Location Explorer** — Browse dimensions, planets, and facilities across the multiverse
- **Episode Guide** — Access all episodes with air dates, codes, and full character cast lists
- **Filter & Search** — Filter characters by status (alive/dead), species, gender, or name
- **Batch Lookup** — Retrieve multiple characters, locations, or episodes in a single request

### How it works

1. Subscribe to this server
2. No API key required — the Rick and Morty API is free and open
3. Start exploring the multiverse from Claude, Cursor, or any MCP-compatible client


## Available Tools
- **get_character**: Get detailed character information
- **get_characters**: Get multiple characters at once
- **get_episode**: Get detailed episode information
- **get_episodes**: Get multiple episodes at once
- **get_location**: Get detailed location information
- **get_locations**: Get multiple locations at once
- **list_characters**: Supports filtering by name, status (alive/dead/unknown), species, type, and gender. Returns character names, species, status, and basic info.

List Rick and Morty characters
- **list_episodes**: Supports filtering by episode name and episode code (e.g., "S01E01").

List Rick and Morty episodes
- **list_locations**: Supports filtering by name, type (e.g., "Planet", "Dimension"), and dimension name.

List Rick and Morty locations


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Rick and Morty** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Show me all alive human characters."

**🤖 AI Agent:**
> Found 42 alive human characters including Morty Smith, Summer Smith, Jerry Smith, Beth Smith, and many others. Want details on any of them?

---

**👤 You:**
> "Tell me about Rick Sanchez."

**🤖 AI Agent:**
> Rick Sanchez (ID: 1) is an alive Human male, status: Alive. Origin: Earth (C-137). Current location: Earth (C-137). He has appeared in 51 episodes across all seasons.

---

**👤 You:**
> "What happened in episode S01E01?"

**🤖 AI Agent:**
> S01E01 is 'Pilot' — the first episode of Rick and Morty, aired on December 2, 2013. It features 16 characters including Rick Sanchez, Morty Smith, Jerry Smith, Summer Smith, and Beth Smith. This is the iconic origin episode where Rick moves in with the Smith family.


## Installation & Usage

To install and use the **Rick and Morty** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/rick-and-morty](https://vinkius.com/mcp/rick-and-morty)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
