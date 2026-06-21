# Oracle Vector DB MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/oracle-vector-db)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [industry-titans](../categories/industry-titans.md)

Run vector similarity searches on Oracle 23ai — execute VECTOR_DISTANCE queries, inspect schemas, list vector indexes, and query tables from any AI agent.

## Description
Bring your **Oracle Database 23ai** vector capabilities directly into your AI agent workflow. Run VECTOR_DISTANCE similarity searches, inspect table schemas, execute SQL queries, and manage vector indexes — all through natural conversation.

### What you can do

- **Vector Similarity Search** — Execute native Oracle 23ai VECTOR_DISTANCE queries with cosine or Euclidean metrics against any table with VECTOR columns
- **Schema Inspection** — List all tables in your schema and describe column types, spotting VECTOR-enabled columns for embedding storage
- **SQL Execution** — Run arbitrary SQL queries against Oracle via ORDS for ad-hoc analysis and data retrieval
- **Vector Index Management** — List all HNSW and IVF vector indexes instantiated across your tables
- **Table Statistics** — Get row counts and optimizer stats for capacity planning and query performance tuning
- **Version Check** — Verify your Oracle runtime version to confirm 23ai vector feature compatibility

### How it works

1. Subscribe to this server
2. Enter your Oracle ORDS URL, Schema, Username, and Password
3. Start querying your vector store from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Enterprise data teams** — run vector searches against production Oracle databases without context-switching to SQL Developer
- **ML engineers** — test embedding queries on Oracle 23ai's native vector engine during RAG pipeline development
- **DBAs** — inspect vector indexes, table stats, and schema configurations through conversation


## Available Tools (7)
- **list_tables**: List accessible tables in the current Oracle schema
- **describe_table**: Describe table columns and explicit data types including VECTORs
- **execute_sql_query**: WARNING: Output payload size is inherently limited, restrict rows fetched (FETCH FIRST 100 ROWS ONLY) to ensure stability.

Execute arbitrary SQL query against the Oracle runtime via ORDS
- **vector_search**: 1, -0.4, 0.5]` against a strict `VECTOR` column natively inside Oracle DB, sorting and fetching the nearest neighbors.

Execute Vector similarity search via Oracle 23ai native VECTOR_DISTANCE
- **list_vector_indexes**: List specialized AI Vector search indexes (HNSW, IVF) instantiated
- **table_stats**: Get table cardinality and optimizer statistics
- **get_database_version**: Get exact Oracle DB Runtime version banner


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Oracle Vector DB** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Show me all tables in my schema that have VECTOR columns."

**🤖 AI Agent:**
> Found 3 tables with VECTOR columns. 1) DOCUMENTS — columns: ID (NUMBER), CONTENT (CLOB), EMBEDDING (VECTOR(1536)), 82,400 rows. 2) PRODUCTS — columns: ID, NAME, FEATURES_VECTOR (VECTOR(768)), 5,200 rows. 3) FAQ_ENTRIES — columns: ID, QUESTION, ANSWER_EMBEDDING (VECTOR(384)), 1,100 rows. Want me to search one?

---

**👤 You:**
> "Find the 5 most similar documents to this embedding using cosine distance."

**🤖 AI Agent:**
> Top 5 results from DOCUMENTS table (cosine): 1) Doc #4521 — 'API Rate Limits Overview', distance: 0.034. 2) Doc #1892 — 'Authentication Flow Guide', distance: 0.089. 3) Doc #7301 — 'Error Handling Reference', distance: 0.112. 4) Doc #2244 — 'SDK Quickstart', distance: 0.145. 5) Doc #9010 — 'Webhook Setup', distance: 0.178.

---

**👤 You:**
> "What version of Oracle is running and does it support vectors?"

**🤖 AI Agent:**
> Oracle Database 23ai (23.4.0.24.05) — Free tier. Vector features: fully supported. VECTOR data type: available. VECTOR_DISTANCE function: available. HNSW index support: yes. Your instance is ready for vector similarity search operations.


## ❓ FAQ

**Q: Does it work with Oracle Autonomous Database?**
Yes. Oracle Autonomous Database on OCI has ORDS enabled by default. Use the ORDS URL from your ADB instance (e.g., https://xxxxx.adb.us-ashburn-1.oraclecloudapps.com/ords), your schema name (typically ADMIN), and the admin credentials. The VECTOR type is available on all 23ai-compatible instances.

**Q: Can I run arbitrary SQL — not just vector searches?**
Yes. The execute_sql_query tool accepts any valid Oracle SQL statement and returns results through ORDS. Add FETCH FIRST N ROWS ONLY to keep payloads manageable. This makes the agent useful for relational queries too, not just vector operations.

**Q: Which distance metrics are available for vector search?**
Oracle 23ai supports COSINE and EUCLIDEAN (L2) distance metrics natively via VECTOR_DISTANCE. Specify the metric when running a search — cosine is recommended for most text embedding use cases, while L2 works better for image or audio embeddings.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/oracle-vector-db](https://vinkius.com/mcp/oracle-vector-db)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Oracle Vector DB** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `oracle-vector-db` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Oracle Vector DB** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "oracle-vector-db": {
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
