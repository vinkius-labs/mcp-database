# Verba MCP Server

Connect your Verba RAG platform to your AI agent. Search your documents, retrieve semantic answers, and manage your Weaviate knowledge base directly.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/verba)

## Overview
**Category:** knowledge-management
**Tools Count:** 6

## Description
Intertwine the open-source **Verba** (by Weaviate) ecosystem natively into your conversational AI IDE. Execute powerful Retrieval-Augmented Generation processes and manage your localized knowledge bases simply by chatting.

### What you can do

- **Augmented Queries** — Cast a question to your agent and have it retrieve fully synthesized answers from the Verba engine completely backed up by exact document citations.
- **Knowledge Management** — Insert new context text, list all ingested documents, retrieve the deeply embedded raw data of any ID, or remove dead knowledge dynamically without Web UIs.
- **Health Checks** — Request system configurations directly via chat to ensure your local LLM connections, embedding models, and cluster health are firing effectively.

### How it works

1. Ensure your local or cloud Verba instance is running
2. Supply your Verba API URL and API Key (if authenticated)
3. Ask Claude or Cursor to query, retrieve, or insert document structures intuitively.

### Who is this for?

- **RAG Developers** — quickly add or delete text chunks to evaluate changes in embedding fidelity directly inside your IDE coding session.
- **Knowledge Managers** — query your dense technical manuals using semantic search and receive the verified text snippets instantly.
- **Open Source Hobbyists** — orchestrate your personal Weaviate/Verba RAG stacks strictly through the programmatic conversational layer.


## Available Tools
- **add_knowledge_document**: Provide the document content and optional metadata JSON.

Ingests a new document into the Verba knowledge base
- **delete_knowledge_document**: This action is irreversible.

Permanently removes a document from the knowledge base
- **get_document_details**: Retrieves the full content and metadata of a specific document
- **get_system_config**: Retrieves the current Verba system configuration
- **list_knowledge_documents**: Lists all documents indexed in the Verba knowledge base
- **perform_rag_query**: Returns summarized answers with citations.

Executes a RAG (Retrieval Augmented Generation) query against the Verba knowledge base


## Installation & Usage

To install and use the **Verba** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/verba](https://vinkius.com/mcp/verba)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
