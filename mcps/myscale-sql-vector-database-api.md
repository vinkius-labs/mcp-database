# MyScale (SQL Vector Database API) MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/myscale-sql-vector-database-api)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [databases](../categories/databases.md)

Manage MyScale vector databases via SQL — execute queries, perform vector searches, and manage indices directly from any AI agent.

## Description
Connect your **MyScale** cluster to any AI agent to manage high-performance vector data using familiar SQL syntax. MyScale combines the power of ClickHouse with advanced vector search capabilities.

### What you can do

- **SQL Execution** — Run arbitrary SQL queries including SELECT, INSERT, and ALTER directly on your cluster via `execute_sql_query`.
- **Vector Search** — Perform similarity searches using the `vector_search` tool which automatically handles distance functions and SQL construction.
- **Index Management** — Create and monitor specialized vector indices (MSTG, ScaNN, HNSW) using `create_vector_index` and `check_index_status`.
- **Schema Control** — Quickly set up new environments with `create_vector_table`, defining dimensions and constraints through natural language.
- **Connectivity Checks** — Instantly verify your database status and credentials with `ping_cluster`.

### How it works

1. Subscribe to this server
2. Enter your MyScale Cluster URL, Username, and Password
3. Start managing your vector data from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **AI Engineers** — test vector search parameters and inspect data distributions without leaving the chat
- **Data Scientists** — manage RAG (Retrieval-Augmented Generation) backends and monitor index health in real-time
- **Backend Developers** — perform database maintenance and schema updates using natural language commands


## Available Tools (6)
- **create_vector_table**: Create a new table with a vector column
- **execute_sql_query**: For SELECT queries, FORMAT JSON is automatically appended.

Execute an arbitrary SQL query on MyScale
- **vector_search**: Automatically constructs the SQL query.

Perform a vector similarity search
- **check_index_status**: vector_indices table to monitor the build status of vector indices (Built, InProgress, Error).

Check the status of vector indices
- **create_vector_index**: ADD VECTOR INDEX statement.

Create a vector index on a table
- **ping_cluster**: Check MyScale cluster connectivity


## 💬 Prompt Examples

Here are some examples of how you can interact with the **MyScale (SQL Vector Database API)** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Check if my MyScale cluster is reachable and credentials are correct."

**🤖 AI Agent:**
> I've pinged the cluster using `ping_cluster`. The connection is successful and the database is responding normally.

---

**👤 You:**
> "Search the 'articles' table for the top 5 matches for vector [0.12, -0.05, 0.33] where author is 'John'."

**🤖 AI Agent:**
> I'm executing a `vector_search` on the 'articles' table. I've applied the filter for author 'John' and limited the results to 5. Here are the most relevant documents found...

---

**👤 You:**
> "Create a new vector table called 'product_embeddings' with 1536 dimensions and an 'id' column."

**🤖 AI Agent:**
> I've initiated the `create_vector_table` tool for 'product_embeddings'. The table has been created with a 1536-dimension float array constraint and an additional 'id' column using the MergeTree engine.


## ❓ FAQ

**Q: How can I check if my vector index has finished building?**
Use the `check_index_status` tool. It queries the system tables to show you the current status (Built, InProgress, or Error) for all vector indices in your cluster.

**Q: Can I perform a vector search with metadata filtering?**
Yes! The `vector_search` tool includes an optional `filter` parameter where you can provide a SQL WHERE clause (e.g., "category = 'science'") to restrict your search results.

**Q: What SQL commands are supported by the execute tool?**
The `execute_sql_query` tool supports standard MyScale/ClickHouse SQL, including SELECT, CREATE, ALTER, and INSERT. For SELECT queries, it automatically formats the output as JSON for the agent.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/myscale-sql-vector-database-api](https://vinkius.com/mcp/myscale-sql-vector-database-api)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **MyScale (SQL Vector Database API)** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `myscale-sql-vector-database-api` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **MyScale (SQL Vector Database API)** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "myscale-sql-vector-database-api": {
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
