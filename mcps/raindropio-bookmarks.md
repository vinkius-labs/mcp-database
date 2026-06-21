# Raindrop.io (Bookmarks) MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/raindropio-bookmarks)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/raindropio-bookmarks-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/raindropio-bookmarks-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Manage your Raindrop.io bookmarks, collections, and tags directly from any AI agent.

## Description
Connect your **Raindrop.io** account to any AI agent and take full control of your digital library through natural conversation.

### What you can do

- **Collection Management** — List root and child collections, create new folders, or merge existing ones to keep your library organized.
- **Bookmark Operations** — Create, update, or delete individual raindrops (bookmarks). Support for bulk operations allows you to manage multiple links at once.
- **Tagging & Filtering** — Organize your content with tags. List, rename, merge, or delete tags to maintain a clean taxonomy.
- **Highlights & Backups** — Access all your saved highlights across collections and view your available backups.
- **Trash Maintenance** — Quickly empty your trash to permanently remove unwanted items.

### How it works

1. Subscribe to this server
2. Enter your Raindrop.io Personal Access Token
3. Start managing your knowledge base from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Researchers** — instantly save and categorize sources without leaving your research chat.
- **Developers** — manage technical bookmarks and documentation links directly from your IDE.
- **Knowledge Workers** — organize deep-dive reading lists and project resources using natural language.


## Available Tools
- **create_collection**: Create a new collection
- **create_many_raindrops**: Create multiple raindrops
- **create_raindrop**: Create a new raindrop (bookmark)
- **delete_collection**: Delete a collection
- **delete_many_raindrops**: Delete multiple raindrops
- **delete_raindrop**: Delete a raindrop (bookmark)
- **delete_tags**: Delete tags
- **empty_trash**: Empty the trash collection
- **get_collection**: Get a single collection
- **get_public_user**: Get public user details
- **get_raindrop**: Get a single raindrop (bookmark)
- **get_user**: io user.

Get authenticated user details
- **list_all_highlights**: List all highlights
- **list_backups**: List all backups
- **list_child_collections**: List child collections
- **list_collection_highlights**: List highlights in a collection
- **list_filters**: ) for a collection.

List filters
- **list_raindrops**: Use 0 for all, -1 for unsorted, -99 for trash.

List raindrops in a collection
- **list_root_collections**: List root collections
- **list_tags**: List tags
- **merge_collections**: Merge multiple collections
- **rename_merge_tags**: Rename or merge tags
- **update_collection**: Update a collection
- **update_many_raindrops**: Update multiple raindrops
- **update_raindrop**: Update a raindrop (bookmark)
- **update_user**: Update authenticated user details


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Raindrop.io (Bookmarks)** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all my top-level bookmark collections."

**🤖 AI Agent:**
> I've retrieved your root collections. You have: 'Unsorted' (ID: 0), 'Work' (ID: 12345), and 'Personal' (ID: 67890). Which one would you like to explore?

---

**👤 You:**
> "Save https://mcp.io to my 'Research' collection with the tag 'ai'."

**🤖 AI Agent:**
> Successfully created a new raindrop for 'mcp.io' in your 'Research' collection (ID: 55443) with the tag 'ai'.

---

**👤 You:**
> "Empty my trash collection."

**🤖 AI Agent:**
> I have permanently deleted all items in your Trash collection.


## Installation & Usage

To install and use the **Raindrop.io (Bookmarks)** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/raindropio-bookmarks](https://vinkius.com/mcp/raindropio-bookmarks)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
