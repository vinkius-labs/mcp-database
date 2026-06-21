# DataStax Astra DB Vector MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/datastax-astra-db-vector)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/datastax-astra-db-vector-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/datastax-astra-db-vector-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [ai-frontier](../categories/ai-frontier.md)

Manage Astra DB collections, documents, and perform vector similarity searches via DataStax directly from your AI agent.

## Description
Connect your **Astra DB** instance to any AI agent and seamlessly execute complex NoSQL and vector searches through natural conversation. Built on DataStax's powerful engine, this integration gives your AI agents full contextual access to your unstructured data layer.

### What you can do

- **Vector Search** — Perform Approximate Nearest Neighbor (ANN) similarity searches directly within your chat to find semantically related documents
- **Document Management** — Insert, discover, read, count, or delete exact NoSQL JSON documents across your active collections
- **Collections** — List and browse available tables and collections currently active in your configured Astra DB namespace

### How it works

1. Subscribe to this secure MCP Server
2. Enter your Astra DB API Endpoint, Namespace, and Application Token
3. Start querying your contextual vector database naturally from Claude, Cursor, or any compatible AI client

Your AI agent becomes a brilliant database administrator capable of exploring embeddings instantly.

### Who is this for?

- **AI Developers** — retrieve precise contextual embeddings during advanced RAG workflows without leaving the IDE
- **Data Engineers** — explore and debug JSON document anomalies quickly through conversational commands
- **Product Teams** — inspect unstructured vector data dynamically to understand AI search results behavior
- **DBAs** — manage and count records across collections effortlessly


## Available Tools
- **list_collections**: List all collections in the Astra DB namespace
- **find_documents**: Useful for standard NoSQL document retrieval.

Find documents in an Astra DB collection
- **find_one_document**: Find a single document in an Astra DB collection
- **vector_search**: Perform an ANN vector similarity search on an Astra DB collection
- **insert_document**: The document can include a pre-generated $vector key for embedding searches.

Insert a new document into an Astra DB collection
- **delete_document**: Delete a document from an Astra DB collection
- **count_documents**: Count total documents in an Astra DB collection


## 💬 Prompt Examples

Here are some examples of how you can interact with the **DataStax Astra DB Vector** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List the collections available in my Astra DB."

**🤖 AI Agent:**
> Here are the collections present in your connected Astra DB namespace: `user_vectors` (active), `products` (active), and `archived_logs`. Which one would you like to inspect?

---

**👤 You:**
> "Count the documents inside the 'products' collection."

**🤖 AI Agent:**
> Your `products` collection currently holds exactly 1,024 active JSON documents across the cluster.

---

**👤 You:**
> "Find documents matching this filter in 'user_vectors': {"city": "San Francisco"}."

**🤖 AI Agent:**
> I found 3 matching documents in `user_vectors`. Here are the returned JSON blobs detailing their user properties and associated embeddings...


## Installation & Usage

To install and use the **DataStax Astra DB Vector** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/datastax-astra-db-vector](https://vinkius.com/mcp/datastax-astra-db-vector)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
