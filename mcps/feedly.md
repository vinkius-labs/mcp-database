# Feedly MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/feedly)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/feedly-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/feedly-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [content-management](../categories/content-management.md)

Manage your news aggregation via Feedly — list collections, read streams, and search for feeds directly through your AI agent.

## Description
Connect your **Feedly** account to any AI agent and take full control of your news consumption and RSS aggregation through natural conversation.

### What you can do

- **Collection Orchestration** — List all your curated collections and feeds to organize your information flow natively
- **Stream Intelligence** — Retrieve the latest articles from specific feeds or entire categories with full metadata flawlessly
- **Read State Management** — Mark articles as read or save them for later directly from the cloud without manual UI interaction
- **Content Discovery** — Search for new RSS feeds and trending topics across the entire Feedly index flawlessly
- **Board & Tag Organization** — List and query articles from your personal boards and tagged content natively
- **User Insights** — Access your Feedly profile and subscription metadata through the agent synchronously

### How it works

1. Subscribe to this server
2. Enter your Feedly Developer Access Token
3. Start managing your news feed from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Researchers & Analysts** — quickly pull the latest industry news and trending topics into your AI-powered research flow
- **Content Creators** — monitor multiple sources and save inspiration to Feedly boards directly from your chat
- **Knowledge Workers** — stay updated on curated feeds without leaving your primary productivity workspace


## Available Tools
- **get_board_contents**: Retrieve articles from a specific board
- **get_entry**: Get details for a specific article entry
- **get_profile**: Get current Feedly user profile
- **get_stream_contents**: Retrieve articles for a specific stream (feed, category, or global)
- **get_subscriptions**: List all individual feed subscriptions
- **get_tag_contents**: Retrieve articles associated with a specific tag
- **list_boards**: List all your Feedly boards (saved for later)
- **list_collections**: List all your Feedly collections (categories) and feeds
- **list_tags**: List all your Feedly tags
- **mark_as_read**: Mark specific articles as read
- **search_feeds**: Search for new RSS feeds in the Feedly index
- **search_topics**: Search for trending topics or specific interests


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Feedly** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List my Feedly collections."

**🤖 AI Agent:**
> I've retrieved your collections. You have 'Tech News', 'Design Inspiration', and 'Marketing' categories. Which collection's latest articles would you like to see?

---

**👤 You:**
> "Show me the latest 5 articles from the 'Tech News' category."

**🤖 AI Agent:**
> Fetching stream contents... Here are the latest updates including 'AI Breakthroughs in 2024' and 'New Smartphone Launch'. Would you like me to summarize any of these for you?

---

**👤 You:**
> "Search for feeds about 'Edge Computing'."

**🤖 AI Agent:**
> Searching the Feedly index... I found several relevant feeds including 'The Edge Blog' and 'Computing Weekly'. Would you like the stream IDs to add them to your collections?


## Installation & Usage

To install and use the **Feedly** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/feedly](https://vinkius.com/mcp/feedly)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
