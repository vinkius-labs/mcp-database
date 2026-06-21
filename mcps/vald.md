# Vald MCP Server

Power your agent with Vald — query, insert, and manage dense vectors on a highly scalable, distributed nearest-neighbor engine.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/vald)

## Overview
**Category:** databases
**Tools Count:** 6

## Description
Connect your **Vald** cluster to any AI agent and bring distributed, high-speed approximate nearest neighbor (ANN) vector search directly to your conversational workflow.

### What you can do

- **Vector Search** — Perform rapid semantic searches across millions of embedded data points just by querying the agent.
- **Data Ingestion** — Insert new high-dimensional vectors directly into the Vald index for instant future retrievability in your RAG pipelines.
- **Index Management** — Update the vector representations of existing records or permanently remove specific items from the engine cluster.
- **Cluster Health** — Automatically retrieve operational system information, agent health statuses, and node details regarding your active Vald deployment.

### How it works

1. Subscribe to this server
2. Enter your Vald Gateway Host address
3. Start performing semantic queries and updates from Claude, Cursor, or any MCP-compatible client

Your AI agent becomes the direct line to your massive vector knowledge base.

### Who is this for?

- **Machine Learning Engineers** — rapidly test and visualize embedding changes against a live Vald instance without scripting.
- **Data Scientists** — execute on-the-fly 'top-k' semantic queries directly from an IDE to validate search recall results.
- **DevOps Engineers** — check the active engine health status and cluster info via natural language whenever anomalies happen.
- **Backend Developers** — quickly purge corrupted vectors or update legacy records bypassing native database terminals.


## Available Tools
- **get_engine_info**: Retrieves operational information and health of the Vald engine
- **get_vector_details**: Retrieves the raw vector data for a specific ID
- **insert_vector**: Provide a unique ID and the vector as a JSON array.

Inserts a new vector into the Vald index
- **delete_vector**: This action is irreversible.

Permanently removes a vector from the Vald index
- **update_vector**: Provide the existing ID and new vector array.

Updates an existing vector in the Vald index
- **search_vectors**: Provide a query vector as a JSON array of floats.

Performs a nearest neighbor vector similarity search


## Installation & Usage

To install and use the **Vald** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/vald](https://vinkius.com/mcp/vald)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
