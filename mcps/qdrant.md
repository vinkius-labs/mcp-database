# Qdrant MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/qdrant)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [ai-frontier](../categories/ai-frontier.md)

Empower your AI to interact directly with your Qdrant vector database — query clusters, perform similarity searches, and manage collections effortlessly.

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


## Available Tools (7)
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


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Qdrant** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List the configurations for all collections in my Qdrant instance."

**🤖 AI Agent:**
> I found 2 collections. 
1. `docs-embeddings`: Contains 4,500 points, optimized using Cosine distance, vector size 1536.
2. `image-features`: Contains 120,400 points, optimized using Dot product, vector size 512.
Should I inspect `docs-embeddings` further?

---

**👤 You:**
> "Count the total embedded points in the 'docs-embeddings' collection."

**🤖 AI Agent:**
> The `count` tool indicates there are exactly 14,235 points currently indexed in the `docs-embeddings` collection.

---

**👤 You:**
> "Scroll and show me the IDs and payloads of the first 3 items in the 'users' collection."

**🤖 AI Agent:**
> Scrolling through 'users', here are the top 3 IDs and payloads:
1. ID: `1f2a3`, Payload: { "role": "admin", "department": "sales" }
2. ID: `7b9c1`, Payload: { "role": "user", "department": "support" }
3. ID: `9d8e4`, Payload: { "role": "user", "department": "sales" }


## ❓ FAQ

**Q: How do I find my Qdrant URL and API Key?**
For **Qdrant Cloud**: Go to the Qdrant Cloud Console, select your cluster to open the Cluster Detail Page. The endpoint will be displayed there (e.g., `xyz.us-east4-0.gcp.cloud.qdrant.io`), and you can generate Database API Keys underneath it (they start with `eyJhb`). For **Self-hosted**: Provide your custom URL and the static custom key you defined in your `config.yaml`.

**Q: Can my AI use this for a RAG architecture directly?**
Yes contextually, but practically your agent acts as the database debugger. It can formulate vector arrays to query `search_points`, retrieving identical payload structures. It's meant for the *engineer building the RAG*, helping you inspect distances and debug faulty retrieval mechanisms mid-code.

**Q: Does it support deleting vectors?**
Yes. If an embedding got corrupted or references dropped articles, use the `delete` tool. Pass the collection name and the list of specific IDs. Qdrant handles the mutation instantly and updates the index without rebuilding.

**Q: What if I have millions of points?**
Instead of overloading your chat context, instruct your agent to use the `count` tool to grasp the scale, and the `scroll` tool with a small limit constraint (e.g., 5-10 records at a time). This paginates large bodies cleanly when analyzing index health.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/qdrant](https://vinkius.com/mcp/qdrant)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Qdrant** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `qdrant` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Qdrant** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "qdrant": {
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
