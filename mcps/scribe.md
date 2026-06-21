# Scribe MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/scribe)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/scribe-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/scribe-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Create step-by-step guides and SOPs automatically by recording your workflow and generating visual documentation instantly.

## Description
Connect your **Scribe** organization to any AI agent and access your process documentation library through natural conversation.

### What you can do

- **Full Search** — Search across all Scribes and Knowledge Pages simultaneously.
- **Filtered Search** — Search only guides or only pages for targeted results.
- **Team Scoping** — Find documents within a specific team for departmental queries.
- **Date Filtering** — Search by creation date range or get recent documents.
- **Teams** — List all teams and their documents for content auditing.
- **Statistics** — Get an overview of your documentation footprint.

### How it works

1. Subscribe to this server
2. Enter your Scribe API key (Enterprise Grid or Global plan required)
3. Start searching documentation from Claude, Cursor, or any MCP client

### Who is this for?

- **Knowledge Managers** — quickly find and audit process documentation.
- **Support Teams** — retrieve step-by-step guides for customer assistance.
- **Operations Leads** — monitor documentation activity across teams.


## Available Tools
- **check_scribe_status**: Verify Scribe API connectivity
- **get_documentation_stats**: Get documentation statistics
- **get_team_documents**: Useful for auditing team documentation.

Get all documents for a specific team
- **list_teams**: List all teams in your Scribe organization
- **search_documents**: Search across all Scribes and Pages
- **search_by_date**: Dates should be in YYYY-MM-DD format.

Search documents by creation date range
- **search_by_team**: Search documents within a specific team
- **search_pages**: Search only Knowledge Pages
- **get_recent_documents**: Get documents created in the last 30 days
- **search_scribes**: Search only Scribe guides


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Scribe** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Search for all documentation about 'onboarding'."

**🤖 AI Agent:**
> Found 12 documents matching 'onboarding': 8 Scribe guides and 4 Knowledge Pages. The most relevant is 'New Employee Onboarding Checklist' (Scribe, HR team).

---

**👤 You:**
> "List all teams in our Scribe organization."

**🤖 AI Agent:**
> Your Scribe organization has 5 teams: Engineering (42 docs), Sales (28 docs), HR (19 docs), Marketing (15 docs), and Customer Support (31 docs).

---

**👤 You:**
> "What documents were created in the last 30 days?"

**🤖 AI Agent:**
> 7 documents were created in the last 30 days: 4 Scribes including 'API Integration Guide' and 'Deployment Checklist', plus 3 Knowledge Pages.


## Installation & Usage

To install and use the **Scribe** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/scribe](https://vinkius.com/mcp/scribe)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
