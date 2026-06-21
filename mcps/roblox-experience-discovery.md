# Roblox Experience Discovery MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/roblox-experience-discovery)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/roblox-experience-discovery-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/roblox-experience-discovery-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [industry-titans](../categories/industry-titans.md)

The definitive server for Roblox experiences — search games, track live players, and discover trends via AI.

## Description
Equip your AI agent with the pulse of the world's largest user-generated gaming platform via **Roblox Experience Discovery**. This server provides deep access to the official Roblox Games database, allowing your agent to instantly identify trending experiences, monitor live player counts, audit community voting stats, and retrieve high-resolution thumbnails for thousands of universes. Whether you are a developer researching market gaps or a gamer looking for the next viral hit like Blox Fruits, your agent acts as a professional Roblox analyst through natural conversation.

### What you can do

- **Comprehensive Discovery** — Search for Roblox experiences using keywords and retrieve live metadata including player counts and creators
- **Deep Auditing** — Fetch detailed metadata for specific universe IDs, including creation dates, descriptions, and technical root place IDs
- **Community Intelligence** — Access official voting statistics (likes/dislikes) to quantify the community sentiment for any title
- **Visual Retrieval** — Retrieve official icons and thumbnails to identify the visual identity of games in seconds

### How it works

1. Subscribe to this server
2. No API key required for public discovery access
3. Start managing your Roblox intelligence from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Game Researchers** — instantly monitor the hype and player base of specific genres and titles
- **Content Creators** — identify trending experiences and new updates for technical reporting and videos
- **Gamers & Parents** — track the popularity and community rating of experiences with micro-metric precision


## Available Tools
- **get_game_badges**: List badges associated with an experience
- **get_game_details**: Get comprehensive details for an experience
- **get_game_icons**: Get the official icon for a game
- **get_game_media**: Get promotional images and videos for a game
- **get_game_servers**: Use the Place ID.

List active public servers for a game
- **get_game_votes**: Get like/dislike stats for an experience
- **get_game_sorts**: List available game sort categories
- **search_roblox_games**: Search for Roblox experiences by keyword


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Roblox Experience Discovery** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Identify the top trending games on Roblox right now and show their player counts."

**🤖 AI Agent:**
> Retrieving global sorts... I've identified the current top experiences including 'Blox Fruits' (540k+ players) and 'Adopt Me!'. I also found high momentum in several new simulator titles. Would you like the detailed voting stats for these games?

---

**👤 You:**
> "Search for Roblox experiences matching the keyword 'Tycoon'."

**🤖 AI Agent:**
> Running the game search for 'Tycoon'... I found 20 matching experiences. The most popular is 'Restaurant Tycoon 2' with 45k players online. I also identified 'Supermarket Tycoon'. Shall I provide the creator details for the top results?

---

**👤 You:**
> "Get full metadata and the creation date for universe ID '123456789'."

**🤖 AI Agent:**
> Inspecting universe metadata... Universe ID '123456789' was created on 2021-05-12. It has reached over 1 billion visits and is currently active. I also have the root place ID and technical description. Would you like to see the official icon URL?


## Installation & Usage

To install and use the **Roblox Experience Discovery** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/roblox-experience-discovery](https://vinkius.com/mcp/roblox-experience-discovery)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
