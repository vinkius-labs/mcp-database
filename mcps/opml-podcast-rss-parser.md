# OPML Podcast & RSS Parser MCP Server

Turn standard OPML export files from your podcast app or RSS reader into clean JSON data. Let your AI analyze your subscriptions and become your personal content curator.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/opml-podcast-rss-parser)

## Overview
**Category:** productivity
**Tools Count:** 1

## Description
When you want Claude to recommend new podcasts or blogs based on what you already consume, you export an `.opml` file from Apple Podcasts, Pocket Casts, or Feedly. But XML outlines are noisy, recursive, and confusing for LLMs to read efficiently.

This MCP uses a fast, deterministic XML parser to flatten the OPML hierarchy into a simple, structured list of your subscriptions, dropping all the unnecessary XML tags and attributes.

### The Superpowers

- **Universal Support:** Parses OPML files from any standard podcast player or RSS reader.
- **Zero Token Waste:** Converts heavy XML markup into a clean, flat JSON array.
- **Local Privacy:** Your subscription habits are parsed locally, ensuring they aren't uploaded to a public server.
- **Assistant Ready:** Turn Claude into your personal entertainment and news curator.


## Available Tools
- **parse_opml_feeds**: Provide the absolute file path.

Parse an OPML file (Podcast or RSS feed export) into a clean JSON list of subscriptions


## Installation & Usage

To install and use the **OPML Podcast & RSS Parser** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/opml-podcast-rss-parser](https://vinkius.com/mcp/opml-podcast-rss-parser)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
