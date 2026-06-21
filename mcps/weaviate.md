# Weaviate MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/weaviate)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/weaviate-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/weaviate-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [loved-by-devs](../categories/loved-by-devs.md)

Search and manage vector data on Weaviate — the AI-native database for building production-grade AI applications.

## Description
Connect your **Weaviate** instance to any AI agent and harness the power of vector search and semantic data management through natural conversation.

### What you can do

- **Semantic Search** — Perform nearest neighbor vector similarity searches to find relevant content based on context and meaning
- **Schema Management** — Retrieve the complete instance schema or specific class definitions to understand your data structure
- **Object Discovery** — Browse and list data objects within any class, including full property values and vector data
- **Deep Data Audit** — Retrieve specific data objects by their UUID to inspect metadata and internal configurations
- **Cluster Monitoring** — Monitor operational health, node status, and resource usage of your Weaviate cluster nodes
- **Instance Metadata** — View server version, enabled modules, and high-level configuration details directly from your agent

### How it works

1. Subscribe to this server
2. Enter your Weaviate Base URL and API Key
3. Start querying your vector data collections through Claude, Cursor, or any MCP-compatible client

No more manual JSON querying in complex database consoles. Your AI agent becomes your vector database administrator.

### Who is this for?

- **AI Developers** — test and refine semantic search queries and verify vector data ingestion
- **Data Engineers** — audit database schemas, monitor cluster health, and browse indexed objects
- **Research Teams** — quickly surface relevant documents and data points from massive vector collections through chat
- **SRE & DevOps** — monitor the operational status of Weaviate nodes and manage instance configurations


## Available Tools
- **get_class_schema**: Retrieves the schema definition for a specific class (collection)
- **get_instance_metadata**: Retrieves metadata about the Weaviate instance
- **get_cluster_nodes**: Retrieves operational information about the Weaviate cluster nodes
- **get_object_details**: Retrieves a specific data object by its UUID
- **get_full_schema**: Retrieves the complete Weaviate schema (all collections)
- **list_objects**: Supports basic pagination via limit.

Lists data objects within a specific class
- **search_near_vector**: Provide a class name and a query vector as a JSON array of floats.

Performs a nearest neighbor vector similarity search


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Weaviate** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all classes in my Weaviate schema."

**🤖 AI Agent:**
> I found 3 classes in your schema: 'Article', 'Product', and 'UserFeedback'. Would you like to see the property definitions for any of these classes?

---

**👤 You:**
> "Search the 'Article' class for items similar to this vector: [0.12, -0.05, 0.88, ...]."

**🤖 AI Agent:**
> I found 5 similar articles. The top match is 'Vector Search for Beginners' (UUID: 550e8400-e29b...) with a similarity score of 0.94. Would you like to see the full content of this article?

---

**👤 You:**
> "What is the current health status of my Weaviate cluster nodes?"

**🤖 AI Agent:**
> All 3 nodes in your cluster are currently 'HEALTHY'. Node-1 is using 42% CPU and 6.5GB RAM. Node-2 and Node-3 are also within normal operating parameters. No issues detected.


## Installation & Usage

To install and use the **Weaviate** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/weaviate](https://vinkius.com/mcp/weaviate)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
