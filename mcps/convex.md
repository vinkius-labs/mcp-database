# Convex MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/convex)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/convex-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/convex-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [loved-by-devs](../categories/loved-by-devs.md)

Interact with your Convex backend directly—execute queries, mutations, and actions from any AI agent.

## Description
Connect your **Convex** deployment to any AI agent and manage your application's data and logic through natural conversation. This server allows you to interact with your real-time database and serverless functions without leaving your AI interface.

### What you can do

- **Data Fetching** — Execute read-only queries to retrieve documents and state from your Convex tables.
- **Transactional Updates** — Run mutations to modify data with full ACID guarantees directly from the agent.
- **Side Effects & APIs** — Trigger Convex actions for external API calls, heavy computation, or non-transactional logic.
- **Flexible Execution** — Call functions using standard colon notation or URL-style identifiers for maximum compatibility.

### How it works

1. Subscribe to this server
2. Enter your Convex Deployment URL (and optional Access Key)
3. Start querying and mutating your data from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Full-stack Developers** — Debug data, run migrations, or check state directly from your IDE or chat.
- **Product Managers** — Query live application metrics and user data using natural language without writing code.
- **Support Teams** — Inspect and update user records or trigger administrative actions through a secure AI interface.


## Available Tools
- **run_action**: Call a Convex action function
- **run_mutation**: Call a Convex mutation function
- **run_query**: Use this for fetching data.

Call a Convex query function
- **run_function**: g., "messages/list" instead of "messages:list").

Call a Convex function by its URL identifier


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Convex** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Run the Convex query 'messages:list' with no arguments."

**🤖 AI Agent:**
> I've executed the query. Here are the latest messages from your database: [List of message objects].

---

**👤 You:**
> "Call the mutation 'users:create' with the argument { "name": "Alice" }."

**🤖 AI Agent:**
> The mutation was successful. User 'Alice' has been created with ID 'jd7...'.

---

**👤 You:**
> "Execute the function 'tasks/get_all' using run_function."

**🤖 AI Agent:**
> I've called the function 'tasks/get_all'. It returned 12 active tasks.


## Installation & Usage

To install and use the **Convex** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/convex](https://vinkius.com/mcp/convex)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
