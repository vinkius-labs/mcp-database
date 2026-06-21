# Milvus (Open-Source Vector Database) MCP Server

Manage vector storage via Milvus — perform ANN searches, query scalar entities, and audit collections.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/milvus-open-source-vector-database)

## Overview
**Category:** loved-by-devs
**Tools Count:** 7

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


## Installation & Usage

To install and use the **Milvus (Open-Source Vector Database)** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/milvus-open-source-vector-database](https://vinkius.com/mcp/milvus-open-source-vector-database)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
