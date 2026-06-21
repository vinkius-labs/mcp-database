# Vectara MCP Server

Empower your agent with Vectara's RAG capabilities. Search corpora natively, execute grounded chats, and manage indexed datasets easily.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/vectara)

## Overview
**Category:** ai-frontier
**Tools Count:** 7

## Description
Connect your **Vectara** environment to any AI agent to unlock enterprise-grade Retrieval-Augmented Generation (RAG) and semantic search directly inside your conversational IDE or workspace.

### What you can do

- **Semantic Search** — Query your indexed private corpora naturally and return highly relevant, grounded documents without traditional keyword matching limitations.
- **Conversational RAG** — Execute fully-fledged interactive chats leveraging Vectara's backend to provide detailed, cited answers strictly based on your secure documents.
- **Corpus Management** — List all available data corpora, retrieve unique keys, and discover the shape of your indexed data environment on the fly.
- **Document Auditing** — Monitor specific document indexes within a corpus, verify correct ingestions, or permanently delete obsolete files avoiding polluted search results.

### How it works

1. Subscribe to this server
2. Enter your Vectara API Key and Customer ID
3. Start retrieving knowledge from Claude, Cursor, or any MCP-compatible client

Your AI agent becomes an elite cognitive search gateway to all your internal data.

### Who is this for?

- **Software Engineers** — debug RAG implementation challenges by directly testing `query` responses via chat instead of writing disposable test scripts.
- **Data Engineers** — securely remove stale database context arrays manually inserted into Vectara via quick conversational text commands.
- **Product Leads** — ask questions against internal product manuals stored as a Vectara corpus without waiting for the frontend UI development.
- **Technical Writers** — locate specific passages traversing across thousands of embedded documents effortlessly leveraging contextual semantic queries.


## Available Tools
- **execute_rag_chat**: Provide corpus keys and the user query to get a summarized AI response with citations.

Executes a RAG-powered chat completion
- **delete_corpus_document**: This action is irreversible.

Permanently removes a document from a corpus
- **get_corpus_details**: Retrieves metadata and configuration for a specific corpus
- **list_chat_sessions**: Lists previous RAG chat sessions
- **list_corpora**: Lists all corpora (searchable datasets) in the Vectara account
- **list_corpus_documents**: Lists all indexed documents within a specific corpus
- **perform_semantic_search**: Provide one or more comma-separated corpus keys and the query text.

Executes a semantic search across one or more corpora


## Installation & Usage

To install and use the **Vectara** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/vectara](https://vinkius.com/mcp/vectara)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
