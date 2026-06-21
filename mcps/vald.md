# Vald MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/vald)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/vald-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/vald-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [databases](../categories/databases.md)

Power your agent with Vald — query, insert, and manage dense vectors on a highly scalable, distributed nearest-neighbor engine.

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


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Vald** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Is the Vald cluster operational right now?"

**🤖 AI Agent:**
> I've checked the Vald Gateway. The engine is healthy and accepting requests! The current clustered infrastructure responds well to Ping mechanisms.

---

**👤 You:**
> "Can you check the vector details stored for UUID 'user-profile-89'?"

**🤖 AI Agent:**
> I retrieved the vector data for `user-profile-89`. The embedding array spans 768 dimensions. Do you want me to render its raw float values here or proceed to query for its nearest neighbors?

---

**👤 You:**
> "Update the existing item 'context-fragment-12' with this new 1536-dimensional array: [0.38, -0.19, 0...]."

**🤖 AI Agent:**
> Done. The vector for ID `context-fragment-12` has been successfully updated in your Vald cluster. The engine replaced its old representation with your newly uploaded 1536-dimensional array without breaking any active query connections.


## Installation & Usage

To install and use the **Vald** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/vald](https://vinkius.com/mcp/vald)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
