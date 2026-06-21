# Notion MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/notion-extended)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/notion-extended-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/notion-extended-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [industry-titans](../categories/industry-titans.md)

Manage your Notion workspace, databases, and pages via AI.

## Description
Connect your Notion workspace to your AI agent. Search across databases, fetch page contents, update block properties, and create new knowledge entries directly from your chat without opening the Notion app.


## Available Tools
- **append_block_children**: Append child blocks to an existing block or page
- **create_page**: You must provide the parent object and properties (schema based on parent type).

Create a new page in Notion
- **get_me**: Get information about the current integration/bot
- **list_databases**: List all databases available to the integration
- **list_users**: List all users in the workspace
- **query_database**: Query a specific Notion database with filters and sorts
- **retrieve_block_children**: Retrieve child blocks of a specific block or page
- **retrieve_database**: Retrieve metadata for a specific database
- **retrieve_page**: Retrieve a specific Notion page by ID
- **retrieve_user**: Retrieve a specific user by ID
- **search**: Search for pages and databases by title
- **update_page**: Update properties of an existing Notion page


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Notion** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Search my Notion workspace for 'Q3 Roadmap'."

**🤖 AI Agent:**
> I found 2 pages mentioning 'Q3 Roadmap'. The primary document is at notion.so/q3-roadmap-xyz.

---

**👤 You:**
> "List all items in database 'DATABASE_ID' marked as 'In Progress'."

**🤖 AI Agent:**
> There are 4 tasks 'In Progress', including 'Redesign Header' and 'Optimize API calls'.

---

**👤 You:**
> "Create a new note titled 'Meeting Notes' under page 'PAGE_ID'."

**🤖 AI Agent:**
> Page 'Meeting Notes' created successfully.


## Installation & Usage

To install and use the **Notion** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/notion-extended](https://vinkius.com/mcp/notion-extended)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
