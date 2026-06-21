# Omnivore (Read-Later) MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/omnivore-read-later)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/omnivore-read-later-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/omnivore-read-later-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Manage your Omnivore library — search articles, read full content, and save new links directly from your AI agent.

## Description
Connect your **Omnivore** account to any AI agent to organize your reading list and extract knowledge from saved articles using natural language.

### What you can do

- **Search & Filter** — Use the `search_articles` tool to find content using labels, folders, or read status (e.g., 'is:unread label:AI')
- **Full Content Retrieval** — Use `get_article` to fetch the complete text, author, and labels for deep analysis or summarization
- **Quick Saving** — Use `save_url` to instantly add new web links to your library without leaving your conversation
- **User Profile** — Use `get_me` to verify your account details and connection status

### How it works

1. Subscribe to this server
2. Enter your Omnivore API Key
3. Start managing your reading list from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Researchers** — quickly find and analyze saved papers or articles within their library
- **Content Creators** — retrieve source material and inspiration from their curated reading list
- **Knowledge Workers** — maintain a seamless flow between reading and acting on information


## Available Tools
- **get_article**: Get full content of a specific article
- **get_me**: Get current Omnivore user details
- **save_url**: Save a URL to Omnivore library
- **search_articles**: g., label:Newsletter, in:inbox, is:unread, has:highlights) to find articles.

Search and filter articles in Omnivore library


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Omnivore (Read-Later)** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Search my Omnivore library for unread articles about 'Machine Learning'."

**🤖 AI Agent:**
> I found 3 unread articles about Machine Learning. The most recent is 'Understanding Transformers' (slug: understanding-transformers). Would you like me to fetch the full content of any of these?

---

**👤 You:**
> "Fetch the full content of the article with slug 'mcp-guide' for username 'alex_dev'."

**🤖 AI Agent:**
> I've retrieved the article 'The Ultimate MCP Guide'. It covers the Model Context Protocol architecture and implementation details. Would you like a summary of the key points?

---

**👤 You:**
> "Save the URL 'https://blog.omnivore.app/p/getting-started' to my library."

**🤖 AI Agent:**
> Successfully saved the URL to your Omnivore library. It is now available in your inbox for later reading.


## Installation & Usage

To install and use the **Omnivore (Read-Later)** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/omnivore-read-later](https://vinkius.com/mcp/omnivore-read-later)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
