# AddSearch MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/addsearch)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/addsearch-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/addsearch-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [developer-tools](../categories/developer-tools.md)

Equip your AI agent with AddSearch to query your indexed site content, push new documents, and retrieve search analytics instantly.

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


## 💬 Prompt Examples

Here are some examples of how you can interact with the **AddSearch** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Show me the top search queries that resulted in 0 hits."

**🤖 AI Agent:**
> Based on the recent stats, the top zero-result queries are:
1. 'internship 2026' - 142 searches
2. 'sso integration' - 89 searches
3. 'gdpr compliance pdf' - 55 searches
These topics might be worth adding to your content backlog.

---

**👤 You:**
> "Search my site for "pricing updates" filtered by category=news."

**🤖 AI Agent:**
> Found 3 results for "pricing updates" in the 'news' category:
1. Q1 Pricing Announcement (Score: 0.95)
2. Subscriptions Fact-sheet (Score: 0.81)
3. Partner Network Updates (Score: 0.72)
Would you like the full URL and snippet for the top result?

---

**👤 You:**
> "Test the auto-suggest for the prefix "shoe"."

**🤖 AI Agent:**
> The auto-suggest API returns these completions for "shoe":
- shoes for running
- shoelaces
- shoe sizing guide
The system confirms the index is correctly populating typed suggestions for this entity.


## Installation & Usage

To install and use the **AddSearch** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/addsearch](https://vinkius.com/mcp/addsearch)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
