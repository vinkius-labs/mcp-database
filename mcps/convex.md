# Convex MCP Server

Interact with your Convex backend directly—execute queries, mutations, and actions from any AI agent.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/convex)

## Overview
**Category:** loved-by-devs
**Tools Count:** 4

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


## Installation & Usage

To install and use the **Convex** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/convex](https://vinkius.com/mcp/convex)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
