# Helpjuice MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/helpjuice)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/helpjuice-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/helpjuice-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [customer-support](../categories/customer-support.md)

Automate knowledge base management via Helpjuice — manage articles, categories, and analytics directly from any AI agent.

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


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Helpjuice** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Find articles related to 'OAuth integration'."

**🤖 AI Agent:**
> Searching knowledge base... I found 3 relevant articles: 'Setting up OAuth 2.0', 'API Authentication Guide', and 'Troubleshooting Connection Issues'. Would you like the full content for the 'Setting up OAuth 2.0' article?

---

**👤 You:**
> "List all categories in my knowledge base."

**🤖 AI Agent:**
> I've retrieved your categories. You have 5 main sections: 'Getting Started', 'User Guides', 'Developer API', 'Release Notes', and 'FAQs'. Should I list the articles inside the 'Developer API' category?

---

**👤 You:**
> "Show me the engagement stats for article ID 1021."

**🤖 AI Agent:**
> Retrieving analytics... Article ID 1021 ('Advanced Filtering') has had 450 views and 32 upvotes this month. It is currently one of your top-performing pieces of documentation. Would you like to see recent search terms that led users here?


## Installation & Usage

To install and use the **Helpjuice** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/helpjuice](https://vinkius.com/mcp/helpjuice)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
