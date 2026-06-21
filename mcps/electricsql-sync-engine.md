# ElectricSQL (Sync Engine) MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/electricsql-sync-engine)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [developer-tools](../categories/developer-tools.md)

Sync Postgres data to your AI agent in real-time using ElectricSQL's HTTP Sync API — fetch shapes, stream updates, and query subsets.

## Description
Connect your **ElectricSQL** sync engine to any AI agent to stream data directly from Postgres into your conversation context. This server leverages the Electric HTTP Sync API to fetch 'shapes' of data efficiently.

### What you can do

- **Real-time Sync** — Fetch data from Postgres tables with support for initial snapshots and incremental updates using log offsets.
- **Shape Management** — Define specific subsets of data (shapes) using SQL-like WHERE clauses and precise column selection.
- **Live Streaming** — Enable long-polling or Server-Sent Events (SSE) to keep your agent updated as data changes in the database.
- **Complex Filtering** — Use POST-based subset snapshots to handle complex WHERE clauses without hitting URL length limits.
- **Pagination & Limits** — Efficiently browse large datasets with built-in limit, offset_rows, and order_by support.

### How it works

1. Subscribe to this server
2. Provide your Electric Service URL (e.g., your local or cloud Electric endpoint)
3. Start querying your Postgres data directly from Claude, Cursor, or any MCP client

### Who is this for?

- **Developers** — build AI-powered tools that need live access to application data without complex backend plumbing.
- **Data Engineers** — inspect and sync specific database 'shapes' for analysis or debugging via natural language.
- **Product Teams** — monitor real-time system state or user activity directly within the AI chat interface.


## Available Tools
- **get_shape**: Use offset=-1 for initial sync.

Sync a shape of data out of Postgres via GET
- **post_shape**: Sync a shape of data out of Postgres via POST (Subset Snapshots)


## 💬 Prompt Examples

Here are some examples of how you can interact with the **ElectricSQL (Sync Engine)** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Sync the 'public.items' table from the beginning using get_shape."

**🤖 AI Agent:**
> I'm initiating the initial sync for 'public.items' with offset -1. I've retrieved 150 rows. The shape handle is 'items-handle-xyz'. Would you like to see the data or wait for live updates?

---

**👤 You:**
> "Use post_shape to get the first 10 rows of 'orders' where status is 'pending', ordered by date."

**🤖 AI Agent:**
> Querying 'orders' via POST... I found 10 pending orders. The most recent is Order #502 from today. I've used the limit and order_by parameters as requested.

---

**👤 You:**
> "Start a live sync for the 'messages' table to watch for new entries."

**🤖 AI Agent:**
> Live sync enabled for 'messages'. I am now long-polling the ElectricSQL engine. I will notify you immediately when new rows are detected in the database.


## ❓ FAQ

**Q: How do I perform an initial sync of a database table?**
Use the `get_shape` tool and set the `offset` parameter to `-1`. This triggers ElectricSQL to send the full initial snapshot of the specified table.

**Q: What should I do if my SQL WHERE clause is too long for a standard URL?**
You should use the `post_shape` tool. It sends the filtering criteria in the request body, which prevents '414 Request-URI Too Long' errors when using complex logic.

**Q: Can the AI agent receive updates automatically when data changes in Postgres?**
Yes! By setting the `live` parameter to `true` in `get_shape`, the agent can establish a long-polling connection to stream incremental changes as they happen.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/electricsql-sync-engine](https://vinkius.com/mcp/electricsql-sync-engine)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **ElectricSQL (Sync Engine)** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `electricsql-sync-engine` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **ElectricSQL (Sync Engine)** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "electricsql-sync-engine": {
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
