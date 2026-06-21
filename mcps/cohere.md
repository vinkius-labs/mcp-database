# Cohere MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/cohere)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [ai-frontier](../categories/ai-frontier.md)

Access Cohere AI models via API — chat with Command models, generate embeddings, rerank documents and tokenize text from any AI agent.

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


## Available Tools (6)
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


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Cohere** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Send a message to Command R+ asking 'What is the capital of Brazil?'"

**🤖 AI Agent:**
> Command R+ responded: 'The capital of Brazil is Brasília. It was purpose-built to replace Rio de Janeiro as the capital in 1960, and is located in the country's central-west region.'

---

**👤 You:**
> "Rerank these documents for the query 'machine learning models': ['Neural networks are inspired by biological neurons.', 'Python is a popular programming language.', 'Transformers use attention mechanisms for sequence processing.']"

**🤖 AI Agent:**
> Reranked results: 1. 'Transformers use attention mechanisms...' (score: 0.95), 2. 'Neural networks are inspired...' (score: 0.72), 3. 'Python is a popular...' (score: 0.12). The transformer and neural network documents are most relevant to ML models.

---

**👤 You:**
> "Generate embeddings for these texts: ['The weather is nice today.', 'I love programming in Python.'] using embed-v4."

**🤖 AI Agent:**
> Generated embeddings for 2 texts using embed-v4 with input_type 'search_document'. Each embedding is a 1024-dimensional vector. You can use these for semantic search, similarity comparison or vector database storage.


## ❓ FAQ

**Q: How do I get a Cohere API Key?**
Log in to the [**Cohere Dashboard**](https://dashboard.cohere.com/api-keys), go to **API Keys** and click **Create API Key**. Copy the key immediately — it starts with a random string and won't be shown again. Free tier includes trial access with rate limits.

**Q: What models are available?**
Use the `list_models` tool to see all available Cohere models. Key models include command-r-plus (most capable, 128K context), command-r (efficient, 128K context), command-r7b (lightweight, 128K context), embed-v4 (embeddings) and rerank-v3.5 (reranking).

**Q: Can I send multi-turn conversations?**
Yes! Pass a messages array with alternating 'user', 'assistant' and 'system' roles. Each message has a 'role' and 'content' field. Command models support function calling and will return tool_calls when appropriate.

**Q: What is reranking and when should I use it?**
Reranking reorders a set of documents by their relevance to a query. Use it after an initial search to improve result quality. The rerank tool takes a query, list of documents and returns them ranked by relevance score. Cohere's rerank models are industry-leading for search applications.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/cohere](https://vinkius.com/mcp/cohere)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Cohere** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `cohere` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Cohere** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "cohere": {
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
