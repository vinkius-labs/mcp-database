# ToolJet MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/tooljet)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/tooljet-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/tooljet-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [developer-tools](../categories/developer-tools.md)

Manage ToolJet databases and trigger workflows directly from your AI agent—query tables, insert data, and automate processes.

## Description
Connect your **ToolJet** workspace to any AI agent to interact with your internal databases and automate business logic through natural language.

### What you can do

- **Database Exploration** — List all available tables within your ToolJet Database to understand your data structure.
- **Advanced Querying** — Execute SQL SELECT queries on your tables to retrieve specific records, filter data, and generate insights.
- **Data Entry** — Insert new rows into your database tables directly from the chat interface using structured JSON data.
- **Workflow Automation** — Trigger complex ToolJet Workflows via webhooks, passing custom payloads to start automated business processes.

### How it works

1. Subscribe to this server
2. Enter your ToolJet API Key (and optional Host URL for self-hosted instances)
3. Start managing your internal data and workflows from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Developers** — Quickly query internal databases or trigger CI/CD workflows without leaving the code editor.
- **Operations Teams** — Update records or start business processes using natural language instead of complex UIs.
- **Data Analysts** — Explore ToolJet Database tables and run ad-hoc queries to verify data integrity.


## Available Tools
- **insert_row**: Insert a new row into a ToolJet Database table
- **list_tables**: List all tables in the ToolJet Database
- **query_table**: Use this for reading data (SELECT).

Perform a SQL query on a ToolJet Database table
- **trigger_workflow**: Trigger a ToolJet Workflow via Webhook


## 💬 Prompt Examples

Here are some examples of how you can interact with the **ToolJet** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all the tables available in my ToolJet Database."

**🤖 AI Agent:**
> I've retrieved the tables for your workspace. You have 3 tables: 'inventory', 'orders', and 'customers'.

---

**👤 You:**
> "Run a query to find all orders with a status of 'pending' in organization 'org_123'."

**🤖 AI Agent:**
> Executing `query_table`... I found 2 pending orders: Order #501 (Total: $120) and Order #505 (Total: $45).

---

**👤 You:**
> "Trigger the workflow 'wf_987' with the payload {"user_id": "123", "action": "reset"}."

**🤖 AI Agent:**
> The workflow 'wf_987' has been triggered successfully. The response from ToolJet indicates the process has started.


## Installation & Usage

To install and use the **ToolJet** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/tooljet](https://vinkius.com/mcp/tooljet)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
