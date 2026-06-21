# Wikidata MCP Server

Access the world's largest open knowledge graph—query entities via SPARQL, perform vector searches, and manage structured data directly from your AI agent.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/wikidata)

## Overview
**Category:** the-unthinkable
**Tools Count:** 8

## Description
Connect to **Wikidata**, the central storage for structured data of Wikimedia projects. This MCP server allows your AI agent to tap into millions of items, properties, and statements using both traditional SPARQL queries and modern vector-based semantic search.

### What you can do

- **Entity Retrieval** — Fetch full data and statements for any Wikidata Item (e.g., Q42) using the `get_item` and `get_item_statements` tools.
- **Advanced Querying** — Execute complex SPARQL queries against the Wikidata Query Service (WDQS) with `execute_sparql` to find relationships and patterns across the entire graph.
- **Semantic Search** — Use `search_items_vector` and `search_properties_vector` to find entities and properties based on meaning rather than just exact keywords.
- **Data Contribution** — Update the knowledge graph by creating statements or setting descriptions with `create_statement` and `set_item_description` (requires OAuth).
- **Similarity Analysis** — Compare text strings against specific entities to get semantic similarity scores using `get_similarity_score`.

### How it works

1. Subscribe to this server
2. Provide your **User Agent** (required by Wikimedia policy)
3. Optionally provide an **OAuth 2.0 Access Token** for write operations
4. Start exploring the world's knowledge from your favorite AI client

### Who is this for?

- **Researchers & Academics** — instantly verify facts, dates, and relationships across history, science, and culture.
- **Data Scientists** — extract structured datasets for analysis or training without leaving the chat interface.
- **Developers** — find entity IDs and property schemas to integrate into applications or automate data enrichment.


## Available Tools
- **create_statement**: Requires OAuth 2.0 Access Token.

Create a new statement for an Item
- **execute_sparql**: Use hint:Query hint:optimizer "None" if queries timeout.

Execute a SPARQL query
- **get_item_statements**: Retrieve statements for a Wikidata Item
- **get_item**: g., Q42) via the Wikibase REST API.

Retrieve a specific Wikidata Item
- **get_similarity_score**: Compute similarity between text and an entity
- **search_items_vector**: Hybrid vector/keyword search for Items
- **search_properties_vector**: Hybrid vector/keyword search for Properties
- **set_item_description**: Requires OAuth 2.0 Access Token.

Set an Item description


## Installation & Usage

To install and use the **Wikidata** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/wikidata](https://vinkius.com/mcp/wikidata)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
