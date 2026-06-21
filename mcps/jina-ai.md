# Jina AI MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/jina-ai)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [ai-frontier](../categories/ai-frontier.md)

Search and read the web for AI — audit search results and reader content via AI.

## Description
Empower your AI agent to orchestrate your entire web intelligence and information retrieval workflow with **Jina AI**, the platform that makes the web readable for machines. By connecting Jina AI to your agent, you transform complex search and reading tasks into a natural conversation. Your agent can instantly search the web for AI-optimized results, audit URL content through high-quality extraction, and rerank documents to maintain a clear view of information relevancy. Whether you are conducting deep research or building advanced RAG pipelines, your agent acts as a real-time data architect, ensuring your intelligence is always grounded in precise, high-density data.

### What you can do

- **Web Auditing** — Query the web using Jina Search and retrieve snippets specifically curated for LLM consumption.
- **Reader Oversight** — Read any URL and retrieve cleaned, LLM-ready content to maintain a structured view of site data.
- **Ranking Intelligence** — Rerank multiple documents or snippets to identify the most relevant information for any specific query.
- **Semantic Intelligence** — Retrieve vector embeddings for text to maintain strict control over semantic search and similarity audits.
- **Fact Checking** — Verify the factuality of statements through Jina's grounded search capabilities.

### How it works

1. Subscribe to this server
2. Enter your Jina AI API Key
3. Start managing your web intelligence through Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **AI Researchers** — monitor search contexts and optimize information retrieval straight from your workflow.
- **Knowledge Engineers** — verify cleaned content from URLs and audit RAG pipeline performance.
- **Data Scientists** — perform rapid audits of semantic embeddings and reranking scores through natural language.
- **Operations Leads** — automate web intelligence querying to orchestrate cross-functional research teams smoothly.


## Available Tools
- **check_fact**: Check the factuality of a statement
- **get_embeddings**: Get vector embeddings for a list of strings
- **read_url**: Read a URL and return cleaned content for LLMs
- **rerank_documents**: Rerank a list of documents based on a query
- **search_web**: Search the web using Jina Search (optimized for AI)
- **tokenize_text**: Tokenize text for LLM processing


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Jina AI** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Search the web for 'best open source LLMs 2024' using Jina AI."

**🤖 AI Agent:**
> I've retrieved the AI-optimized search results. Top matches include Llama 3, Mistral, and Mixtral. Would you like the snippets and links for the top 5 results?

---

**👤 You:**
> "Read the content of https://jina.ai/news and give me a summary."

**🤖 AI Agent:**
> I've read the URL! The main content discusses Jina's latest updates on Search and Reader APIs. Notable news include new model releases. Would you like a more detailed breakdown?

---

**👤 You:**
> "Check the fact: 'The moon is made of green cheese'."

**🤖 AI Agent:**
> I've performed a grounded search. The statement is false; according to scientific consensus, the moon is composed of rock and metal. I can provide the sources if you'd like.


## ❓ FAQ

**Q: How do I find my Jina AI API Key?**
Log in to your [**Jina AI dashboard**](https://jina.ai/api-keys), and you will find your API Key on the main page. Copy and paste it below.

**Q: What is the difference between Jina Search and Reader?**
Jina Search searches across the entire web for results, while Reader extracts the specific main content from a single provided URL, optimized for AI models.

**Q: Can the agent rerank my search results?**
Yes. The `rerank_documents` tool allows your agent to sort a list of documents by relevancy to a query using Jina's advanced reranking models.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/jina-ai](https://vinkius.com/mcp/jina-ai)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Jina AI** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `jina-ai` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Jina AI** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "jina-ai": {
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
