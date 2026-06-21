# Calibre-Web MCP Server

Browse and manage your Calibre-Web library via OPDS and Kobo sync — access catalogs, specific shelves, and device metadata directly.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/calibre-web)

## Overview
**Category:** knowledge-management
**Tools Count:** 3

## Description
Connect your **Calibre-Web** instance to any AI agent and interact with your digital book collection using natural language. This server provides tools to navigate your library structure and prepare books for e-reader synchronization.

### What you can do

- **OPDS Catalog Access** — Retrieve the main OPDS XML feed to browse your entire library structure, categories, and recent additions.
- **Shelf Browsing** — Query specific shelf IDs to list books within curated collections or user-defined categories.
- **Kobo Synchronization** — Fetch structured metadata and secure download links optimized for Kobo devices using your dedicated sync token.
- **Library Inspection** — Use the AI to find specific book entries and metadata within your self-hosted instance.

### How it works

1. Subscribe to this server
2. Enter your Calibre-Web instance URL and optional credentials
3. Start exploring your library from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Avid Readers** — quickly find books in large collections without manual searching
- **Digital Librarians** — verify shelf contents and catalog structures via chat
- **Kobo Users** — automate the retrieval of sync metadata for your e-reader devices


## Available Tools
- **sync_kobo_library**: Requires Kobo Token.

Sync Kobo library
- **get_opds_catalog**: Useful for browsing the library structure.

Get the main OPDS catalog feed
- **get_opds_shelf**: Get the OPDS feed for a specific shelf


## Installation & Usage

To install and use the **Calibre-Web** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/calibre-web](https://vinkius.com/mcp/calibre-web)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
