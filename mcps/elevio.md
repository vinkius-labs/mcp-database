# Elevio MCP Server

Equip your AI agent to manage knowledge base articles, track categories, and monitor assistant modules via the Elevio API.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/elevio)

## Overview
**Category:** productivity
**Tools Count:** 10

## Description
Integrate **Elevio**, the leading customer education and knowledge management platform, directly into your AI workflow. Manage your knowledge base articles and categories, track real-time publishing statuses, monitor active assistant modules, and oversee your organizational learning content using natural language.

### What you can do

- **Article Oversight** — List and retrieve detailed information, HTML content, and publishing status for all your knowledge base articles.
- **Category Intelligence** — Monitor the category tree, resolving structural relationships and identifying empty categories requiring attention.
- **Module Management** — Access and monitor all Elevio assistant modules (support, search, tickets) and their activation statuses.
- **Knowledge Auditing** — Retrieve high-level summaries of article volumes, category coverage, and organizational content health.

### How it works

1. Connect the Elevio integration to your AI assistant.
2. Authorize using your Elevio API Key (found in your account settings).
3. Orchestrate your customer education and knowledge management through intuitive conversation.

### Who is this for?

- **Knowledge Managers** — Quickly check article publishing statuses and category coverage on the go.
- **Customer Success Teams** — Research specific article content and metadata via chat to assist customers.
- **Operations Teams** — Monitor content updates and organizational knowledge metadata instantly.


## Available Tools
- **get_elevio_account_metadata**: Retrieve metadata and limits for your Elevio account
- **get_article_details**: Get detailed settings and full content for a specific article
- **quick_content_health_audit**: Retrieve a high-level summary of article and category volumes
- **list_knowledge_articles**: List all articles in your Elevio knowledge base
- **list_knowledge_categories**: List all categories configured in your Elevio account
- **list_draft_knowledge_articles**: Identify articles that are currently in a "Draft" status
- **list_empty_knowledge_categories**: Identify categories that currently have no associated articles (mock logic)
- **list_active_modules**: List all Elevio assistant modules (e.g. support, search, tickets)
- **list_latest_article_updates**: Identify the most recently created or updated articles
- **search_knowledge_articles**: Search for articles using a title or keyword


## Installation & Usage

To install and use the **Elevio** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/elevio](https://vinkius.com/mcp/elevio)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
