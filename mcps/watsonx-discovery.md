# watsonx Discovery MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/watsonx-discovery)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [industry-titans](../categories/industry-titans.md)

Search and analyze complex data with AI-powered insights on IBM watsonx Discovery — the cognitive search engine.

## Description
Connect your **IBM watsonx Discovery** account to any AI agent and harness the power of cognitive search and NLP-driven text analytics through natural conversation.

### What you can do

- **Cognitive Search** — Perform natural language or Discovery Query Language (DQL) queries against your data collections for high-quality semantic search
- **Data Discovery** — Browse and list all data collections within your project to retrieve collection and document IDs
- **Document Analysis** — Retrieve comprehensive metadata, ingestion status, and technical details for specific indexed documents
- **NLP Enrichments** — List and monitor available enrichments (NLP models) like Sentiment, Entities, and Keywords being applied to your data
- **Component Health** — Verify project-level configurations, ingestion notices, and health settings for all project components
- **Semantic Insights** — Surface relevant information and hidden patterns from massive unstructured datasets through simple chat commands

### How it works

1. Subscribe to this server
2. Enter your watsonx URL, API Key, and Project ID
3. Start querying your cognitive data collections through Claude, Cursor, or any MCP-compatible client

No more manual digging through complex IBM Cloud consoles to query your data. Your AI agent becomes your cognitive data scientist.

### Who is this for?

- **Enterprise Developers** — build grounded AI applications using Discovery's semantic search and ingestion pipelines
- **Knowledge Analysts** — quickly surface information from large document repositories and audit NLP enrichments
- **Data Scientists** — test and refine DQL queries and monitor data ingestion status through chat
- **Product Teams** — implement AI-powered search features and monitor the health of your discovery project


## Available Tools
- **get_document_details**: Retrieves metadata and status for a specific indexed document
- **get_component_settings**: Retrieves the configuration and health settings for project components
- **list_discovery_collections**: Lists all data collections within the current watsonx Discovery project
- **list_collection_documents**: Lists all documents indexed within a specific collection
- **list_available_enrichments**: g., Sentiment, Entities) are being applied to documents.

Lists all enrichments (NLP models) configured for the project
- **query_discovery_content**: Provide a collection ID and the query text.

Performs a natural language or DQL query against a discovery collection


## 💬 Prompt Examples

Here are some examples of how you can interact with the **watsonx Discovery** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all my Discovery collections."

**🤖 AI Agent:**
> I found 3 collections in your project: 'Legal Documents' (ID: col-1), 'Technical Support KB' (ID: col-2), and 'Marketing Research' (ID: col-3). Which one would you like to query?

---

**👤 You:**
> "Search the 'Legal Documents' collection for 'contract termination clauses'."

**🤖 AI Agent:**
> I found several matches. The most relevant document mentions that termination requires a 30-day written notice and highlights specific liability limitations. Would you like me to pull the full document text?

---

**👤 You:**
> "What enrichments are currently active in my project?"

**🤖 AI Agent:**
> Your project has 4 active NLP enrichments: 1. Sentiment Analysis, 2. Entity Extraction (People, Places, Organizations), 3. Category Classification, and 4. Keyword Extraction. These are applied to all documents during ingestion.


## ❓ FAQ

**Q: Can I query my data collections using natural language?**
Yes. The `query_discovery_content` tool allows your AI agent to perform natural language queries against your watsonx Discovery collections, returning highly relevant results based on IBM's cognitive search engine.

**Q: How do I see what NLP models are being applied to my documents?**
Use the `list_available_enrichments` tool to see all NLP enrichments (like Sentiment, Entity Extraction, or Category Classification) configured for your project and applied during the ingestion pipeline.

**Q: Can I monitor the ingestion status of a specific document?**
Absolutely. Using the `get_document_details` tool, you can check the ingestion status and technical metadata for any specific document ID, ensuring your data is correctly indexed and searchable.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/watsonx-discovery](https://vinkius.com/mcp/watsonx-discovery)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **watsonx Discovery** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `watsonx-discovery` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **watsonx Discovery** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "watsonx-discovery": {
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
