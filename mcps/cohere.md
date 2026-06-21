# Cohere MCP Server

Access Cohere AI models via API — chat with Command models, generate embeddings, rerank documents and tokenize text from any AI agent.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/cohere)

## Overview
**Category:** ai-frontier
**Tools Count:** 6

## Description
Connect your **Cohere** account to any AI agent and leverage enterprise-grade AI models through natural conversation.

### What you can do

- **Model Discovery** — List all available Cohere models with their names, capabilities and context lengths
- **Chat API** — Send conversations to Command models (command-r-plus, command-r, command-r7b) and receive responses with citations and tool call support
- **Embeddings** — Generate vector embeddings for semantic search with multiple embedding types (float, int8, uint8, binary)
- **Reranking** — Rerank documents by relevance to a search query using Cohere's industry-leading reranking models
- **Tokenization** — Tokenize and detokenize text for estimating token counts and debugging

### How it works

1. Subscribe to this server
2. Enter your Cohere API Key
3. Start using Cohere models from Claude, Cursor, or any MCP-compatible client

No more switching between API tools to interact with Cohere. Your AI acts as an LLM orchestration layer.

### Who is this for?

- **Developers** — quickly send messages to Command models, generate embeddings and rerank search results without writing HTTP code
- **ML Engineers** — discover available models, compare capabilities and generate embeddings with multiple types (float, int8, binary)
- **Search Teams** — rerank documents by relevance, tokenize text and generate embeddings for search index building


## Available Tools
- **chat**: Requires the model ID (e.g. "command-r-plus", "command-r", "command-r7b") and messages array in JSON format. Each message must have a "role" ("user", "assistant", "system" or "tool") and "content" (text or array of content blocks). Optionally set max_tokens, temperature (0-1), p (nucleus sampling 0-1) and tools array for function calling. Returns the model's response with text, citations and tool calls.

Send a chat message to a Cohere model
- **detokenize**: Requires the token IDs array. Returns the reconstructed text. Useful for debugging and verifying tokenization.

Detokenize token IDs back to text using Cohere
- **embed**: Requires the model ID (e.g. "embed-v4", "embed-v3"), texts array and input_type ("search_document", "search_query", "classification", "clustering"). Returns embedding vectors for each input text. Useful for semantic search, similarity comparison and vector database storage.

Generate embeddings using Cohere
- **list_models**: Each model returns its name (e.g. "command-r-plus", "command-r", "embed-v4", "rerank-v3.5"), endpoint compatibility, context length and tokenization info. Use this to discover which models are available and their capabilities.

List all available Cohere models
- **rerank**: Requires the model ID (e.g. "rerank-v3.5", "rerank-english-v3.0"), query text and documents array. Optionally set top_n to return only the top N results. Returns ranked documents with relevance scores.

Rerank documents by relevance to a query
- **tokenize**: Requires the text to tokenize and optionally the model. Returns the list of token IDs and token strings. Useful for estimating token counts before sending to chat or embed endpoints.

Tokenize text using Cohere


## Installation & Usage

To install and use the **Cohere** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/cohere](https://vinkius.com/mcp/cohere)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
