# Cohere (Embed & Rerank) MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/cohere-embed-rerank)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [ai-frontier](../categories/ai-frontier.md)

Empower RAG via Cohere — generate high-quality text embeddings, rerank documents for better accuracy, and perform AI classification directly from any AI agent.

## Description
Connect your **Cohere** account to any AI agent and take full control of your enterprise AI and RAG workflows through natural conversation.

### What you can do

- **Text Embeddings** — Generate precise dense vector shapes for plain strings to power semantic search and knowledge retrieval
- **Semantic Reranking** — Structure contextual chunks by priority ordering documents against specific queries for improved RAG accuracy
- **Conversational AI** — Execute formatted conversational transformations using Cohere's generation limits and state-of-the-art LLMs
- **Text Classification** — Categorize inputs into predefined labels using few-shot training blocks and extract confidence scores
- **Tokenization** — Retrieve exact structural segmentation of NLP contexts to audit token counts and model dictionaries
- **Model Registry** — Enumerate available Cohere models and hashes to verify API availability based on your plan

### How it works

1. Subscribe to this server
2. Enter your Cohere API Key (Trial or Production key from the Dashboard)
3. Start optimizing your RAG pipelines from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **AI Developers** — test and debug embedding and reranking logic without writing boilerplate code
- **Data Scientists** — evaluate semantic matching accuracy and text classification confidence in real-time
- **Product Teams** — quickly prototype search and retrieval features using enterprise-grade AI models
- **LLM Engineers** — audit tokenization and model availability for complex conversational workflows


## Available Tools (5)
- **list_models**: List all available Cohere models on your plan
- **tokenize_text**: Tokenize text into token IDs for a specific model
- **embed_texts**: Generate dense vector embeddings from text using Cohere models
- **rerank_documents**: Rerank documents by semantic relevance to a query
- **chat_completion**: Generate conversational text responses using Cohere chat models


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Cohere (Embed & Rerank)** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Generate embeddings for these texts: ['Hello world', 'Artificial Intelligence']"

**🤖 AI Agent:**
> Embeddings generated! I've retrieved the dense vector representations for both strings. You can now use these floats for semantic search or similarity calculations.

---

**👤 You:**
> "Rerank these documents for query 'Best pizza in NY': ['Pizza hut review', 'Joe's Pizza is the local favorite']"

**🤖 AI Agent:**
> Reranking complete! 'Joe's Pizza is the local favorite' has been moved to rank 0 with a high relevance score. 'Pizza hut review' is now at rank 1.

---

**👤 You:**
> "How many tokens are in the text: 'The quick brown fox jumps over the lazy dog'?"

**🤖 AI Agent:**
> That sentence contains 9 tokens according to the Cohere tokenizer. I can provide the exact integer array mapping these tokens if you'd like.


## ❓ FAQ

**Q: Can my agent improve my RAG system's accuracy using Cohere?**
Yes. The 'rerank_documents' tool is specifically designed for this. Provide a query and a list of documents, and Cohere will reorder them based on semantic relevance, ensuring the most accurate context is fed to your LLM.

**Q: How do I test text classification via the agent?**
Use the 'classify_texts' tool. Provide your input strings and a few-shot JSON array of examples (text and label). The agent will return the predicted categories along with confidence scores from the Cohere engine.

**Q: What is the difference between Trial and Production keys?**
Trial keys are free for development but have strict rate limits (approx. 1,000 calls per month). Production keys remove these limits but require a paid plan. Both types work seamlessly with this server.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/cohere-embed-rerank](https://vinkius.com/mcp/cohere-embed-rerank)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Cohere (Embed & Rerank)** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `cohere-embed-rerank` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Cohere (Embed & Rerank)** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "cohere-embed-rerank": {
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
