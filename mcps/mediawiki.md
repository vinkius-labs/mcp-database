# MediaWiki MCP Server

Connect to any MediaWiki instance to search pages, read content, list categories, and track recent changes directly from your AI agent.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/mediawiki)

## Overview
**Category:** collaboration
**Tools Count:** 13

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


## Installation & Usage

To install and use the **MediaWiki** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/mediawiki](https://vinkius.com/mcp/mediawiki)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
