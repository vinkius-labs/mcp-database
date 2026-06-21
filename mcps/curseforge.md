# CurseForge MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/curseforge)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/curseforge-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/curseforge-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [developer-tools](../categories/developer-tools.md)

Access the world's largest repository of gaming mods — search for projects, fetch metadata, and manage mod files for Minecraft, WoW, and more.

## Description
Connect to the **CurseForge** API and empower your AI agent to navigate the vast ecosystem of gaming modifications. From Minecraft to World of Warcraft, this server provides deep access to mod metadata, file management, and discovery tools.

### What you can do

- **Mod Discovery** — Search for mods using filters like game ID, category, version, and text search via `search_mods`.
- **Detailed Metadata** — Fetch complete mod descriptions, screenshots, and author information using `get_mod` and `get_mod_description`.
- **File Management** — Retrieve specific mod files, changelogs, and direct download URLs using `get_mod_file` and `get_mod_file_download_url`.
- **Game Intelligence** — List supported games, version types, and categories to understand the structure of different gaming ecosystems.
- **Fingerprint Matching** — Identify mods from local files using fingerprint matching tools like `get_fingerprints_matches`.

### How it works

1. Subscribe to this server
2. Enter your CurseForge API Key
3. Start exploring and managing mods from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Gamers & Modders** — Quickly find the latest versions of your favorite mods and read changelogs without leaving your chat interface.
- **Tool Developers** — Integrate CurseForge data into your own applications or mod managers using the AI as a bridge.
- **Server Administrators** — Automate the process of checking for mod updates and gathering download links for server packs.


## Available Tools
- **list_categories**: Get all available classes and categories for a game
- **get_files_batch**: Get a list of files by their IDs
- **get_fingerprints_matches_fuzzy**: Get matches for a list of file fingerprints using fuzzy matching
- **get_fingerprints_matches**: Used for identifying mods from local files.

Get matches for a list of file fingerprints
- **get_game**: Get details for a specific game
- **list_games**: List all games available to the API key
- **get_mod_description**: Get the HTML description of a mod
- **get_mod_file_changelog**: Get the HTML changelog for a specific file
- **get_mod_file_download_url**: Get a signed download URL for a specific file
- **get_mod_file**: Get details for a specific file of a mod
- **list_mod_files**: Get all files for a specific mod
- **get_mod**: Get details for a specific mod
- **get_mods_batch**: Get a list of mods by their IDs
- **search_mods**: Search for mods based on criteria
- **list_game_version_types**: Get all available version types for a game
- **list_game_versions_v1**: Get all available versions for a game (V1)
- **list_game_versions_v2**: Get detailed version information for a game (V2)


## 💬 Prompt Examples

Here are some examples of how you can interact with the **CurseForge** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Search for Minecraft mods with 'industrial' in the name."

**🤖 AI Agent:**
> I found several mods. The most popular is 'Industrial Foregoing' (ID: 266515). Would you like to see its full description or available files?

---

**👤 You:**
> "Get the HTML description for mod ID 238222."

**🤖 AI Agent:**
> I've retrieved the description for 'Just Enough Items (JEI)'. It includes details on usage, keybindings, and configuration options. Should I summarize the main features for you?

---

**👤 You:**
> "List all categories available for game ID 432."

**🤖 AI Agent:**
> For Minecraft (ID: 432), I found categories such as 'Adventure and RPG', 'Magic', 'Technology', and 'Storage'. Which category would you like to explore?


## Installation & Usage

To install and use the **CurseForge** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/curseforge](https://vinkius.com/mcp/curseforge)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
