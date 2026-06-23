# Wikidata MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/wikidata)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [the-unthinkable](../categories/the-unthinkable.md)

Access the world's largest open knowledge graph—query entities via SPARQL, perform vector searches, and manage structured data directly from your AI agent.

## Description
Connect to **Wikidata**, the central storage for structured data of Wikimedia projects. This MCP server allows your AI agent to tap into millions of items, properties, and statements using both traditional SPARQL queries and modern vector-based semantic search.

### What you can do

- **Entity Retrieval** — Fetch full data and statements for any Wikidata Item (e.g., Q42) using the `get_item` and `get_item_statements` tools.
- **Advanced Querying** — Execute complex SPARQL queries against the Wikidata Query Service (WDQS) with `execute_sparql` to find relationships and patterns across the entire graph.
- **Semantic Search** — Use `search_items_vector` and `search_properties_vector` to find entities and properties based on meaning rather than just exact keywords.
- **Data Contribution** — Update the knowledge graph by creating statements or setting descriptions with `create_statement` and `set_item_description` (requires OAuth).
- **Similarity Analysis** — Compare text strings against specific entities to get semantic similarity scores using `get_similarity_score`.

### How it works

1. Subscribe to this server
2. Provide your **User Agent** (required by Wikimedia policy)
3. Optionally provide an **OAuth 2.0 Access Token** for write operations
4. Start exploring the world's knowledge from your favorite AI client

### Who is this for?

- **Researchers & Academics** — instantly verify facts, dates, and relationships across history, science, and culture.
- **Data Scientists** — extract structured datasets for analysis or training without leaving the chat interface.
- **Developers** — find entity IDs and property schemas to integrate into applications or automate data enrichment.


## Available Tools (8)
- **create_statement**: Requires OAuth 2.0 Access Token.

Create a new statement for an Item
- **execute_sparql**: Use hint:Query hint:optimizer "None" if queries timeout.

Execute a SPARQL query
- **get_item_statements**: Retrieve statements for a Wikidata Item
- **get_item**: g., Q42) via the Wikibase REST API.

Retrieve a specific Wikidata Item
- **get_similarity_score**: Compute similarity between text and an entity
- **search_items_vector**: Hybrid vector/keyword search for Items
- **search_properties_vector**: Hybrid vector/keyword search for Properties
- **set_item_description**: Requires OAuth 2.0 Access Token.

Set an Item description


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Wikidata** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Search for Wikidata items related to 'artificial neural networks' using vector search."

**🤖 AI Agent:**
> I've performed a vector search for 'artificial neural networks'. The most relevant item is 'artificial neural network' (Q192713), described as a computational model inspired by biological neural networks. Other related items include 'deep learning' (Q197536) and 'machine learning' (Q11660).

---

**👤 You:**
> "Run a SPARQL query to find the 5 most populated cities in Brazil."

**🤖 AI Agent:**
> Executing the SPARQL query... The 5 most populated cities in Brazil are: 1. São Paulo (Q174), 2. Rio de Janeiro (Q8678), 3. Brasília (Q2844), 4. Salvador (Q36851), and 5. Fortaleza (Q43463).

---

**👤 You:**
> "Get all statements for the Wikidata item Q42."

**🤖 AI Agent:**
> I've retrieved the statements for Douglas Adams (Q42). Key statements include: instance of 'human' (P31), occupation 'writer' (P106), and notable work 'The Hitchhiker's Guide to the Galaxy' (P800).


## ❓ FAQ

**Q: How can I find a Wikidata Item if I don't know its Q-ID?**
You can use the `search_items_vector` tool. It performs a hybrid search using high-dimensional embeddings and keywords to find the most relevant entities based on your natural language description.

**Q: Is it possible to run complex queries like 'List all female scientists born in the 19th century'?**
Yes, the `execute_sparql` tool allows you to run any valid SPARQL query against the Wikidata Query Service. This is the most powerful way to filter and aggregate data across the entire knowledge graph.

**Q: Can I use this server to update information on Wikidata?**
Yes, if you provide an OAuth 2.0 Access Token, you can use `create_statement` to add new data or `set_item_description` to update descriptions in various languages.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/wikidata](https://vinkius.com/mcp/wikidata)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Wikidata** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `wikidata` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Wikidata** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "wikidata": {
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
