# Tenor MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/tenor)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/tenor-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/tenor-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [image-video](../categories/image-video.md)

Search and discover the world's largest library of GIFs and stickers directly from your AI agent.

## Description
Connect your AI agent to **Tenor** to bring visual expression to your workflows. Access millions of GIFs and stickers, discover trending content, and get smart search suggestions through natural conversation.

### What you can do

- **GIF & Sticker Search** — Find the perfect visual for any emotion or topic using powerful search filters and safety levels.
- **Trending Content** — Stay up to date with global trends by fetching currently featured GIFs and trending search terms.
- **Smart Suggestions** — Get alternative search terms and autocomplete suggestions to refine your visual discovery.
- **Category Exploration** — Browse curated categories like reactions or specific emotions to find exactly what you need.
- **Direct Access** — Retrieve specific GIF metadata and posts using unique IDs for precise sharing.

### How it works

1. Subscribe to this server
2. Enter your Tenor API Key (obtained from Google Cloud Console)
3. Start searching for GIFs in Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Content Creators** — Find relevant visual content for social media posts and articles without leaving your workspace.
- **Community Managers** — Quickly grab the perfect reaction GIF to engage with your audience.
- **Developers** — Integrate visual search capabilities into your AI-driven applications and chat interfaces.


## Available Tools
- **get_autocomplete**: Retrieve autocomplete suggestions for a partial search term
- **list_categories**: Retrieve a list of GIF categories
- **get_featured_gifs**: Retrieve the current global featured GIFs
- **get_posts**: Retrieve specific GIFs by their IDs
- **register_share**: Use this when a user explicitly selects/shares a GIF.

Register a share event when a user selects a GIF
- **get_search_suggestions**: Retrieve alternative search terms for a query
- **search_gifs**: Search for GIFs on Tenor
- **get_trending_terms**: Retrieve the current trending search terms


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Tenor** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Search for funny 'victory dance' GIFs on Tenor."

**🤖 AI Agent:**
> I've found several 'victory dance' GIFs for you. Here are the top results, including a celebratory Carlton dance and a joyful animated character. Which one would you like to use?

---

**👤 You:**
> "What are the trending search terms on Tenor right now?"

**🤖 AI Agent:**
> The current trending terms on Tenor include 'Monday motivation', 'happy birthday', 'shocked face', and 'congratulations'. Would you like to see GIFs for any of these?

---

**👤 You:**
> "Give me some search suggestions related to 'coffee'."

**🤖 AI Agent:**
> Based on 'coffee', here are some suggested search terms: 'morning coffee', 'coffee addict', 'iced coffee', and 'need coffee'. Should I search for one of these instead?


## Installation & Usage

To install and use the **Tenor** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/tenor](https://vinkius.com/mcp/tenor)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
