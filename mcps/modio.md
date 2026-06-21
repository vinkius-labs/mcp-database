# Mod.io MCP Server

Manage game mods, browse titles, and handle subscriptions via mod.io — discover, rate, and organize game content directly from any AI agent.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/modio)

## Overview
**Category:** developer-tools
**Tools Count:** 22

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


## Installation & Usage

To install and use the **Mod.io** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/modio](https://vinkius.com/mcp/modio)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
