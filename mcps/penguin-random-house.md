# Penguin Random House MCP Server

Access the global Penguin Random House catalog—search for authors, titles, works, and literary categories directly from your AI agent.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/penguin-random-house)

## Overview
**Category:** knowledge-management
**Tools Count:** 13

## Description
Connect the **Penguin Random House** Open Service to your AI agent to explore one of the world's largest trade book catalogs. Retrieve detailed metadata for millions of titles, authors, and literary events through natural conversation.

### What you can do

- **Author Discovery** — List authors, illustrators, and narrators. Filter by tour status or last initial to find specific contributors.
- **Title & ISBN Lookup** — Fetch complete metadata for specific book editions using ISBNs, including format details, sale dates, and award status.
- **Work Grouping** — Access 'Works' which group different formats (hardcover, ebook, audio) of the same book under a single identifier for better organization.
- **Category Hierarchy** — Explore the complex tree of book categories and genres to discover new content or classify existing lists.
- **Event Tracking** — List upcoming author events and tours to stay updated on the literary world.

### How it works

1. Subscribe to this server
2. Enter your Penguin Random House API Key
3. Start querying the catalog from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Content Creators & Researchers** — quickly verify book details, author bios, and publication dates without manual web searches.
- **Developers & Librarians** — integrate professional-grade book metadata into workflows or personal databases.
- **Book Enthusiasts** — find upcoming releases, award-winning titles, and author tour dates through simple chat.


## Available Tools
- **get_author**: Get details for a specific author
- **get_category_hierarchy**: Get category hierarchy view
- **get_series**: Get details for a specific series
- **get_title**: Get details for a specific title by ISBN
- **get_work**: Get details for a specific work
- **list_authors**: Can be scoped to a domain and filtered by tour status or last initial.

List authors, illustrators, narrators, and contributors
- **list_categories**: List book categories
- **list_events**: List author events (signings, talks)
- **list_series**: List book series
- **list_titles**: Can be scoped to a domain and filtered by format, sale dates, etc.

List book editions identified by ISBN
- **list_works**: A work groups different formats (hardcover, ebook, etc.) under a single ID.

List works (groups of different formats of the same book)
- **predictive_search**: Predictive search for autocomplete
- **search**: Responses include a facets array for filtering results.

Full-text search powered by Apache Solr


## Installation & Usage

To install and use the **Penguin Random House** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/penguin-random-house](https://vinkius.com/mcp/penguin-random-house)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
