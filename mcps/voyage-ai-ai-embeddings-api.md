# Voyage AI (AI Embeddings API) MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/voyage-ai-ai-embeddings-api)
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


## Available Tools (13)
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
- **cancel_batch**: Cancel a batch job
- **create_batch**: Create a batch inference job
- **create_contextualized_embeddings**: Create contextualized chunk embeddings


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


## ❓ FAQ

**Q: How does reranking improve my RAG system's accuracy?**
By using the `rerank` tool, your agent can take a list of potentially relevant documents and re-score them using a powerful cross-encoder model. This ensures that the most semantically relevant pieces of information are ranked first, providing better context for the LLM to answer queries.

**Q: What is the benefit of using contextualized embeddings?**
The `create_contextualized_embeddings` tool allows you to embed chunks of text while considering the surrounding content of the same document. This prevents loss of meaning that often happens with standard chunking, leading to much higher retrieval precision.

**Q: Can I process images and text in the same vector space?**
Yes! With `create_multimodal_embeddings`, you can provide interleaved sequences of text and image URLs. Voyage AI will generate a single embedding that represents the combined semantic meaning, perfect for visual or hybrid search.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/voyage-ai-ai-embeddings-api](https://vinkius.com/mcp/voyage-ai-ai-embeddings-api)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Voyage AI (AI Embeddings API)** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `voyage-ai-ai-embeddings-api` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Voyage AI (AI Embeddings API)** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "voyage-ai-ai-embeddings-api": {
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
