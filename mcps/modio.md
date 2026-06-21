# Mod.io MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/modio)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/modio-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/modio-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [developer-tools](../categories/developer-tools.md)

Manage game mods, browse titles, and handle subscriptions via mod.io — discover, rate, and organize game content directly from any AI agent.

## Description
Connect your **mod.io** account to any AI agent to manage your gaming library and modding workflows through natural conversation.

### What you can do

- **Game Discovery** — Browse all games on the platform using `get_games` and fetch detailed stats and metadata for specific titles with `get_game_stats`.
- **Mod Management** — Search for mods using `get_mods`, view detailed descriptions with `get_mod`, and manage your own mod profiles including adding, editing, or deleting entries.
- **User Subscriptions** — Subscribe or unsubscribe from mods using `subscribe_mod` and `unsubscribe_mod`, rate content with `rate_mod`, and track your personal collections.
- **Account Insights** — Access your profile with `get_me`, check your wallet information via `get_wallets`, and view purchased content directly through the API.

### How it works

1. Subscribe to this server
2. Enter your mod.io API Key and Access Token
3. Start managing your mods from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Gamers** — instantly find and subscribe to new mods for your favorite games without leaving your chat interface
- **Mod Creators** — manage your mod listings, update summaries, and check performance stats directly from your workspace
- **Community Managers** — monitor mod ratings and game statistics to understand community trends and engagement


## Available Tools
- **add_collection**: Requires OAuth 2 Access Token.

Create a new mod collection
- **add_mod**: Requires OAuth 2 Access Token.

Add a new mod to a game
- **get_collection_mods**: Get mods within a collection
- **get_collections**: Get all mod collections for a game
- **delete_mod**: Requires OAuth 2 Access Token.

Delete a mod
- **edit_mod**: Requires OAuth 2 Access Token.

Edit details of an existing mod
- **get_game_stats**: Get statistics for a game
- **get_game**: Get details for a specific game
- **get_games**: io platform.

Get all games on mod.io
- **get_me**: Requires OAuth 2 Access Token.

Get authenticated user details
- **get_mod_file**: Get a specific modfile
- **get_mod_files**: Get all files for a mod
- **get_mod**: Get details for a specific mod
- **get_mods**: Get all mods for a game
- **get_my_purchases**: Requires OAuth 2 Access Token.

Get mods purchased by the user
- **rate_mod**: Requires OAuth 2 Access Token.

Rate a mod
- **get_my_ratings**: Requires OAuth 2 Access Token.

Get ratings submitted by the user
- **subscribe_mod**: Requires OAuth 2 Access Token.

Subscribe to a mod
- **get_my_subscriptions**: Requires OAuth 2 Access Token.

Get mods the user is subscribed to
- **get_terms**: Get text and links for user consent dialogs
- **unsubscribe_mod**: Requires OAuth 2 Access Token.

Unsubscribe from a mod
- **get_my_wallets**: Requires OAuth 2 Access Token.

Get user wallets for monetization


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Mod.io** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all games available on mod.io."

**🤖 AI Agent:**
> I've retrieved the list of games. You can explore titles like 'Deep Rock Galactic' (ID: 123) or 'Totally Accurate Battle Simulator' (ID: 456). Which one would you like to see mods for?

---

**👤 You:**
> "Show me the mods for game ID 123."

**🤖 AI Agent:**
> Fetching mods for game 123... I found several entries using `get_mods`. Notable mods include 'Enhanced Lighting' and 'New Maps Pack'. Would you like the full details for any of these?

---

**👤 You:**
> "Rate mod 789 for game 123 as positive."

**🤖 AI Agent:**
> Processing your rating... I've used `rate_mod` to submit a positive rating for mod 789 in game 123. Your feedback has been successfully recorded.


## Installation & Usage

To install and use the **Mod.io** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/modio](https://vinkius.com/mcp/modio)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
