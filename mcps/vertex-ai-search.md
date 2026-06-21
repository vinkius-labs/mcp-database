# Vertex AI Search MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/vertex-ai-search)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/vertex-ai-search-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/vertex-ai-search-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [ai-frontier](../categories/ai-frontier.md)

Search across your enterprise data using Google's semantic search and generative AI grounding.

## Description
Connect your **Vertex AI Search** account to any AI agent and harness the power of Google's semantic search technology on your own enterprise data through natural conversation.

### What you can do

- **Semantic Search** — Perform high-quality semantic searches across documents with AI-powered relevance and accuracy
- **Grounded Answers** — Get direct, natural language answers grounded in your private document collection for reliable Q&A
- **Data Stores** — List and browse your enterprise data stores and search engines to manage your searchable datasets
- **Document Discovery** — Browse and list indexed documents within your data store branches directly from your agent
- **Personalized Recommendations** — Retrieve intelligent recommendations based on user interaction events and patterns
- **Search Engines** — View and manage high-level search applications configured for specific business use cases

### How it works

1. Subscribe to this server
2. Enter your Google Cloud Project ID, Location, and Access Token
3. Start querying your enterprise data through Claude, Cursor, or any MCP-compatible client

No more manual digging through complex documentation systems. Your AI agent becomes your enterprise knowledge expert.

### Who is this for?

- **Enterprise Developers** — build grounded AI applications using internal documentation and knowledge bases without manual indexing
- **Knowledge Managers** — quickly surface relevant information from massive document repositories through simple conversation
- **Data Scientists** — rapidly test and refine search relevance and generative grounding configurations
- **Product Teams** — implement personalized recommendations and AI-powered search features with minimal friction


## Available Tools
- **get_grounded_answer**: Returns a natural language response based on your private data.

Retrieves an AI-generated answer grounded in the documents of a data store
- **get_datastore_details**: Retrieves configuration and metadata for a specific data store
- **list_data_stores**: Lists all data stores in the Vertex AI Search collection
- **list_datastore_documents**: Provide data store and branch IDs.

Lists all indexed documents within a specific data store branch
- **list_search_engines**: Lists all search engines configured in the collection
- **get_recommendations**: Provide a data store ID and user event data as a JSON object.

Retrieves personalized recommendations based on user events
- **search_documents**: Provide a data store ID and the query text.

Performs a search query across documents in a specific data store


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Vertex AI Search** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all my available data stores in Vertex AI Search."

**🤖 AI Agent:**
> I found 3 data stores: 'documentation-v1' (ID: doc-123), 'hr-policies' (ID: hr-456), and 'product-catalog' (ID: prod-789). Which one would you like to search through?

---

**👤 You:**
> "Based on our documentation, what is our remote work policy?"

**🤖 AI Agent:**
> Grounded in the 'hr-policies' data store: Our remote work policy allows for up to 3 days of work from home per week, provided there is prior alignment with the team manager. Employees must ensure a stable internet connection and maintain core working hours. Would you like me to pull the full document?

---

**👤 You:**
> "Search the product catalog for 'blue wireless headphones'."

**🤖 AI Agent:**
> I found several matches in 'product-catalog': 1. 'CloudBass Pro Blue' (In Stock), 2. 'SkyBuds v2 Azure' (Limited Stock), and 3. 'Oceanic Beats Wireless' (Discontinued). I can provide more details on features or pricing for any of these.


## Installation & Usage

To install and use the **Vertex AI Search** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/vertex-ai-search](https://vinkius.com/mcp/vertex-ai-search)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
