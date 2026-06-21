# Amiibo MCP Server

Search and filter the complete Amiibo database — access figures, cards, and series data directly from any AI agent.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/amiibo)

## Overview
**Category:** databases
**Tools Count:** 7

## Description
Connect to the **AmiiboAPI** and explore the vast world of Nintendo's Amiibo collectibles through natural conversation. This server provides comprehensive access to data on figures, cards, and plushies.

### What you can do

- **Search & Filter** — Find Amiibos by name, character, game series, or collection series using the `list_amiibos` tool.
- **Detailed Inspection** — Get precise metadata for a specific Amiibo using its unique 16-digit ID with `get_amiibo`.
- **Metadata Discovery** — List all available types, game series, and characters to understand the scope of the collection.
- **Database Status** — Check when the Amiibo database was last synchronized with the latest releases using `get_last_updated`.

### How it works

1. Subscribe to this server
2. No API key is required for the public AmiiboAPI
3. Start querying Nintendo collectible data from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Collectors** — quickly check which Amiibos exist in a specific series or for a favorite character
- **Developers** — integrate Amiibo metadata into gaming apps or inventory trackers
- **Nintendo Fans** — explore the history and variety of Amiibo releases across different platforms


## Available Tools
- **get_amiibo**: Get data for a specific Amiibo by ID
- **get_last_updated**: Get database last updated timestamp
- **list_amiibo_series**: Get all Amiibo Series
- **list_amiibos**: Can be filtered by name, character, game series, amiibo series, type, or ID segments.

List all Amiibo with optional filters
- **list_characters**: Get all Characters
- **list_game_series**: Get all Game Series
- **list_types**: g., Figure, Card).

Get all Amiibo types


## Installation & Usage

To install and use the **Amiibo** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/amiibo](https://vinkius.com/mcp/amiibo)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
