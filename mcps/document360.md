# Document360 MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/document360)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/document360-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/document360-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [collaboration](../categories/collaboration.md)

Manage knowledge bases via Document360 — list project versions, handle categories and articles, search content, and track analytics directly from any AI agent.

## Description
Connect your **Document360** portal to any AI agent and take full control of your enterprise knowledge base and documentation workflows through natural conversation.

### What you can do

- **Project & Version Navigation** — Analyze specific localized versions mapping exactly which documentation segments exist globally across your portal
- **Categorical Orchestration** — Extract explicitly attached categories bounding physical groupings active inside specific project versions
- **Article Management** — Perform structural extraction of explicit document lists and retrieve raw content texts securely via unique IDs
- **Semantic Search** — Execute immediate semantic queries discovering strictly mapped textual responses active inside your knowledge base
- **Team & Author Oversight** — Retrieve complex RBAC profiles outlining registered authors physically mapped against workspace boundaries
- **Analytics & Traffic Auditing** — Read available metrics exposing explicit traffic ranges and visitor interaction stamps to monitor KB performance

### How it works

1. Subscribe to this server
2. Enter your Document360 API Key (found in Settings > Knowledge base portal > API Tokens)
3. Start managing your knowledge base from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Technical Writers & Editors** — search for articles and manage categories without navigating the web portal
- **Product Managers** — monitor knowledge base analytics and audit team contributions using natural language
- **Customer Support** — quickly search for documentation and retrieve article content to resolve customer inquiries
- **Developers** — test and debug knowledge base integrations and verify documentation schemas directly from the IDE


## Available Tools
- **list_projects**: List project versions
- **list_categories**: List categories in a version
- **list_articles**: List articles in a category
- **get_article**: Get article content
- **search**: Search articles
- **list_team**: List team accounts
- **analytics**: Get knowledge base analytics


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Document360** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all versions for my Document360 project"

**🤖 AI Agent:**
> I found 3 project versions: 'V1.0 (Main)', 'V2.0-Beta', and 'Internal-Docs'. Which version would you like to explore for categories?

---

**👤 You:**
> "Search for 'Single Sign On setup' in my KB"

**🤖 AI Agent:**
> Searching for 'Single Sign On setup'... I found 2 matching articles: 'SSO Configuration Guide' (ID: art_123) and 'Troubleshooting Login Issues' (ID: art_456). Would you like to read the full content of the guide?

---

**👤 You:**
> "Show me knowledge base analytics from the last 30 days"

**🤖 AI Agent:**
> Retrieving analytics for the last 30 days... Your KB had 1,200 unique visitors and 4,500 pageviews. Most visited article: 'API Quickstart'. I can provide a daily breakdown of this traffic.


## Installation & Usage

To install and use the **Document360** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/document360](https://vinkius.com/mcp/document360)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
