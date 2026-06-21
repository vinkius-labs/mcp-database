# LinkAce MCP Server

Manage your bookmarks, tags, and collections via the LinkAce REST API.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/linkace)

## Overview
**Category:** productivity
**Tools Count:** 9

## Description
Connect your **LinkAce** instance to any AI agent to automate your personal knowledge base and link archiving. This MCP server enables your agent to add new bookmarks, organize them into lists and tags, and search your entire library directly from natural language interfaces.

### What you can do

- **Instant Archiving** — Quickly add new URLs to your LinkAce library with custom titles and descriptions
- **Deep Organization** — Create and manage tags and lists to keep your bookmarks categorized and easy to find
- **Semantic Discovery** — Search through your entire archived library using keywords via natural language commands
- **Library Maintenance** — Retrieve detailed metadata for specific links or permanently remove outdated bookmarks
- **Self-Hosted Support** — Works with any self-hosted LinkAce instance using your personal API token

### How it works

1. Subscribe to this server
2. Enter your LinkAce API Key (Bearer Token) and your Instance URL
3. Start managing your links from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Researchers** — Automatically archive and tag useful resources while you work or browse
- **Developers** — Build a personal technical library and search for specific snippets or documentation links
- **Power Users** — Automate the curation of your personal bookmark manager directly from your productivity tools


## Available Tools
- **create_new_bookmark**: Requires at least a URL.

Add a new link to your archive
- **create_new_collection**: Add a new collection (list)
- **create_new_tag**: Add a new tag
- **delete_bookmark**: Remove a bookmark from your archive
- **get_bookmark_details**: Get details for a specific bookmark
- **list_all_bookmarks**: List all bookmarks (links) in your LinkAce account
- **list_all_collections**: List all bookmark collections (lists)
- **search_bookmarks**: Search for bookmarks by keyword
- **list_all_tags**: List all tags used for organizing bookmarks


## Installation & Usage

To install and use the **LinkAce** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/linkace](https://vinkius.com/mcp/linkace)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
