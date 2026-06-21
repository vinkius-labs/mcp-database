# Helpjuice MCP Server

Automate knowledge base management via Helpjuice — manage articles, categories, and analytics directly from any AI agent.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/helpjuice)

## Overview
**Category:** customer-support
**Tools Count:** 12

## Description
Connect your **Helpjuice** knowledge base to any AI agent and take full control of your internal and external documentation through natural conversation.

### What you can do

- **Article Management** — List all articles, retrieve full content, and create or update documentation directly from the chat.
- **Search Capabilities** — Perform text-based searches across your entire knowledge base to find answers quickly.
- **Content Organization** — List and manage categories to keep your documentation structured and easy to navigate.
- **Analytics Insights** — Retrieve engagement statistics for specific articles and monitor recent search trends.
- **User & Group Oversight** — Access lists of internal contributors and user groups defined for permissions.
- **Interactive Voting** — Record upvotes and downvotes for articles to track content helpfulness.

### How it works

1. Subscribe to this server
2. Enter your Helpjuice API Key and Subdomain
3. Start managing your knowledge base from Claude, Cursor, or any MCP-compatible client

No more manual navigating through complex CMS folders. Your AI assistant acts as a dedicated Knowledge Manager or Documentation Specialist.

### Who is this for?

- **Knowledge Managers** — instantly retrieve article statuses and identify missing or outdated documentation.
- **Support Teams** — check existing documentation and search for answers during customer interactions.
- **Content Creators** — automate the creation of draft articles and monitor engagement stats.


## Available Tools
- **create_article**: Requires a name/title. Pass body fields as a JSON string in "body_json".

Create a new article in the knowledge base
- **downvote_article**: Record a downvote for an article
- **get_article_details**: Get detailed content and metadata for a specific article
- **get_article_stats**: Get engagement statistics for a specific article
- **get_search_trends**: List recent search terms used by visitors
- **list_articles**: Useful for getting a birds-eye view of your content library.

List all articles in the Helpjuice knowledge base
- **list_categories**: List all categories in the knowledge base
- **list_kb_groups**: List user groups defined for permissions
- **list_kb_users**: List all internal users/authors in Helpjuice
- **search_kb**: Useful for finding existing answers to customer questions.

Search the knowledge base for articles matching a query
- **update_article**: Update an existing article
- **upvote_article**: Record an upvote for an article


## Installation & Usage

To install and use the **Helpjuice** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/helpjuice](https://vinkius.com/mcp/helpjuice)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
