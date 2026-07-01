# LanceDB (Serverless Vector DB) MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/lancedb-serverless-vector-db)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [loved-by-devs](../categories/loved-by-devs.md)

Manage vectorized data via LanceDB — perform similarity searches, create tables, and manage multi-modal embeddings.

## Description
Connect your **LanceDB Cloud** account to any AI agent and take full control of your serverless vector storage and RAG infrastructure through natural conversation.

### What you can do

- **Vector Orchestration** — List all vectorized tables and retrieve precise schema metadata, including tensor dimensions and vector topologies directly from your agent
- **Similarity Search** — Execute highly-optimized KNN (K-Nearest Neighbor) lookups to retrieve semantically related rows based on embedding array similarity
- **Dynamic Ingestion** — Insert new structured row payloads and vectors into existing tables, updating the underlying ANN index in real-time
- **Table Management** — Provision new columnar vector tables declaring specific Apache Arrow schemas and multi-dimensional layouts required for AI workloads
- **Database Audit** — Discover active table boundaries and verify storage configurations assigned to your serverless database instance securely
- **Resource Cleanup** — Irreversibly delete entire vector tables to maintain a clean and optimized data environment for your AI applications

### How it works

1. Subscribe to this server
2. Enter your LanceDB API URL, API Key, and Database Name
3. Start managing your vector storage from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **RAG Developers** — perform semantic searches and verify document retrieval results through natural conversation without manual Python scripts
- **Data Engineers** — provision and manage vector tables with strict Apache Arrow schemas to power multi-modal AI applications
- **AI Architects** — monitor vector topologies and audit storage usage across multiple serverless database instances efficiently


## Available Tools (6)
- **list_tables**: List all vectorized tables residing in LanceDB
- **get_table**: Get precise schema and metadata for a specific LanceDB table
- **vector_search**: Perform a highly-optimized KNN Vector similarity search
- **insert_rows**: Data dynamically updates the underlying ANN index.

Insert structured row payloads and vectors into a table
- **create_table**: Provision a new LanceDB table with a strict schema
- **delete_table**: Irreversibly vaporize an entire LanceDB vector table


## 💬 Prompt Examples

Here are some examples of how you can interact with the **LanceDB (Serverless Vector DB)** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all active tables in my LanceDB instance"

**🤖 AI Agent:**
> I've retrieved your vector tables. Active tables include 'customer_docs', 'product_embeddings', 'support_kb', and 'user_logs'. Which one would you like to inspect the schema for?

---

**👤 You:**
> "Perform a vector search in 'product_embeddings' for this vector: [0.1, 0.2, ...]"

**🤖 AI Agent:**
> Executing similarity search… I've found the 5 most relevant products. Highlights include 'Cloud-Native Sneakers' (Distance: 0.12), 'Edge Performance Runner' (Distance: 0.15), and 'Vector Pro Trainer' (Distance: 0.18). All results are now available in your workspace.

---

**👤 You:**
> "Show me the schema for the 'support_kb' table"

**🤖 AI Agent:**
> Schema for 'support_kb': The table has 4 columns: 'id' (String), 'text' (String), 'vector' (Float32, Dimensions: 1536), and 'metadata' (JSON). It is currently using an IVF-PQ index for optimized ANN lookups.


## ❓ FAQ

**Q: Can I perform a semantic similarity search using my agent?**
Yes. Use the `vector_search` tool by providing the target Table name and a JSON array of floating-point numbers representing your query embedding. Your agent will return the k-nearest rows from LanceDB based on semantic similarity.

**Q: How do I create a new table with a specific Apache Arrow schema?**
The `create_table` tool allows your agent to initialize a new columnar vector table. You just need to provide the desired Table name and a valid Apache Arrow schema mapping in JSON format defining dimensions and scalar fields.

**Q: Can my agent insert new embeddings directly into a LanceDB table?**
Absolutely. Use the `insert_rows` tool to persist new data rows containing native embeddings and arbitrary JSON metadata. Your agent will handle the payload delivery, and LanceDB will automatically update its ANN index.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/lancedb-serverless-vector-db](https://vinkius.com/mcp/lancedb-serverless-vector-db)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **LanceDB (Serverless Vector DB)** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `lancedb-serverless-vector-db` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **LanceDB (Serverless Vector DB)** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "lancedb-serverless-vector-db": {
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
