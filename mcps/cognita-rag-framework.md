# Cognita (RAG Framework) MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/cognita-rag-framework)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [friends-mcp](../categories/friends-mcp.md)

Manage modular RAG via Cognita — list collections, ingest data sources, and perform AI-driven Q&A directly from any AI agent.

## Description
Connect your **Cognita** (TrueFoundry) instance to any AI agent and take full control of your modular RAG workflows through natural conversation.

### What you can do

- **Knowledge Collections** — List and audit RAG collections to inspect embedding configurations, token lengths, and parser details
- **Data Ingestion** — Force sync remote files from SQL, Cloud Storage, or APIs into your vector space to update your knowledge base
- **RAG Queries** — Dispatch automated AI questions that query your vector store and synthesize accurate answers from stored context
- **Chunk Auditing** — Perform lexical or semantic searches to pull raw document chunks and verify precise text segments
- **Model Registry** — Enumerate available LLMs and embedding models registered inside your modular Cognita installation
- **DataSource Management** — List all connected data sources to verify which external data is mapped into your AI workflows

### How it works

1. Subscribe to this server
2. Enter your Cognita Base URL and API Key (if required by your TrueFoundry or self-hosted setup)
3. Start managing your RAG pipelines from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **AI Engineers** — test and debug RAG queries and chunk retrieval logic without writing Python scripts
- **Data Scientists** — monitor ingestion pipelines and verify document chunking consistency across collections
- **Product Teams** — quickly audit what knowledge is being fed to AI agents during the prototyping phase
- **DevOps Teams** — monitor Cognita model registries and ensure that all LLM endpoints are active and reachable


## Available Tools (7)
- **rag_query**: Identify precise active arrays spanning rented Transformation vectors
- **list_models**: Inspect deep internal arrays mitigating specific Picture constraints
- **list_collections**: Identify bounded routing spaces inside the Headless Cognita RAG limit
- **get_collection**: Retrieve explicit Cloud logging tracing explicit Payload IDs
- **list_data_sources**: Perform structural extraction of properties driving active Buckets
- **ingest_data**: Provision a highly-available JSON Payload generating new Resource directories
- **search_chunks**: Enumerate explicitly attached structured rules exporting active Presets


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Cognita (RAG Framework)** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all RAG collections in Cognita"

**🤖 AI Agent:**
> I found 3 collections: 'technical-docs', 'legal-kb', and 'customer-support'. Which one would you like to inspect for metadata?

---

**👤 You:**
> "Query collection 'technical-docs' for: 'How do I configure OAuth in our API?'"

**🤖 AI Agent:**
> Based on your technical docs, you need to navigate to the /auth/settings endpoint and register a new client ID. [Detailed answer synthesized from 3 context chunks].

---

**👤 You:**
> "Ingest data from source 'gh-repo-vinkius' into collection 'technical-docs'"

**🤖 AI Agent:**
> Ingestion pipeline triggered! Cognita is now syncing 'gh-repo-vinkius' into the 'technical-docs' collection. I will let you know once the knowledge base is updated.


## ❓ FAQ

**Q: Can my agent perform semantic RAG queries against my collections?**
Yes. The 'rag_query' tool allows you to ask questions in natural language. The agent queries your vector store via Cognita and uses an LLM to synthesize a final answer based explicitly on the retrieved context.

**Q: How can I trigger a data ingestion pipeline through the agent?**
Provide the collection name and the data source FQN (Fully Qualified Name). The 'ingest_data' tool will command the Cognita backend to start a sync, updating your RAG vector space with the latest remote documents.

**Q: Can I audit the raw document chunks before LLM generation?**
Absolutely. Use the 'search_chunks' tool to perform vector searches that return raw text segments and metadata without LLM synthesis. This is the perfect way to verify that your retrieval logic is pulling the correct data boundaries.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/cognita-rag-framework](https://vinkius.com/mcp/cognita-rag-framework)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Cognita (RAG Framework)** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `cognita-rag-framework` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Cognita (RAG Framework)** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "cognita-rag-framework": {
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
