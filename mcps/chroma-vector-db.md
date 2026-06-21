# Chroma (Vector DB) MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/chroma-vector-db)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [loved-by-devs](../categories/loved-by-devs.md)

Manage vector embeddings via Chroma — list collections, query embeddings, and audit document counts directly from any AI agent.

## Description
Connect your **Chroma** vector database to any AI agent and take full control of your semantic data through natural conversation.

### What you can do

- **Vector Collections** — List all available collections and inspect their deep configuration and metadata
- **Semantic Search** — Perform high-dimensional vector similarity searches to find relevant context for your LLM applications
- **Document Auditing** — Count documents, peek at unstructured data segments, and retrieve specific records by ID
- **Instance Health** — Monitor heartbeats and connectivity across Chroma Cloud or self-hosted instances
- **Tenant & Database Management** — Switch between different tenants and databases to isolate your production and staging environments

### How it works

1. Subscribe to this server
2. Enter your Chroma URL (Cloud or self-hosted) and your API Key
3. Start querying your embeddings from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **AI Developers** — test and debug vector search logic using natural language without writing Python scripts
- **Data Engineers** — audit collection volumes and metadata consistency across different environments
- **Product Managers** — inspect what context is being fed to AI agents by peeking at stored embeddings
- **DevOps Teams** — monitor instance connectivity and health through automated heartbeats


## Available Tools
- **list_collections**: List all explicitly defined Vector Collections within a given tenant database
- **get_collection**: Identify bounded logical settings configuring a specific Vector Collection block
- **count_documents**: Execute explicit structural tracking enumerating total document volumes
- **get_documents**: Retrieve exact physical documents and semantic context inside known arrays
- **query_embeddings**: Identify precise logical bounds matching high-dimensional semantic clustering
- **peek_documents**: Extracts explicitly attached bounded preview of the Database limits
- **check_heartbeat**: Validate fundamental network availability against explicit Chroma API nodes


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Chroma (Vector DB)** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all vector collections"

**🤖 AI Agent:**
> I found 3 collections: 'knowledge-base', 'user-embeddings', and 'staging-docs'. Would you like to check the document count for any of them?

---

**👤 You:**
> "Peek at the first 5 documents in 'knowledge-base'"

**🤖 AI Agent:**
> Peeking into 'knowledge-base'... Here are the first 5 documents. They contain technical documentation about our API endpoints and authentication flows. Each has metadata like 'source' and 'last_updated'.

---

**👤 You:**
> "Is the Chroma server alive?"

**🤖 AI Agent:**
> Checking heartbeat... Connection successful! The Chroma instance responded in 12ms and is fully operational.


## ❓ FAQ

**Q: Can my agent perform semantic search across my collections?**
Yes. Provide the vector embedding array in JSON format, and your agent will return the closest document matches along with their distance metrics. It is the perfect way to test your RAG (Retrieval-Augmented Generation) logic without complex scripts.

**Q: How can I verify the health of my self-hosted Chroma instance?**
Simply ask your agent to check the heartbeat. The agent performs a nanosecond-level responsiveness test against your API nodes, confirming the physical database is active and reachable from the gateway.

**Q: I manage multiple tenants — how do I switch between them?**
You can define the tenant and database names during the setup phase. If you need to switch often, you can update the credentials in the dashboard. The agent uses these values for all collection and document operations to ensure strict isolation.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/chroma-vector-db](https://vinkius.com/mcp/chroma-vector-db)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Chroma (Vector DB)** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `chroma-vector-db` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Chroma (Vector DB)** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "chroma-vector-db": {
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
