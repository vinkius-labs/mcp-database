# GIPHY MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/giphy)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/giphy-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/giphy-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [image-video](../categories/image-video.md)

Search, discover and share millions of GIFs and stickers via AI.

## Description
Connect **GIPHY**, the world's largest GIF library, to any AI agent and instantly search, discover, and retrieve animated content through natural language.

### What you can do

- **GIF Search** — Search millions of GIFs by keyword with rating and pagination filters
- **Trending Content** — Retrieve currently trending GIFs and stickers
- **Text Translation** — Convert any phrase to the most relevant GIF automatically
- **Random Discovery** — Get random GIFs for inspiration or entertainment
- **Sticker Library** — Access transparent animated stickers for messaging
- **Category Browsing** — Explore GIFs organized by categories and tags

### How it works

1. Subscribe to this server
2. Enter your GIPHY API Key (free from developers portal)
3. Start discovering GIFs from Claude, Cursor, or any MCP-compatible client


## Available Tools
- **get_gif_by_id**: Get a specific GIF by its ID
- **get_gifs_by_ids**: Get multiple GIFs by their IDs
- **list_gif_categories**: List available GIF categories
- **random_gif**: Optionally filter by tag or rating.

Get a random GIF
- **search_gifs**: Supports pagination, rating filters, and returns up to 50 results per request.

Search for GIFs by keyword
- **search_stickers**: Works same as GIF search but returns sticker-format content.

Search for animated stickers
- **search_tags**: Useful for tag autocomplete and suggestions.

Search for GIF tags by keyword
- **translate_to_gif**: More precise than search.

Convert text to a relevant GIF
- **trending_gifs**: Perfect for finding viral and popular content.

Get currently trending GIFs
- **trending_searches**: Get currently trending search terms
- **trending_stickers**: Get currently trending stickers


## 💬 Prompt Examples

Here are some examples of how you can interact with the **GIPHY** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Find me a happy birthday GIF."

**🤖 AI Agent:**
> Here's a trending 'Happy Birthday' GIF with colorful confetti and dancing cake. URL: https://giphy.com/gifs/happy-birthday-xyz

---

**👤 You:**
> "Show me what GIFs are trending right now."

**🤖 AI Agent:**
> Top trending GIFs right now include: funny cat reactions, sports highlights, and celebrity moments. Here are the top 10 with their URLs.

---

**👤 You:**
> "Convert 'good morning' to a GIF."

**🤖 AI Agent:**
> Perfect match! Found a cute coffee cup with sunrise animation that says 'Good Morning!' URL: https://giphy.com/gifs/good-morning-coffee


## Installation & Usage

To install and use the **GIPHY** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/giphy](https://vinkius.com/mcp/giphy)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
