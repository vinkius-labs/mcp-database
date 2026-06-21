# Qdrant MCP Server

Empower your AI to interact directly with your Qdrant vector database — query clusters, perform similarity searches, and manage collections effortlessly.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/qdrant)

## Overview
**Category:** ai-frontier
**Tools Count:** 7

## Description
Connect your **Qdrant** vector database (Cloud or Self-Hosted) to any AI agent and bring powerful semantic retrieval and database management into your conversation.

### What you can do

- **Discover Collections** — List all vector collections in your cluster, fetch detailed distance metrics, and monitor total payload points instantly
- **Semantic Vector Search** — Perform nearest neighbor similarity searches. Pass a JSON array of floats and retrieve the exact payloads matching your query
- **Data Management** — Read specific points by ID or scroll sequentially through giant datasets to debug payloads and embedding quality
- **Mutation Operations** — Delete redundant data points safely without building separate admin scripts

### How it works

1. Subscribe to this server
2. Provide your Qdrant Base URL and API Key
3. Start querying your embeddings directly from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **AI & ML Engineers** — query embedded spaces directly from your console while building RAG (Retrieval-Augmented Generation) applications
- **Data Scientists** — inspect payloads and test distance parameters on live indices without launching Jupyter Notebooks
- **Backend Developers** — manage vector cluster configuration and clear bad datasets efficiently


## Available Tools
- **list_collections**: Lists all collections in the Qdrant instance
- **get_collection**: Retrieves detailed information about a specific collection
- **search**: You must provide a JSON array of floats for the query vector.

Performs a nearest neighbor vector search in a collection
- **get_points**: Retrieves specific points by their IDs
- **scroll**: Returns points with their payloads.

Scrolls through points in a collection, useful for pagination
- **count**: Counts the total number of points in a collection
- **delete**: This action is irreversible.

Deletes specific points from a collection


## Installation & Usage

To install and use the **Qdrant** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/qdrant](https://vinkius.com/mcp/qdrant)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
