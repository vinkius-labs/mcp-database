# pgvector (Vector Database) MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/pgvector-vector-database)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/pgvector-vector-database-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/pgvector-vector-database-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [loved-by-devs](../categories/loved-by-devs.md)

Run vector similarity searches, manage embedding tables, and build AI-powered retrieval pipelines — all directly inside your existing PostgreSQL database.

## Description
Connect your **PostgreSQL + pgvector** database to any AI agent and manage vector embeddings, similarity searches, and index optimizations through natural conversation.

### What you can do

- **Vector Similarity Search** — Run nearest-neighbor queries using cosine, L2, or inner product distance metrics across millions of embeddings with a single prompt.
- **Table Management** — Discover which tables contain vector columns, create new embedding tables with custom dimensions, and inspect your schema.
- **Embedding CRUD** — Insert, update, and delete individual vector entries with metadata, keeping your knowledge base fresh and accurate.
- **Index Optimization** — Create HNSW or IVFFlat indexes on vector columns to accelerate approximate nearest-neighbor (ANN) queries by orders of magnitude.

### How it works

1. Subscribe to the pgvector integration on the marketplace.
2. Paste your PostgreSQL connection string (e.g., `postgresql://user:pass@host:5432/db`).
3. Ask your AI agent to search vectors, create tables, or optimize indexes.

### Who is this for?

- **AI Engineers** — Build RAG (Retrieval-Augmented Generation) pipelines that query production embeddings without writing custom API endpoints.
- **Data Architects** — Manage vector schemas, monitor index performance, and optimize query latency from a single conversational interface.
- **Fullstack Developers** — Add semantic search to existing apps by querying pgvector directly through your AI agent, no new microservices needed.


## Available Tools
- **search_vectors**: Vector similarity search
- **list_tables**: List tables
- **insert_vector**: Insert a vector
- **delete_vector**: Delete a vector
- **create_table**: Create vector table
- **create_index**: Create vector index


## 💬 Prompt Examples

Here are some examples of how you can interact with the **pgvector (Vector Database)** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Show me all tables with vector columns in my database."

**🤖 AI Agent:**
> Found 2 tables with vector columns: `document_chunks` (1536 dimensions, 48,200 rows, HNSW index active) and `product_embeddings` (768 dimensions, 12,500 rows, no index). Want me to create an IVFFlat index on `product_embeddings`?

---

**👤 You:**
> "Search for the 5 most similar documents to this query in the document_chunks table."

**🤖 AI Agent:**
> Top 5 results from `document_chunks` (cosine distance):
1. "API Authentication Guide" — distance: 0.12
2. "OAuth 2.0 Setup" — distance: 0.18
3. "Token Refresh Flow" — distance: 0.23
4. "Security Best Practices" — distance: 0.31
5. "Rate Limiting" — distance: 0.35
Want me to retrieve the full content of the top result?

---

**👤 You:**
> "Create a new table called 'support_tickets' with 1536-dimension vectors and an HNSW index."

**🤖 AI Agent:**
> Done. Created table `support_tickets` with columns: `id TEXT PRIMARY KEY`, `embedding vector(1536)`, `metadata JSONB`. Then created HNSW index using `vector_cosine_ops`. The table is ready for inserts.


## Installation & Usage

To install and use the **pgvector (Vector Database)** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/pgvector-vector-database](https://vinkius.com/mcp/pgvector-vector-database)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
