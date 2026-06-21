# Cognee MCP Server

Build knowledge graphs from unstructured data — ingest text, extract entities and relationships, and search with graph-aware AI reasoning.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/cognee)

## Overview
**Category:** ai-frontier
**Tools Count:** 4

## Description
Connect your AI agent to **Cognee** — the open-source knowledge graph platform that transforms unstructured data into structured, searchable knowledge.

### What you can do

- **Add Data** — Ingest raw text, documents, or structured data into named datasets. Cognee processes and stores the data for subsequent graph construction
- **Cognify** — Transform ingested data into a structured knowledge graph by automatically extracting entities, relationships, and semantic connections
- **Search Knowledge** — Query the knowledge graph using four retrieval strategies: graph-aware completion (LLM + graph traversal), summaries, structured insights, or raw vector similarity
- **Get Insights** — Retrieve structured entity relationships showing how concepts connect across your knowledge base

### How it works

1. Subscribe to this server
2. Enter your Cognee API key
3. Ingest data → Cognify → Search with graph-aware reasoning

### Why Cognee over standard RAG?

- **Relationship-aware** — understands HOW facts connect, not just what they say
- **Graph + Vector hybrid** — combines graph traversal with semantic search for superior recall
- **Temporal awareness** — tracks when facts were added and reason over time-based connections


## Available Tools
- **cognee_add_data**: After ingestion, use the cognify tool to process the data into a structured knowledge graph with entities and relationships.

Ingest text or documents into the Cognee knowledge base. This is the first step before building a knowledge graph
- **cognee_cognify**: This step extracts entities, identifies relationships, generates embeddings, and creates the graph structure needed for intelligent search.

Process ingested data into a structured knowledge graph. Extracts entities, relationships, and builds a searchable graph structure
- **cognee_get_insights**: Useful for understanding relationships between topics, discovering hidden connections, and building comprehensive knowledge views.

Retrieve structured entity relationships and insights from the knowledge graph
- **cognee_search**: Search the knowledge graph using natural language. Returns context-aware answers using graph traversal and semantic search


## Installation & Usage

To install and use the **Cognee** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/cognee](https://vinkius.com/mcp/cognee)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
