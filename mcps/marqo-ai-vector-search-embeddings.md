# Marqo AI (Vector Search & Embeddings) MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/marqo-ai-vector-search-embeddings)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [ai-frontier](../categories/ai-frontier.md)

Manage semantic search via Marqo — execute tensor queries, index JSON documents, and audit vector indices.

## Description
Connect your **Marqo** instance to any AI agent and take full control of your semantic search infrastructure, vector embeddings, and real-time document indexing through natural conversation.

### What you can do

- **Tensor Search Orchestration** — Execute dense semantic similarity searches against your indices using natural language queries, with Marqo handling embedding extraction automatically
- **Dynamic Document Ingestion** — Write new JSON records into your vector indices directly from your agent, allowing for instant searchability of fresh data mappings
- **Index Lifecycle Management** — Create explicitly bounded new vector indices with custom model settings and dimension constraints to optimize your search architecture
- **Vector Audit & Stats** — Retrieve detailed configuration metrics for your indices, including document counts, embedding model types, and underlying schema mappings
- **Precision Deletion** — Physically eradicate vectorized representations by targeting specific scalar identifiers to maintain a clean and relevant search index
- **Resource Inventory** — List all available vector indices on your Marqo instance to identify collection boundaries before executing search queries

### How it works

1. Subscribe to this server
2. Enter your Marqo API URL and API Key
3. Start optimizing your semantic search from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Search Architects** — test semantic relevance and verify index configurations through natural conversation without manual API tools
- **Machine Learning Engineers** — monitor vector index stats and verify document embedding results directly from your workspace
- **Software Developers** — integrate AI-powered search results into applications and manage document lifecycles across multiple Marqo environments efficiently


## Available Tools (6)
- **list_indexes**: Crucial before writing queries hitting arbitrary collections.

List all Marqo vector indexes
- **get_index_stats**: Get configuration and stats for an index
- **tensor_search**: Perform natural language tensor search on Marqo
- **add_documents**: Write new documents into Marqo
- **delete_documents**: Delete specific documents from Marqo by targeting their IDs
- **create_index**: Create an explicitly bounded new vector index


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Marqo AI (Vector Search & Embeddings)** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Semantic search in index 'products' for 'lightweight running shoes for trails'"

**🤖 AI Agent:**
> Executing tensor search… I've found 5 highly relevant products. Top match: 'Swift-Trail Runner' (Score: 0.89). Other results include specialized mountain gear and ultra-light hikers. Would you like to see the full JSON metadata for these matches?

---

**👤 You:**
> "List all vector indexes in my Marqo instance"

**🤖 AI Agent:**
> I've identified 3 indexes: 'products' (Ecommerce catalog), 'support-docs' (Technical KB), and 'user-profiles' (Personalization data). Which one would you like to check the stats for?

---

**👤 You:**
> "Add this document to the 'support-docs' index: {"title": "API Auth", "content": "Use Marqo-API-Key header"}"

**🤖 AI Agent:**
> Document added successfully to 'support-docs'. Marqo has vectorized the content using your configured embedding model. The document is now indexed and immediately available for semantic searches. Your new doc ID is 'marqo-12345'.


## ❓ FAQ

**Q: Does Marqo handle the vector embeddings for me through the agent?**
Yes. Marqo is an end-to-end engine. When you use the `tensor_search` tool, you provide natural language and Marqo handles the model inference and vector extraction under the hood, returning semantically relevant results immediately.

**Q: Can I add new data to a vector index through a conversation?**
Absolutely. Use the `add_documents` tool by providing a JSON array of your documents. Your agent will synchronize these records into the target index, and they will be searchable via semantic query instantly.

**Q: How do I check the stats of my vector index?**
The `get_index_stats` tool retrieves critical metrics for a specific index. Your agent will report the document count, memory usage, and configuration details, helping you monitor the health of your vector store.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/marqo-ai-vector-search-embeddings](https://vinkius.com/mcp/marqo-ai-vector-search-embeddings)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Marqo AI (Vector Search & Embeddings)** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `marqo-ai-vector-search-embeddings` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Marqo AI (Vector Search & Embeddings)** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "marqo-ai-vector-search-embeddings": {
      "url": "https://edge.vinkius.com/[TOKEN]/mcp"
    }
  }
}
```

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
