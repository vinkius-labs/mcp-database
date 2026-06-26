# Typesense Vector Search MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/typesense-vector-search)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [loved-by-devs](../categories/loved-by-devs.md)

Automate vector similarity searches via Typesense — index documents, manage collections, and execute semantic queries directly from your AI agent.

## Description
Connect your **Typesense Vector Search** environment to any AI agent and take full autonomous control over vector collections, indexing processes, and semantic querying through daily conversation.

### What you can do

- **Vector Semantic Search** — Issue combined text-filtering alongside vector similarity (`vec`) queries natively through chat
- **Collection Provisioning** — Instantly create new semantic schema datasets holding complex vector embedding structures organically
- **Document Indexing** — Let your AI insert or update JSON payloads into your database, bypassing manual code-level REST integrations
- **Schema & Records Insights** — Retrieve absolute schema geometries mapping collections to ensure developers map fields correctly

### How it works

1. Subscribe to this connected MCP server
2. Provide your active Typesense Host URL alongside an Admin API Key
3. Start fetching vector similarities natively across Claude, Cursor, or your specific MCP workspace

No digging into CURL terminal payloads or writing Python scripts for basic document mutations. Your agent performs all indexation logic flawlessly.

### Who is this for?

- **AI Application Builders** — prompt the agent to create semantic collections supporting `float[]` logic seamlessly
- **Data Engineers** — let the AI ingest missing RAG reference documents manually into a running collection
- **Backend Devs** — perform sanity checks and text-filtered semantic searches inspecting exact relevance scores


## Available Tools (6)
- **search_vectors**: Provide the collection name, a text query, and a vector_query string (e.g., "vec:(0.1, 0.2, ...)").

Performs a vector similarity search combined with optional text filtering
- **create_collection**: Provide the schema details as a JSON object.

Creates a new search collection with a specific schema
- **delete_document**: This action is irreversible.

Permanently removes a document from a collection by its ID
- **get_collection_details**: Retrieves schema and metadata for a specific collection
- **index_document**: Provide the collection name and the document data as a JSON object.

Adds or updates a document in a search collection
- **list_vector_collections**: Lists all collections in the Typesense instance


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Typesense Vector Search** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all active collections on this vector cluster. Do I have any collections initialized yet?"

**🤖 AI Agent:**
> I've listed 2 active collections: 'customer_kb_index' (configured with a 1536-dimensional embedding schema) and 'products_inventory'. Need me to execute a vector search on either limit?

---

**👤 You:**
> "I have an embedding snippet: [0.34, 0.42, 0.99...]. Delete the document carrying ID 'test-123' and re-index it using this JSON data on collection 'faqs'."

**🤖 AI Agent:**
> Document 'test-123' has been successfully wiped. I've seamlessly pushed the new JSON package into 'faqs', updating the embedding vectors as instructed.

---

**👤 You:**
> "Explain the schema definitions used inside the 'products_inventory' collection."

**🤖 AI Agent:**
> The collection 'products_inventory' uses 4 strict fields: `product_id` (string), `name` (string), `popularity` (int32), and critically `embeddings` formulated as a `float[]` of 768 dimensions representing product semantics.


## ❓ FAQ

**Q: Can the agent perform vector plus text-filtering search combined natively?**
Yes. Provide the agent with the collection name alongside the text payload and tell it the exact vector structure. It leverages internal filters querying natively and returns the nearest neighbors with exact accuracy scores.

**Q: How do I make the AI create a semantic collection ready for embeddings (OpenAI 1536 dims)?**
Ask the agent to use 'create_collection'. Provide standard JSON declaring the name, the field structure, and explicitly define the `float[]` field tracking the 1536 dims length. The cluster will spin the framework up instantly.

**Q: Can it delete problematic vectors holding bad geometry data manually?**
Absolutely. Supplying the explicit collection target and the item 'id' to the delete_document prompt securely wipes out all traces from the dataset. Use this sparingly as it can't be undone easily.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/typesense-vector-search](https://vinkius.com/mcp/typesense-vector-search)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Typesense Vector Search** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `typesense-vector-search` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Typesense Vector Search** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "typesense-vector-search": {
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
