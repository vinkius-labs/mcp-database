# Elevio MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/elevio)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/elevio-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/elevio-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Equip your AI agent to manage knowledge base articles, track categories, and monitor assistant modules via the Elevio API.

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


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Elevio** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all published knowledge articles."

**🤖 AI Agent:**
> I've found 12 published articles, including 'Getting Started Guide' and 'Billing FAQ'. 3 articles are currently in draft status. Would you like to see the details for the Getting Started Guide?

---

**👤 You:**
> "Show me the categories in our knowledge base."

**🤖 AI Agent:**
> I've retrieved 5 categories, including 'Product Basics' (8 articles), 'Advanced Features' (4 articles), and 'Troubleshooting'. 'Troubleshooting' currently has 0 articles. Should I pull the list of draft articles to see if any belong there?

---

**👤 You:**
> "Search for articles about 'integrations'."

**🤖 AI Agent:**
> I've found 3 articles matching 'integrations': 'Setting up Slack', 'API Overview', and 'Webhooks Guide'. All are published. Would you like the full content for the API Overview?


## Installation & Usage

To install and use the **Elevio** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/elevio](https://vinkius.com/mcp/elevio)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
