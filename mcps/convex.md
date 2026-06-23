# Convex MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/convex)
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


## Available Tools (4)
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


## ❓ FAQ

**Q: What is the difference between run_query and run_mutation?**
Use `run_query` for read-only operations that fetch data. Use `run_mutation` when you need to write, update, or delete data transactionally in your database.

**Q: Can I call external APIs using this server?**
Yes, by using the `run_action` tool. Actions in Convex are designed for side effects like calling third-party APIs or performing long-running tasks.

**Q: How do I reference functions in subdirectories?**
You can use `run_query` with colon notation (e.g., 'folder/file:function') or use `run_function` which accepts URL-style identifiers with slashes.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/convex](https://vinkius.com/mcp/convex)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Convex** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `convex` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Convex** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "convex": {
      "url": "https://edge.vinkius.com/[TOKEN]/mcp"
    }
  }
}
```

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
