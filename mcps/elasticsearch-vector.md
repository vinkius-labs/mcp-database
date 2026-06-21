# Elasticsearch Vector MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/elasticsearch-vector)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/elasticsearch-vector-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/elasticsearch-vector-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [brain-trust](../categories/brain-trust.md)

Empower vector search via Elasticsearch — perform dense vector kNN searches, handle index mappings, and index embedding documents directly from any AI agent.

## Description
Connect your **Elasticsearch** cluster to any AI agent and take full control of your vector search and semantic discovery workflows through natural conversation.

### What you can do

- **AI-Powered Vector Search** — Perform raw K-Nearest Neighbors (kNN) computations mapping absolute semantic similarity across multi-dimensional embedding arrays
- **Index Orchestration** — Enumerate active storage namespaces and validate physical Elasticsearch clusters tracking explicit dimensional shards securely
- **Schema Management** — Analyze specific index mapping rules and provision strictly typed data structures enforcing numeric dimensions for cluster readiness
- **Document Indexing** — Command synchronous bulk insertions attaching exact `dense_vector` embedding payloads to persist data into raw Lucene partitions
- **Data Invalidation** — Enforce immediate hard document vaporization finding specific exact UUIDs stripping records from physical indices seamlessly
- **Metadata Auditing** — Analyze dimensional constraints and matching similarity thresholds perfectly to verify your vector search configurations

### How it works

1. Subscribe to this server
2. Enter your Elasticsearch Host URL and API Key (found in Kibana > Stack Management > Security > API Keys)
3. Start managing your vector search from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **AI Engineers** — perform semantic searches and test embedding models without writing complex query DSL
- **Software Developers** — index embedding documents and verify kNN search results directly from the IDE or chat
- **Data Scientists** — monitor vector index mappings and verify dimensional constraints using natural language
- **Ops Teams** — verify cluster index health and manage vector storage namespaces in real-time


## Available Tools
- **search**: Dense vector knn search
- **list_indexes**: List all indexes
- **get_index**: Get index info
- **index_document**: Index a document
- **delete_document**: Delete a document
- **create_index**: Create dense_vector index


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Elasticsearch Vector** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Perform a kNN search in index 'product-embeddings' with vector [0.1, 0.2, ...]"

**🤖 AI Agent:**
> Searching 'product-embeddings'... I found the top 5 most similar documents. Result #1: 'Leather Backpack' (Similarity: 0.98). Result #2: 'Canvas Tote' (Similarity: 0.92). Would you like the full metadata for these results?

---

**👤 You:**
> "Create a new vector index 'image-features' with 512 dimensions"

**🤖 AI Agent:**
> Index created! 'image-features' is now initialized with 512 dimensions and is ready for document ingestion. I can now help you index your first embedding document.

---

**👤 You:**
> "List all vector indexes in my cluster"

**🤖 AI Agent:**
> Retrieving indexes... I found 3 vector-enabled indexes: 'product-embeddings' (1536 dims), 'image-features' (512 dims), and 'text-semantic-v1' (768 dims). Which one would you like to inspect?


## Installation & Usage

To install and use the **Elasticsearch Vector** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/elasticsearch-vector](https://vinkius.com/mcp/elasticsearch-vector)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
