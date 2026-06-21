# MediaWiki MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/mediawiki)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/mediawiki-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/mediawiki-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [collaboration](../categories/collaboration.md)

Connect to any MediaWiki instance to search pages, read content, list categories, and track recent changes directly from your AI agent.

## Description
Connect your AI agent to any **MediaWiki** site (like Wikipedia or a private corporate wiki) to query knowledge, inspect page history, and explore categories through natural language.

### What you can do

- **Search & Discovery** — Use full-text search or list all pages in the main namespace to find specific information quickly
- **Content Retrieval** — Fetch page revisions, metadata, and internal links to understand the full context of any wiki entry
- **Category Exploration** — List all members of a specific category and see which categories a page belongs to
- **Site Monitoring** — Track recent changes across the wiki and inspect site-wide configurations and namespaces
- **User Context** — Retrieve information about the currently authenticated user and fetch necessary tokens for data-modifying actions

### How it works

1. Subscribe to this server
2. Enter your MediaWiki API URL (and optional Bot credentials)
3. Start querying your wiki from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Knowledge Managers** — instantly retrieve and organize information from internal wikis without manual navigation
- **Researchers** — search and extract content from Wikipedia or specialized wikis directly within their research workflow
- **Developers** — check documentation and site configurations straight from the code editor


## Available Tools
- **list_all_pages**: Enumerate all pages on the wiki
- **list_category_members**: List all pages in a category
- **create_account**: Requires a createaccount token fetched via get_tokens.

Create a new user account
- **edit_page**: Requires a CSRF token fetched via get_tokens.

Edit a wiki page
- **get_page_categories**: List categories on a page
- **get_page_info**: Get basic page information
- **get_page_links**: List all internal links on a page
- **get_page_revisions**: Get revision content or metadata for pages
- **list_recent_changes**: Enumerate recent wiki edits
- **search_pages**: Full-text search for pages
- **get_site_info**: Get general wiki settings and site info
- **get_tokens**: Fetch tokens for data-modifying actions
- **get_user_info**: Get information about the current user


## 💬 Prompt Examples

Here are some examples of how you can interact with the **MediaWiki** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Search the wiki for pages related to 'Artificial Intelligence'."

**🤖 AI Agent:**
> I've searched the wiki using `search_pages`. I found several relevant entries including 'Artificial Intelligence', 'Machine Learning', and 'Neural Networks'. Which one would you like to explore?

---

**👤 You:**
> "Get the latest content for the page 'Project_Roadmap'."

**🤖 AI Agent:**
> Using `get_page_revisions`, I've retrieved the latest content for 'Project_Roadmap'. It includes sections on Q3 goals, current blockers, and the team directory. Would you like a summary of the Q3 goals?

---

**👤 You:**
> "Show me the 5 most recent changes made to the wiki."

**🤖 AI Agent:**
> I've called `list_recent_changes` with a limit of 5. Recent edits include updates to 'API Documentation' by User:Admin and a new page 'Draft:Policy' created by User:Editor1. Would you like details on any of these?


## Installation & Usage

To install and use the **MediaWiki** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/mediawiki](https://vinkius.com/mcp/mediawiki)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
