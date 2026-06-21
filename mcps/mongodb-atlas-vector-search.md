# MongoDB Atlas Vector Search MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/mongodb-atlas-vector-search)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/mongodb-atlas-vector-search-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/mongodb-atlas-vector-search-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [industry-titans](../categories/industry-titans.md)

Manage vector storage via MongoDB Atlas — perform similarity searches, query MQL documents, and audit collections.

## Description
Connect your **MongoDB Atlas** cluster to any AI agent and take full control of your high-performance vector search, embedding storage, and operational data management through natural conversation.

### What you can do

- **Vector Similarity Search** — Execute sophisticated '$vectorSearch' queries against your collections to retrieve semantically relevant matches using raw embedding vectors directly from your agent
- **Unified Data Management** — Find, insert, and delete standard MongoDB documents using literal MQL (MongoDB Query Language) filters to manage both vector and operational data in a single system
- **Search Index Provisioning** — Create and configure Atlas Search indices with custom dimensions and mapping definitions to optimize your cluster's similarity calculation infrastructure
- **Collection Lifecycle Audit** — List all managed data collections and retrieve schema boundaries to understand namespace references and database organization natively
- **Real-time Ingestion** — Synchronize new JSON records into your collections, allowing for instant searchability and automated vector parsing if Atlas triggers are enabled
- **Precision Retrieval** — Execute targeted MQL queries to fetch specific data points or metadata chunks, bypassing vector logic for rapid structural verification and auditing

### How it works

1. Subscribe to this server
2. Enter your MongoDB Atlas Data API URL and API Key
3. Start optimizing your search infrastructure from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **ML Engineers** — test vector relevance and verify embedding dimensions through natural conversation without manual SDK scripts
- **Backend Developers** — manage operational data and vector search results in a single workflow directly from your workspace terminal
- **Search Architects** — audit search indices and monitor collection organization across multiple Atlas environments efficiently


## Available Tools
- **search**: Perform highly-dimensional Vector similarity search using $vectorSearch
- **find**: Find standard MongoDB documents resolving standard query filters
- **insert**: Insert a distinct generic document into standard target collection
- **delete**: Delete literal documents bounded by the parsed MongoDB filters
- **list_collections**: List accessible data collections bound explicitly inside Atlas limits
- **create_index**: Create literal standard embedding Search Index bound to dimensions


## 💬 Prompt Examples

Here are some examples of how you can interact with the **MongoDB Atlas Vector Search** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Vector search in 'knowledge_base' for vector: [0.1, -0.2, ...]"

**🤖 AI Agent:**
> Executing $vectorSearch on Atlas… I've identified the 5 most similar documents in the 'knowledge_base' collection. The top match has a high similarity score and contains content about 'Cloud Architecture'. Would you like the full JSON metadata for these matches?

---

**👤 You:**
> "Find active users in the 'users' collection with plan 'pro'"

**🤖 AI Agent:**
> Executing MQL find query… I've identified 12 users matching the criteria: `{"status": "active", "plan": "pro"}`. Highlights include 'Alex Smith' (ID: 123) and 'Sarah Johnson' (ID: 456). I can retrieve the full account metadata for any of these users if you'd like.

---

**👤 You:**
> "List all collections in the 'production' database"

**🤖 AI Agent:**
> I've retrieved the collection list for the 'production' database: 'users', 'orders', 'knowledge_base', 'system_logs', and 'product_catalog'. Which one would you like to audit or run a similarity search on?


## Installation & Usage

To install and use the **MongoDB Atlas Vector Search** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/mongodb-atlas-vector-search](https://vinkius.com/mcp/mongodb-atlas-vector-search)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
