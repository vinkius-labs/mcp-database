# Voyage AI (AI Embeddings API) MCP Server

Generate high-quality text, multimodal, and contextualized embeddings, plus high-precision reranking for RAG workflows.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/voyage-ai-ai-embeddings-api)

## Overview
**Category:** developer-tools
**Tools Count:** 13

## Description
Connect your **Voyage AI** account to any AI agent to leverage state-of-the-art embedding and reranking models. Optimized for Retrieval-Augmented Generation (RAG), this server enables your agent to process complex data structures and find the most relevant information with surgical precision.

### What you can do

- **Advanced Embeddings** — Generate vectors for text, code, and documents using models like `voyage-4` and `voyage-code-3`.
- **Contextualized Retrieval** — Use `voyage-context-3` to embed chunks while maintaining the context of the surrounding document, significantly reducing retrieval errors.
- **Multimodal Search** — Vectorize interleaved text and images into a single vector space for visual search capabilities.
- **Smart Reranking** — Refine search results using cross-encoders (`rerank-2.5`) to ensure the most relevant context is provided to your LLM.
- **Batch Operations** — Manage large-scale data processing by initiating and monitoring batch inference jobs.

### How it works

1. Subscribe to this server
2. Enter your Voyage AI API Key
3. Start building high-performance RAG systems directly from your agent

### Who is this for?

- **AI Engineers** — building production-grade RAG pipelines that require better retrieval than standard embedding models.
- **Data Scientists** — experimenting with multimodal search and contextualized chunking.
- **Developers** — looking to integrate high-precision search into their applications without managing complex infrastructure.


## Available Tools
- **cancel_batch**: Cancel a batch job
- **create_batch**: Create a batch inference job
- **create_contextualized_embeddings**: Create contextualized chunk embeddings
- **create_embeddings**: Create text embeddings
- **create_multimodal_embeddings**: Create multimodal embeddings
- **delete_file**: Delete a file
- **get_batch**: Retrieve batch status
- **get_file_content**: Download file content
- **get_file**: Retrieve file metadata
- **list_batches**: List all batches
- **list_files**: List all files
- **rerank**: Rerank documents against a query
- **upload_file**: Purpose must be "batch".

Upload a file for batch inference


## Installation & Usage

To install and use the **Voyage AI (AI Embeddings API)** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/voyage-ai-ai-embeddings-api](https://vinkius.com/mcp/voyage-ai-ai-embeddings-api)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
