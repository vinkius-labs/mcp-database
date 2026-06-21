# AddSearch MCP Server

Equip your AI agent with AddSearch to query your indexed site content, push new documents, and retrieve search analytics instantly.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/addsearch)

## Overview
**Category:** developer-tools
**Tools Count:** 10

## Description
Connect your **AddSearch** account to your AI agent and turn your site's search index into an interactive, manageable database. Perfect for content teams and developers who need to audit site search performance without opening dashboards.

### What you can do

- **Deep Search** — Query your indexed content using natural language, apply custom field filters (e.g. "category=shoes"), or sort by custom variables
- **Document Management** — List all indexed pages, import new content directly via JSON, or permanently delete outdated documents from the index
- **Search Analytics** — Retrieve live statistics on user queries, identifying top searches, zero-result queries, and click-through rates
- **Frontend Emulation** — Test your auto-suggestions and pagination just like a real user interacting with your search bar

### How it works

1. Subscribe to this server
2. Enter your AddSearch Site Key and optional Secret Key
3. Start managing your search index from Claude, Cursor, or any MCP-compatible environment

### Who is this for?

- **Content Managers** — ask your agent what the most popular zero-result queries were this week to identify content gaps
- **Developers** — debug the search index by looking up a specific URL's metadata or manually pushing a JSON document fix in seconds
- **E-Commerce Teams** — query specific product categories and verify if the relevance ranking is displaying the right inventory


## Available Tools
- **delete_document**: Requires Secret Key.

Permanently delete a document
- **search_filtered**: g., "category=shoes", "brand=nike").

Search indexed content by custom field
- **index_document**: Requires Secret Key.

Add or update an indexed document
- **list_documents**: Requires Secret Key.

List all indexed documents
- **search_pagination**: Retrieve a specific page of search results
- **search_keyword**: Search indexed content by keyword
- **search_sorted**: Search indexed content with custom sort
- **stats_clicks**: Requires Secret Key.

Retrieve click-through analytics
- **stats_queries**: Requires Secret Key.

Retrieve search query analytics
- **autosuggest**: Get autocomplete suggestions


## Installation & Usage

To install and use the **AddSearch** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/addsearch](https://vinkius.com/mcp/addsearch)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
