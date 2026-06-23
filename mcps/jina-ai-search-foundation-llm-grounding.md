# Jina AI (Search Foundation & LLM Grounding) MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/jina-ai-search-foundation-llm-grounding)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [ai-frontier](../categories/ai-frontier.md)

Power your RAG and search via Jina AI — generate embeddings, rerank documents, read URLs, and perform semantic web search.

## Description
Connect your **Jina AI** account to any AI agent and take full control of state-of-the-art search infrastructure and LLM grounding through natural conversation.

### What you can do

- **LLM Grounding & Reader** — Extract clean, readable Markdown context from any web URL, stripping away noise and navigation to feed high-quality data to your agent
- **Semantic Web Search** — Perform context-rich web searches that return structured results specifically optimized for RAG pipelines and AI analysis
- **Vector Embeddings** — Generate high-quality embeddings using Jina's advanced models to power semantic search and document similarity workflows
- **Precision Reranking** — Improve search relevance by re-ordering candidate documents based on their semantic match to a specific query block
- **Zero-Shot Classification** — Categorize text inputs against custom labels with confidence scores without training specific models manually
- **Intelligent Segmentation** — Break down long documents into semantically cohesive chunks to optimize retrieval-augmented generation (RAG)

### How it works

1. Subscribe to this server
2. Enter your Jina AI API Key
3. Start grounding your AI with real-time web intelligence from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **AI & RAG Developers** — provide your agents with real-time web access and precise document retrieval capabilities through natural conversation
- **Data Scientists** — test embedding models and reranking logic without writing manual Python scripts or using curl
- **Automation Engineers** — automate the extraction of clean web content and semantic classification for large-scale data pipelines


## Available Tools (6)
- **generate_embeddings**: The input must be a JSON array of strings.

Generate vector embeddings from text
- **rerank_documents**: Rerank search documents against a query
- **read_url_content**: Excellent for grounding LLMs with live web content.

Read and extract clean text from a URL
- **search_web_jina**: Returns context-rich structured search results, suitable for RAG pipelines.

Perform a semantic web search
- **classify_texts**: Perform zero-shot text classification
- **segment_content**: Semantically segment and chunk long text content


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Jina AI (Search Foundation & LLM Grounding)** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Extract the main content from 'https://jina.ai/embeddings' as Markdown"

**🤖 AI Agent:**
> Reading URL… I've extracted the clean text from the page. It covers Jina's embedding models (v2 and v3), multilingual support for 80+ languages, and common use cases like semantic search and recommendation systems. Would you like a summary?

---

**👤 You:**
> "Search the web for the latest updates on 'DeepSeek-V3 architecture'"

**🤖 AI Agent:**
> Searching the web… Based on the structured results from Jina Search, DeepSeek-V3 features a Multi-head Latent Attention (MLA) mechanism and a Mixture-of-Experts (MoE) architecture with 671B total parameters. Would you like me to read the full technical paper URL?

---

**👤 You:**
> "Segment this long text into semantically cohesive chunks: [text content]"

**🤖 AI Agent:**
> Segmenting content… I've broken your text into 5 semantically distinct segments. Each segment focuses on a single core topic (e.g., Introduction, Architecture, Benchmarks). This is now optimized for vector storage and RAG retrieval.


## ❓ FAQ

**Q: How can Jina AI help my agent provide more accurate answers?**
Use the `read_url_content` tool to give your agent access to live web data. By converting URLs into clean Markdown, your agent can 'read' the latest information from documentation or news sites, grounding its answers in up-to-date facts.

**Q: What is the difference between search and rerank?**
Search (embeddings) helps you find a broad set of relevant documents quickly. Rerank takes that smaller set and uses a more powerful cross-encoder model to sort them by exact semantic matching, ensuring the absolute best context is sent to the LLM.

**Q: Can I search the web through my agent using Jina?**
Absolutely. Use the `search_web_jina` tool to dispatch a semantic query. Your agent will return structured results including snippets and titles from top web pages, allowing it to synthesize answers from the live internet.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/jina-ai-search-foundation-llm-grounding](https://vinkius.com/mcp/jina-ai-search-foundation-llm-grounding)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Jina AI (Search Foundation & LLM Grounding)** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `jina-ai-search-foundation-llm-grounding` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Jina AI (Search Foundation & LLM Grounding)** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "jina-ai-search-foundation-llm-grounding": {
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
