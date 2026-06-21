# Pinecone MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/pinecone)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/pinecone-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/pinecone-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [loved-by-devs](../categories/loved-by-devs.md)

Equip your AI agent to manage your Pinecone vector databases. Query embeddings, fetch metrics, manage collections, and run stats natively via chat.

## Description
Connect your **Pinecone** knowledge graph environment straight into your AI agent's logic. Give your preferred Large Language Model the keys to fetch, query, and modify vector spaces via natural language context without leaving the chat interface.

### What you can do

- **Index Hierarchy** — Retrieve structural blueprints instantly using `list_indexes` and fetch intricate topology parameters utilizing `describe_index`.
- **Semantic Harvesting** — Pass pure array values to execute blazing-fast retrieval with `query_vectors`, or pinpoint specific embeddings natively employing `fetch_vectors`.
- **Space Archiving** — Monitor grouped snapshot arrays leveraging `list_collections` and perform surgical cleanups executing `delete_vectors` accurately.
- **Performance Auditing** — Ask the model to pull real-time health checks calling `get_index_stats` to reveal vector capacity limits across pods.

### How it works

1. Subscribe digitally to this MCP Server
2. Introduce your secret API Key extracted directly from the Pinecone Developer Console
3. Engage your IDE/Chat framework asking it to run RAG checks on your vector stores or pull statistics via standard conversation

### Who is this for?

- **AI/ML Engineers** — troubleshoot the relevance of semantic chunks actively fetched through conversational queries without constructing Python test scripts.
- **Data Custodians** — audit storage capacities across multitenant indexes checking if garbage collection deleted vectors properly via terminal prompts.
- **Agent Builders** — weave dynamic RAG integrations into other systems testing the Pinecone core endpoints directly via a Cursor workspace.


## Available Tools
- **delete_vectors**: Delete vectors from an index
- **describe_index**: Get configuration details for an index
- **fetch_vectors**: Fetch specific vectors by their IDs
- **get_index_stats**: Get usage statistics for an index
- **list_collections**: List all index collections
- **list_indexes**: List all Pinecone indexes
- **query_vectors**: Returns the most similar vectors and their metadata.

Search for similar vectors


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Pinecone** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Check the vector count stats for the index named `document-embeddings`."

**🤖 AI Agent:**
> Index `document-embeddings` currently holds 45,920 vector records. Its mathematical dimension is locked at 1536 (typical OpenAI output), and the pod architecture is 90% full.

---

**👤 You:**
> "Delete all vectors belonging to the user ID 'auth-abc123' namespace."

**🤖 AI Agent:**
> Executed `delete_vectors` successfully. The cluster associated with 'auth-abc123' has been wiped from the index.

---

**👤 You:**
> "List all existing collections created in my Pinecone environment."

**🤖 AI Agent:**
> You have 2 active collection snapshots stored mapping to production: `backup-q1-2026` and `knowledge-base-staging`.


## Installation & Usage

To install and use the **Pinecone** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/pinecone](https://vinkius.com/mcp/pinecone)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
