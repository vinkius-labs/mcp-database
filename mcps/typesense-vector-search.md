# Typesense Vector Search MCP Server

Automate vector similarity searches via Typesense — index documents, manage collections, and execute semantic queries directly from your AI agent.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/typesense-vector-search)

## Overview
**Category:** loved-by-devs
**Tools Count:** 6

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


## Available Tools
- **create_collection**: Provide the schema details as a JSON object.

Creates a new search collection with a specific schema
- **delete_document**: This action is irreversible.

Permanently removes a document from a collection by its ID
- **get_collection_details**: Retrieves schema and metadata for a specific collection
- **index_document**: Provide the collection name and the document data as a JSON object.

Adds or updates a document in a search collection
- **list_vector_collections**: Lists all collections in the Typesense instance
- **search_vectors**: Provide the collection name, a text query, and a vector_query string (e.g., "vec:(0.1, 0.2, ...)").

Performs a vector similarity search combined with optional text filtering


## Installation & Usage

To install and use the **Typesense Vector Search** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/typesense-vector-search](https://vinkius.com/mcp/typesense-vector-search)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
