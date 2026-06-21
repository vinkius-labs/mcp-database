# Couchbase (Vector & NoSQL) MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/couchbase-vector-nosql)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [databases](../categories/databases.md)

Manage vector search and NoSQL via Couchbase — execute N1QL queries, perform KNN vector searches, and audit documents directly from any AI agent.

## Description
Connect your **Couchbase** (Capella or self-hosted) cluster to any AI agent and take full control of your NoSQL and vector data through natural conversation.

### What you can do

- **Vector Search (KNN)** — Execute direct searches mapping AI embeddings to locate textual similarities using native vector indices
- **N1QL SQL-for-JSON** — Push absolute explicit querying using N1QL (SQL for Couchbase) to retrieve complex JSON structures across your buckets
- **Document CRUD** — Fetch elaborate internal properties and retrieve exact Data maps from specific collections using unique document keys
- **Full-Text Search (FTS)** — Perform structural text-based extraction matching query strings across advanced FTS search indexes
- **Schema Navigation** — Identify bounded routing spaces including Buckets, Scopes, and Collections to understand your data organization
- **Index Auditing** — Enumerate explicitly registered Search Indexes and verify vector definitions and cluster configurations

### How it works

1. Subscribe to this server
2. Enter your Couchbase URL, Database Username, and Database Password
3. Start querying your NoSQL and vector data from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **AI Developers** — test and debug vector similarity searches and semantic matching for RAG applications
- **Data Architects** — audit NoSQL data structures and verify collection organization across environments
- **Database Administrators** — monitor search indexes and execute N1QL queries to verify data consistency
- **Product Teams** — quickly prototype search features and audit JSON document schemas through natural language


## Available Tools (7)
- **list_buckets**: Identify bounded routing spaces inside the Headless Couchbase DB
- **list_scopes**: Retrieve explicit UX logging tracing explicit Scope and Collection Object limits
- **list_indexes**: Enumerate explicitly attached structured rules exporting active Search Indexes
- **execute_n1ql_query**: Provision a highly-available JSON Payload generating generic N1QL constraints
- **vector_search**: Execute static listing mapping structural KNN Vector similarities via Index
- **get_document**: Fetch elaborate internal mapped properties limiting Couchbase KV documents
- **fts_search**: Perform structural text-based extraction matching asynchronous Content Trees


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Couchbase (Vector & NoSQL)** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all search indexes in my cluster"

**🤖 AI Agent:**
> I found 3 search indexes: 'vector-index-v1', 'fts-content-search', and 'customer-lookup'. Which one would you like to use for a search?

---

**👤 You:**
> "Find the top 3 similar products using this vector: [0.12, -0.5, 0.88]"

**🤖 AI Agent:**
> Vector search complete! I found 3 matches in 'vector-index-v1'. The top result is 'Wireless Pro Headphones' with a similarity score of 0.98. Would you like to see the full document metadata?

---

**👤 You:**
> "Run N1QL query: 'SELECT name, price FROM `travel-sample` WHERE price < 100 LIMIT 5'"

**🤖 AI Agent:**
> Query executed successfully! I've retrieved 5 items from 'travel-sample'. Results include 'Economy Flight' ($85) and 'Local Tour' ($45). I have the full JSON response if you need more details.


## ❓ FAQ

**Q: Can my agent perform K-Nearest Neighbor (KNN) vector searches in Couchbase?**
Yes. Provide the search index name, the vector embedding array, and the number of results (k). The agent uses Couchbase's native vector capabilities to locate the most semantically similar documents in your cluster.

**Q: How do I execute a N1QL query through the agent?**
Use the 'execute_n1ql_query' tool and provide your SQL-like statement. The agent will fetch the structural JSON blocks directly from Couchbase, allowing you to perform complex data retrieval using familiar SQL syntax.

**Q: Can I search documents using full-text query logic?**
Absolutely. The 'fts_search' tool leverages Couchbase's Full-Text Search (FTS) engine. Provide an index name and a boolean query string to perform structural text-based extraction across your document trees.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/couchbase-vector-nosql](https://vinkius.com/mcp/couchbase-vector-nosql)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Couchbase (Vector & NoSQL)** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `couchbase-vector-nosql` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Couchbase (Vector & NoSQL)** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "couchbase-vector-nosql": {
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
