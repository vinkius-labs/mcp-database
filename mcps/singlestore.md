# SingleStore MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/singlestore)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/singlestore-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/singlestore-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [ai-frontier](../categories/ai-frontier.md)

Equip your AI agent to natively interact with your SingleStore database. Execute raw SQL queries, perform semantic vector searches, list workspaces, and audit billing directly from the terminal.

## Description
Grant your AI agent (like Claude or Cursor) absolute read-and-write sovereignty over your SingleStore infrastructure. The SingleStore MCP equips your LLM to act as a fully autonomous database administrator. Stop navigating external dashboards to check schema details or run complex search queries.

### What you can do

- **Execute SQL Queries** — Execute raw SQL natively from your AI agent using `execute_sql`.
- **Semantic Vector Search** — Perform semantic vector similarity searches natively against your data with `vector_search`.
- **Workspace & Billing Administration** — Survey your server clusters with `list_workspaces`, list databases with `list_databases`, and audit billing usage via `get_billing_usage`.


## Available Tools
- **execute_sql**: Use read-only SQL statements whenever possible.

Executes a SQL query on a SingleStore database
- **get_billing_usage**: Retrieves billing and usage metrics
- **list_databases**: Lists all databases within a specific workspace
- **list_organizations**: Lists organizations associated with the account
- **list_workspaces**: Lists all SingleStore workspaces
- **vector_search**: Performs a DOT_PRODUCT vector similarity search


## 💬 Prompt Examples

Here are some examples of how you can interact with the **SingleStore** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all my available workspaces."

**🤖 AI Agent:**
> I've successfully identified 2 distinct workspaces assigned to your account:
- **Workspace A** (ID: ws_ab12)
- **Workspace B** (ID: ws_ef56)

---

**👤 You:**
> "List all databases within workspace ID 1234, and then find the first 5 records in 'users_db'."

**🤖 AI Agent:**
> The databases configured for workspace 1234 includes 'users_db' and 'logs_db'. After executing a `SELECT * FROM users LIMIT 5`, here are the detailed user rows you requested.


## Installation & Usage

To install and use the **SingleStore** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/singlestore](https://vinkius.com/mcp/singlestore)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
