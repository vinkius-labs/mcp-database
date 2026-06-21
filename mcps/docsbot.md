# DocsBot MCP Server

Equip your AI agent to manage AI-powered knowledge bases, track sources, and query your bots via the DocsBot API.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/docsbot)

## Overview
**Category:** customer-support
**Tools Count:** 10

## Description
Integrate **DocsBot**, the AI-powered knowledge base platform, directly into your AI workflow. Manage your custom AI bots, track their data sources (URLs, PDFs, documents), monitor indexing status, and query your bots directly using natural language.

### What you can do

- **Bot Oversight** — List and retrieve detailed configuration and metadata for all the AI bots in your team.
- **Knowledge Management** — Monitor data sources used to train your bots and track their last indexing timestamps.
- **Bot Interaction** — Query your bots directly via the agent to retrieve AI-generated answers based on your knowledge base.
- **Analytics & Logs** — Access technical logs of recent bot interactions, including questions and generated answers.

### How it works

1. Connect the DocsBot integration to your AI assistant.
2. Authorize using your DocsBot API Key (found in your account settings).
3. Orchestrate your AI knowledge bases and queries through intuitive conversation.

### Who is this for?

- **Support Teams** — Quickly query documentation bots to assist with customer resolution via chat.
- **Knowledge Managers** — Monitor bot source coverage and indexing status on the go.
- **Product Teams** — Audit bot interaction logs to identify common user questions and content gaps.


## Available Tools
- **ask_bot_question**: Ask a technical question to a specific DocsBot and retrieve an AI-generated answer
- **get_docsbot_account_metadata**: Retrieve metadata for the current authenticated user
- **get_bot_knowledge_summary**: Retrieve a high-level summary of the knowledge base size and source count
- **get_bot_details**: Get detailed settings and information for a specific bot
- **list_recently_indexed_bots**: Identify bots that have had their knowledge base updated recently (mock logic)
- **list_bot_interaction_logs**: List recent questions and answers handled by a specific bot
- **list_team_bots**: List all AI bots configured within a specific team
- **list_bot_knowledge_sources**: List all data sources (URL, PDF, etc.) used to train a specific bot
- **list_docsbot_teams**: List all teams you are a member of in DocsBot
- **search_bot_sources**: Search for specific knowledge sources by name keyword


## Installation & Usage

To install and use the **DocsBot** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/docsbot](https://vinkius.com/mcp/docsbot)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
