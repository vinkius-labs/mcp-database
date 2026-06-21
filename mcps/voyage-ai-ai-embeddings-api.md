# Voyage AI (AI Embeddings API) MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/voyage-ai-ai-embeddings-api)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/voyage-ai-ai-embeddings-api-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/voyage-ai-ai-embeddings-api-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [developer-tools](../categories/developer-tools.md)

Generate high-quality text, multimodal, and contextualized embeddings, plus high-precision reranking for RAG workflows.

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


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Voyage AI (AI Embeddings API)** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Create embeddings for the text 'What are the benefits of vector search?' using the voyage-4 model."

**🤖 AI Agent:**
> I've generated the embeddings for your text using `voyage-4`. The output includes a high-dimensional vector ready for your vector database or similarity search.

---

**👤 You:**
> "Rerank these documents ["Doc A content...", "Doc B content..."] for the query 'AI safety' using rerank-2.5."

**🤖 AI Agent:**
> I've reranked the documents. Doc B scored significantly higher (0.92) than Doc A (0.45) for the query 'AI safety'. You should prioritize Doc B in your response.

---

**👤 You:**
> "Start a batch embedding job for the file 'file-987' using the embeddings endpoint."

**🤖 AI Agent:**
> The batch job has been initiated successfully. You can monitor its progress using the `get_batch` tool with the ID: `batch_v1_abc123`.


## Installation & Usage

To install and use the **Voyage AI (AI Embeddings API)** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/voyage-ai-ai-embeddings-api](https://vinkius.com/mcp/voyage-ai-ai-embeddings-api)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
