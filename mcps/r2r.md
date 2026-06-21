# R2R MCP Server

Equip your AI with direct access to your R2R engine — execute vector searches, run precise RAG queries, and manage your documents.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/r2r)

## Overview
**Category:** friends-mcp
**Tools Count:** 6

## Description
Connect your **R2R (Rag to Riches)** deployment to an AI agent, bringing your RAG infrastructure inside your chat interface. By linking this server, the AI can query its own constructed knowledge base on demand.

### What you can do

- **Vector Search** — Perform semantic similarity queries across your document database to retrieve contextually relevant chunks of information.
- **Execute RAG Queries** — Use the 'rag_query' endpoint to have the R2R server directly summarize information based on vector data.
- **Knowledge Management** — Call the API to list ingested documents, read metadata attributes, and filter logical collections.
- **Instance Health Monitoring** — Quickly ping the connection using health checks to verify your system is responsive.

### How it works

1. Enable the server integration.
2. Provide your active R2R Base URL and Auth Key (if applicable).
3. Trigger RAG requests natively within your supported chat interfaces.

### Who is this for?

- **AI & ML Engineers** — Query your vector instances locally without needing Postman or external scripts.
- **Data Custodians** — Quickly verify document ingestions and browse metadata directly inside the terminal.
- **Backend Developers** — Audit engine responses and fine-tune semantic retrieval limits easily.


## Available Tools
- **search**: Performs a vector search across ingested documents
- **rag_query**: Executes a RAG (Retrieval-Augmented Generation) query
- **list_documents**: Lists all ingested documents in the R2R system
- **get_document**: Retrieves details for a specific document
- **list_collections**: Lists all document collections
- **get_health**: Checks the health status of the R2R server


## Installation & Usage

To install and use the **R2R** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/r2r](https://vinkius.com/mcp/r2r)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
