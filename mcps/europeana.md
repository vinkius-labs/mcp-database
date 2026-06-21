# Europeana MCP Server

Explore millions of cultural heritage items — search artworks, books, and records from European museums and libraries directly through your AI agent.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/europeana)

## Overview
**Category:** knowledge-management
**Tools Count:** 4

## Description
Connect to **Europeana**, the digital heart of Europe's cultural heritage. This MCP server allows your AI agent to search and retrieve metadata for millions of digitized items from thousands of European galleries, libraries, archives, and museums.

### What you can do

- **Advanced Search** — Use `search_records` to find specific items using boolean operators and filters (e.g., searching for 'Paris' AND 'Louvre' with image filters).
- **Detailed Metadata** — Retrieve deep technical and descriptive metadata for specific cultural objects using `get_record` with collection and record IDs.
- **Entity Exploration** — Discover linked information about People, Places, Topics, and Organizations associated with cultural records via `get_entity`.
- **Bulk Harvesting** — Access professional-grade metadata harvesting through the `oaipmh_request` tool for large-scale data analysis.

### How it works

1. Subscribe to this server
2. Enter your Europeana API Key (WSKey)
3. Start exploring European history and art from Claude, Cursor, or any MCP client

### Who is this for?

- **Researchers & Academics** — Quickly find primary sources and metadata for historical research.
- **Educators** — Discover high-quality cultural assets and descriptions for lesson planning.
- **Developers & Data Scientists** — Access structured cultural data for applications or analysis via OAI-PMH.


## Available Tools
- **get_entity**: Retrieve information about linked entities
- **oaipmh_request**: Returns XML data.

Bulk harvesting of metadata via OAI-PMH
- **get_record**: Get detailed information about a specific cultural heritage object
- **search_records**: Search Europeana metadata


## Installation & Usage

To install and use the **Europeana** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/europeana](https://vinkius.com/mcp/europeana)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
