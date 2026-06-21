# OpenSearch Vector MCP Server

Run k-NN vector searches on OpenSearch — create indexes, upsert embeddings, query similar documents, and manage your vector store from any AI agent.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/opensearch-vector)

## Overview
**Category:** loved-by-devs
**Tools Count:** 6

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


## Installation & Usage

To install and use the **OpenSearch Vector** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/opensearch-vector](https://vinkius.com/mcp/opensearch-vector)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
