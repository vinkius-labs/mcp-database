# Exa MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/exa)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/exa-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/exa-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [ai-frontier](../categories/ai-frontier.md)

Semantic search engine built for AI — find conceptually relevant web content, not just keyword matches. Powered by neural search technology.

## Description
Connect your AI agent to **Exa** — the semantic search engine built from the ground up for AI applications.

### What you can do

- **Semantic Search** — Search the web using natural language. Unlike Google, Exa understands concepts and meaning, returning results that are semantically relevant even without exact keyword matches
- **Find Similar** — Provide any URL and discover web pages with similar content. Perfect for competitive analysis, research expansion, and content discovery
- **Extract Contents** — Get clean text, highlights, and summaries from any list of URLs. Ideal for building knowledge bases from curated sources

### How it works

1. Subscribe to this server
2. Enter your Exa API key (1,000 free searches/month)
3. Your agent can now search the web with semantic understanding

### Who is this for?

- **AI Agent Developers** — give agents web search that truly understands context and meaning
- **Research Teams** — find related papers, articles, and resources that keyword search would miss
- **Content Teams** — discover competitors, alternatives, and related content at scale


## Available Tools
- **exa_find_similar**: Useful for finding competitors, related articles, or alternative sources on the same subject.

Find web pages semantically similar to a given URL. Perfect for competitive analysis and content discovery
- **exa_get_contents**: Useful when you already know which pages you want to read and need their content in a structured format.

Extract clean text content from specific URLs. Provide comma-separated URLs to retrieve their content
- **exa_search**: Returns page text, highlights, and relevance scores. Supports search types: auto (default), instant (fastest), fast, deep (most thorough).

Search the web using Exa semantic search engine. Finds conceptually relevant results, not just keyword matches


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Exa** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Search for companies building memory infrastructure for AI agents."

**🤖 AI Agent:**
> Found 10 semantically relevant results:

1. **Mem0** (mem0.ai) — Score: 0.94
   Leading memory layer for AI agents with hybrid KV+vector+graph storage...

2. **Zep** (getzep.com) — Score: 0.91
   Long-term conversational memory with temporal knowledge graphs...

3. **Letta** (letta.com) — Score: 0.88
   OS-inspired agent runtime with self-managed memory hierarchy...

---

**👤 You:**
> "Find pages similar to https://docs.langchain.com/docs/get_started/introduction"

**🤖 AI Agent:**
> Found 10 pages similar to LangChain's introduction:

1. **LlamaIndex Documentation** (docs.llamaindex.ai) — Score: 0.92
2. **CrewAI Getting Started** (docs.crewai.com) — Score: 0.89
3. **AutoGen Documentation** (microsoft.github.io/autogen) — Score: 0.86
4. **Haystack Introduction** (docs.haystack.deepset.ai) — Score: 0.83

---

**👤 You:**
> "Extract the content from these 3 URLs: https://arxiv.org/abs/2401.00001, https://openai.com/blog, https://anthropic.com/research"

**🤖 AI Agent:**
> Extracted content from 3 URLs:

### 1. arxiv.org — Research Paper
> Key highlights: Novel approach to multi-agent coordination using graph neural networks...

### 2. openai.com — Blog Post
> Full text extracted: 4,200 words covering latest research developments...

### 3. anthropic.com — Research Page
> Highlights: Constitutional AI methodology and safety-first approach...


## Installation & Usage

To install and use the **Exa** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/exa](https://vinkius.com/mcp/exa)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
