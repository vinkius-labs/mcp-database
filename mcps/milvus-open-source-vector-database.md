# Milvus (Open-Source Vector Database) MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/milvus-open-source-vector-database)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [loved-by-devs](../categories/loved-by-devs.md)

Manage vector storage via Milvus — perform ANN searches, query scalar entities, and audit collections.

## Description
Connect your **Milvus** instance to any AI agent and take full control of your high-performance vector search, embedding storage, and scalar data management through natural conversation.

### What you can do

- **Vector Search Orchestration** — Execute Approximate Nearest Neighbor (ANN) searches against your collections by providing raw embedding vectors to retrieve semantically relevant matches directly from your agent
- **Scalar Query Filters** — Use sophisticated scalar expressions to filter entities by structured fields (e.g., tags, IDs, dates) alongside your vector search for precise data retrieval
- **Collection Lifecycle Audit** — List all managed vector collections and retrieve detailed schema definitions, including dimensions, primary keys, and index types natively
- **Performance Statistics** — Extract real-time metrics for your collections, including entity counts and physical memory usage, to monitor the health of your vector store
- **Precision Retrieval** — Fetch specific vector items by their primary keys, bypassing standard semantic boundaries to audit exact data points securely
- **Data Management** — Irreversibly delete specific vector records using primary identifiers to maintain a clean and optimized search index across your Milvus instance

### How it works

1. Subscribe to this server
2. Enter your Milvus Base URL and API Key (or Zilliz Cloud Token)
3. Start optimizing your vector search from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **ML Engineers** — test vector relevance and verify embedding dimensions through natural conversation without manual SDK scripts
- **Search Architects** — audit collection schemas and monitor indexing performance directly from your workspace
- **Software Developers** — integrate AI-powered retrieval into applications and manage vector lifecycles across multiple Milvus environments efficiently


## Available Tools
- **list_collections**: Always query this first.

List index collections tracked inside the Milvus Vector Database
- **describe_collection**: Explore the explicit schema mapping and indexing definition of a Milvus collection
- **get_collection_stats**: Get collection statistics bounding row counts natively
- **search_vectors**: Make sure to feed a strict explicit JSON Array matching exact dimensions.

Search nearest vector neighbors matching implicit embedding inputs
- **query_entities**: Query explicitly using scalar expressions to retrieve entities
- **get_entities**: Extract unique vector items bounding exactly by known Primary Keys
- **delete_entities**: Irreversibly delete specific vector records utilizing primary keys


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Milvus (Open-Source Vector Database)** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all vector collections in my Milvus instance"

**🤖 AI Agent:**
> I've retrieved 3 collections from your Milvus instance: 'image_embeddings' (Dim: 512), 'text_knowledge_base' (Dim: 1536), and 'user_profiles' (Dim: 768). Which one would you like to check the stats or schema for?

---

**👤 You:**
> "Search collection 'text_knowledge_base' for vector: [0.1, -0.2, ...]"

**🤖 AI Agent:**
> Executing ANN search… I've identified the 5 nearest neighbors. The top match has a similarity score of 0.94 and maps to entity ID '12345'. Other results include related technical documentation fragments. Would you like the full scalar data for these entities?

---

**👤 You:**
> "Show me the row count and memory stats for collection 'image_embeddings'"

**🤖 AI Agent:**
> Retrieving stats… The 'image_embeddings' collection contains 1,250,000 entities. It is currently occupying approximately 2.4 GB of memory. All indices are loaded and healthy. No anomalous data distribution detected.


## ❓ FAQ

**Q: How do I perform an ANN search through my agent?**
Use the `search_vectors` tool by providing the collection name and a JSON float array matching the collection's dimensions. Your agent will perform an Approximate Nearest Neighbor search and return the most semantically relevant entities.

**Q: Can I filter results using structured fields instead of just vectors?**
Yes. Use the `query_entities` tool with a Milvus-style filter expression. This allows you to retrieve entities based on primary keys, tags, or other scalar fields without necessarily performing a vector similarity search.

**Q: How do I check the schema and dimension requirements for a Milvus collection?**
The `describe_collection` tool retrieves the complete schema mapping. Your agent will report the required vector dimensions, index types, and primary key names, helping you ensure your search queries are compatible with the database logic.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/milvus-open-source-vector-database](https://vinkius.com/mcp/milvus-open-source-vector-database)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Milvus (Open-Source Vector Database)** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `milvus-open-source-vector-database` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Milvus (Open-Source Vector Database)** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "milvus-open-source-vector-database": {
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
