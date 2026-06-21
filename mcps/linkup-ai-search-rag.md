# Linkup (AI Search & RAG) MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/linkup-ai-search-rag)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/linkup-ai-search-rag-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/linkup-ai-search-rag-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [ai-frontier](../categories/ai-frontier.md)

Power your AI agents with real-time web search via Linkup — execute semantic queries and extract RAG-ready content.

## Description
Connect your **Linkup** account to any AI agent and take full control of real-time web intelligence and content retrieval for RAG pipelines through natural conversation.

### What you can do

- **Semantic Web Search** — Execute context-rich queries that return high-relevancy results specifically optimized for Large Language Models directly from your agent
- **Deep Content Retrieval** — Extract clean, readable text from any web URL, stripping away noise and navigation to feed high-quality grounding data to your AI
- **RAG-Ready Payloads** — Retrieve structured search results including titles, snippets, and source URLs designed for seamless integration into vector stores
- **Precision Extraction** — Target specific URLs for content parsing, ensuring your agent has the exact technical context or documentation required for its task
- **Real-time Intelligence** — Access the latest facts and data from across the internet to ground your agent's answers in up-to-date reality
- **Search Breadth** — Switch between standard and deep search modes to balance between rapid fact-finding and comprehensive research across the web

### How it works

1. Subscribe to this server
2. Enter your Linkup API Key
3. Start grounding your AI with live web data from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **RAG Developers** — provide your agents with real-time web access and precise document retrieval for contextual grounding through natural conversation
- **AI & ML Engineers** — automate the extraction of high-quality web content for model fine-tuning and evaluation datasets
- **Market Researchers** — perform large-scale data collection and fact-finding across the web without manual scraping scripts


## Available Tools
- **search_web**: Choose "fast" mapping for basic factual requests and "deep" for thorough research limits.

Perform a real-time web search extracting deep answers utilizing Linkup Platform
- **fetch_url**: Bypasses advanced bot protections executing complex SPA JavaScript loops automatically.

Fetch and extract clean content from any specific URL using Linkup Platform


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Linkup (AI Search & RAG)** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Search for the latest NVIDIA earnings report summary"

**🤖 AI Agent:**
> Searching the web… Based on the latest results from Linkup, NVIDIA reported Q4 revenue of $22.1 billion, up 265% year-over-year. Data center revenue hit a record $18.4 billion. Would you like me to fetch the full detailed analysis from one of the source articles?

---

**👤 You:**
> "Extract the technical specifications from this documentation URL: [url]"

**🤖 AI Agent:**
> Fetching content… I've extracted the clean technical text. The system requirements include 16GB RAM, an NVIDIA RTX 30-series GPU, and Python 3.10+. I can provide the full list of API endpoints described in the doc as well.

---

**👤 You:**
> "Deep search for 'AI agent security best practices 2024'"

**🤖 AI Agent:**
> Performing deep search… I've synthesized security insights from 12 diverse sources. Key best practices for 2024 include: 1) Strict tool-call sandboxing, 2) Human-in-the-loop for high-stakes actions, 3) Real-time prompt injection monitoring. Would you like a detailed breakdown of the sandboxing techniques?


## Installation & Usage

To install and use the **Linkup (AI Search & RAG)** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/linkup-ai-search-rag](https://vinkius.com/mcp/linkup-ai-search-rag)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
