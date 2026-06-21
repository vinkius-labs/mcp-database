# Fern MCP Server

Manage and interact with Fern documentation platforms — generate access tokens, index websites for AI, and query analytics directly from your agent.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/fern)

## Overview
**Category:** developer-tools
**Tools Count:** 6

## Description
Connect to the **Fern** ecosystem to supercharge your documentation workflows. This server allows AI agents to manage documentation access, trigger AI indexing, and interact with the 'Ask Fern' assistant.

### What you can do

- **AI Chat Completion** — Interact with the Ask Fern AI assistant to get answers from specific documentation domains using `post_chat_completion`.
- **Website Indexing** — Trigger new crawling and indexing jobs via `index_website` to keep your documentation searchable and AI-ready.
- **Access Management** — Generate JWTs and Algolia search keys for secure documentation access using `get_jwt` and `get_search_key`.
- **Analytics & Insights** — Retrieve recent user queries and analytics with `get_recent_queries` to understand how people interact with your docs.
- **User Verification** — Quickly check authentication status and user details with the `whoami` tool.

### How it works

1. Subscribe to this server
2. Enter your Fern API Key and Token
3. Start managing your documentation lifecycle from your favorite AI client

### Who is this for?

- **Documentation Engineers** — automate the indexing of new content and monitor search analytics.
- **Support Teams** — use the Ask Fern AI to find answers across complex documentation domains.
- **Developers** — programmatically manage access keys and verify user permissions.


## Available Tools
- **get_jwt**: Get JWT from Fern API key
- **get_recent_queries**: Get recent queries and analytics
- **get_search_key**: Get Algolia search credentials
- **index_website**: Start crawling and indexing a website for Ask Fern
- **post_chat_completion**: Interact with the Ask Fern AI assistant
- **whoami**: Get current user information


## Installation & Usage

To install and use the **Fern** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/fern](https://vinkius.com/mcp/fern)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
