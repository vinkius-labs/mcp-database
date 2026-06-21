# Fortnite Map, Playlists & Engine Intelligence MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/fortnite-map-playlists-engine-intelligence)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/fortnite-map-playlists-engine-intelligence-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/fortnite-map-playlists-engine-intelligence-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [artificial-intelligence](../categories/artificial-intelligence.md)

The technical server for Fortnite engine data — track the island map, active gamemodes, and AES keys via AI.

## Description
Equip your AI agent with the structural intelligence of the Fortnite ecosystem via **Fortnite Map, Playlists & Engine Intelligence**. This specialized server provides deep access to the technical core of the game, allowing your agent to instantly retrieve the current island map with high-resolution imagery, audit active Points of Interest (POIs), and list all currently available game modes and playlists. Additionally, it provides essential technical data for developers and modders, including official AES keys for pak file decryption and current build versioning. Whether you are analyzing map changes or auditing technical metadata, your agent acts as a professional Fortnite engine analyst through natural conversation.

### What you can do

- **Cartographic Auditing** — Retrieve the official current island map, including coordinates for all named Points of Interest (POIs)
- **Playlist Intelligence** — List all active and limited-time game modes (LTMs), including player limits and technical descriptions
- **Technical Access** — Fetch official AES keys required for pak file analysis and decryption directly from the latest game build
- **Version Monitoring** — Track the latest game versions, build IDs, and technical update timestamps in real-time

### How it works

1. Subscribe to this server
2. Enter your Fortnite-API Key (obtainable via their official dashboard)
3. Start managing your Fortnite technical intelligence from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Technical Analysts** — perform deep audits of map changes and POI distributions after every patch
- **Developers & Modders** — instantly retrieve the latest AES keys and pak file metadata for developmental research
- **Pro Gamers & Coaches** — identify active playlists and player limits to optimize training sessions and strategies


## Available Tools
- **get_aes_encryption_keys**: Useful for datamining.

Get encryption keys for game files
- **get_battle_royale_news**: Get current Battle Royale news
- **get_banner_colors**: List all banner color options
- **get_profile_banners**: List all Fortnite profile banner icons
- **get_current_map**: Get the current Fortnite map with POIs
- **get_playlist_details**: Get details for a specific playlist/gamemode
- **get_save_the_world_news**: Get current Save the World news
- **list_all_playlists**: List all available Fortnite playlists


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Fortnite Map, Playlists & Engine Intelligence** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Show me the current island map and list all named POIs."

**🤖 AI Agent:**
> Retrieving high-res satellite map... I've identified the current island configuration. Major POIs include 'Tilted Towers' and 'Pleasant Park'. I also have the blank map imagery for tactical planning. Would you like the coordinates for any specific location?

---

**👤 You:**
> "What are the current AES keys for version 29.40?"

**🤖 AI Agent:**
> Checking engine metadata... For version 29.40, the main AES key is `0x44AB...`. I also found 5 dynamic keys for recent pak files. Would you like the full technical list of encrypted file names?

---

**👤 You:**
> "List all active 50v50 or large team gamemodes available today."

**🤖 AI Agent:**
> Running the playlist audit... I found an active LTM 'Big Battle' which supports up to 40 players per match. I also identified 'Team Rumble'. Would you like to see the minimum player requirements for these modes?


## Installation & Usage

To install and use the **Fortnite Map, Playlists & Engine Intelligence** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/fortnite-map-playlists-engine-intelligence](https://vinkius.com/mcp/fortnite-map-playlists-engine-intelligence)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
