# Wallabag (Pocket Alternative) MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/wallabag-pocket-alternative)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/wallabag-pocket-alternative-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/wallabag-pocket-alternative-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Manage your self-hosted read-it-later list — save URLs, organize with tags, and retrieve article content directly from your AI agent.

## Description
Connect your **Wallabag** instance to any AI agent and transform your read-it-later list into an interactive knowledge base. Wallabag is the leading open-source alternative to Pocket and Instapaper, allowing you to host your own articles.

### What you can do

- **Article Management** — List all saved entries, fetch full content for specific articles, and save new URLs instantly.
- **Organization** — Mark articles as read (archive) or favorite (star), and manage tags to keep your library structured.
- **Annotations & Highlights** — Retrieve existing annotations or create new highlights and notes directly on your saved articles.
- **Tagging System** — List all your existing tags and apply them to entries to categorize your research.
- **Clean Reading** — Access the extracted text of articles without ads or distractions, perfect for AI analysis.

### How it works

1. Subscribe to this server
2. Enter your Wallabag instance URL and API credentials (Client ID, Secret, Username, and Password)
3. Start managing your reading list from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Researchers** — save sources and annotate them using AI to summarize key findings.
- **Knowledge Workers** — organize a massive backlog of articles and find exactly what you need via natural language.
- **Privacy Enthusiasts** — keep your reading data on your own server while still benefiting from AI-powered insights.


## Available Tools
- **add_tags_to_entry**: Add tags to a specific entry
- **create_annotation**: Create an annotation on an entry
- **create_entry**: Save a new URL to Wallabag
- **delete_entry**: Delete an entry from Wallabag
- **get_entry**: Get a single entry by ID
- **list_annotations**: Get annotations for an entry
- **list_entries**: Get all entries (articles) from Wallabag
- **list_tags**: Get all tags from Wallabag
- **mark_entry_favorite**: Mark an entry as favorite (starred)
- **mark_entry_read**: Mark an entry as read (archive)
- **remove_tag_from_entry**: Remove a tag from an entry


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Wallabag (Pocket Alternative)** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List my most recent articles from Wallabag."

**🤖 AI Agent:**
> I've retrieved your latest entries. You have articles like 'The Future of AI' (ID: 452) and 'Open Source Guide' (ID: 453). Would you like me to fetch the content for any of these?

---

**👤 You:**
> "Save this URL to my Wallabag: https://example.com/article"

**🤖 AI Agent:**
> Successfully saved! The article has been added to your Wallabag account with Entry ID 454. Would you like me to add any tags to it?

---

**👤 You:**
> "Mark article 452 as read and add the tag 'finished'."

**🤖 AI Agent:**
> Done. Article 452 has been archived and tagged as 'finished'.


## Installation & Usage

To install and use the **Wallabag (Pocket Alternative)** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/wallabag-pocket-alternative](https://vinkius.com/mcp/wallabag-pocket-alternative)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
