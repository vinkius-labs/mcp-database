# OpenSearch Vector MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/opensearch-vector)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/opensearch-vector-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/opensearch-vector-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [loved-by-devs](../categories/loved-by-devs.md)

Run k-NN vector searches on OpenSearch — create indexes, upsert embeddings, query similar documents, and manage your vector store from any AI agent.

## Description
Turn your **OpenSearch** cluster into an AI-native vector database. Create k-NN indexes, upsert embeddings, run similarity searches, and inspect index configurations — all through natural conversation with your AI agent.

### What you can do

- **Vector Search** — Execute k-Nearest Neighbors queries against any k-NN index with custom top-K limits and dense float vectors
- **Index Management** — List all cluster indexes with health status and document counts, or inspect a specific index's vector dimension, engine config, and distance metric
- **Create Index** — Provision new k-NN indexes optimized for cosine similarity with configurable vector dimensions (384, 768, 1536, etc.)
- **Document Operations** — Upsert vector documents with metadata, or delete documents from the embedding space by ID

### How it works

1. Subscribe to this server
2. Enter your OpenSearch Host, Username, and Password
3. Start managing your vector store from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **ML engineers** — test similarity queries against production embeddings without writing curl commands
- **RAG developers** — index and retrieve context documents for retrieval-augmented generation pipelines
- **Data teams** — inspect index health, document counts, and vector configurations through conversation instead of Kibana dashboards


## Available Tools
- **search**: Provide the exact index name and a JSON-stringified dense float vector array to find conceptually similar embeddings natively.

Execute a K-Nearest Neighbors (k-NN) vector search against OpenSearch
- **list_indexes**: List all explicit indexes residing on the OpenSearch cluster
- **get_index**: Retrieve explicit OpenSearch index mapping and settings
- **index_document**: This executes a fast transactional atomic insertion into the embedding space.

Upsert a singular vector document directly into an OpenSearch KNN index
- **delete_document**: Delete an explicit vector document bounding from OpenSearch
- **create_index**: knn: true` and mapping a rigid dynamic dense vector field optimized for cosine similarity.

Create a new native OpenSearch KNN index ready for vector embeddings


## 💬 Prompt Examples

Here are some examples of how you can interact with the **OpenSearch Vector** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all vector indexes in my OpenSearch cluster."

**🤖 AI Agent:**
> Found 4 indexes. 1) 'product-embeddings' — 45,230 docs, green health, 768 dimensions. 2) 'support-tickets' — 12,800 docs, green, 1536 dimensions. 3) 'knowledge-base' — 3,450 docs, green, 384 dimensions. 4) 'test-index' — 50 docs, yellow, 768 dimensions. Want me to inspect the mapping of any of these?

---

**👤 You:**
> "Find the 5 most similar documents to this embedding in the knowledge-base index."

**🤖 AI Agent:**
> Top 5 results from 'knowledge-base' (cosine similarity): 1) 'API Rate Limiting Guide' — score: 0.94. 2) 'Authentication Best Practices' — score: 0.89. 3) 'Error Handling Documentation' — score: 0.87. 4) 'SDK Migration Guide v3' — score: 0.83. 5) 'Webhook Configuration' — score: 0.81. Want me to pull the full content of the top result?

---

**👤 You:**
> "Create a new k-NN index called 'customer-feedback' with 1536 dimensions."

**🤖 AI Agent:**
> Index 'customer-feedback' created successfully. Configuration: k-NN enabled, 1536 dimensions, cosine similarity, NMSLIB engine. The index is empty and ready for document ingestion. Want me to upsert a test document to verify the mapping?


## Installation & Usage

To install and use the **OpenSearch Vector** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/opensearch-vector](https://vinkius.com/mcp/opensearch-vector)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
