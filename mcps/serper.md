# Serper MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/serper)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/serper-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/serper-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [developer-tools](../categories/developer-tools.md)

Fast, affordable Google Search API — get real-time SERP results, news, and images with 2,500 free searches per month.

## Description
Connect your AI agent to **Serper.dev** — the fastest and most cost-effective way to get Google Search results programmatically.

### What you can do

- **Google Search** — Get organic search results with titles, links, snippets, and positions. Supports geolocation and language parameters for localized results
- **Google News** — Search the latest news articles with headlines, sources, publication dates, and snippets
- **Google Images** — Find image results with URLs, titles, and source pages for visual research

### How it works

1. Subscribe to this server
2. Enter your Serper API key (2,500 free searches/month)
3. Your agent can now search Google in real-time

### Why Serper?

- **2,500 free searches/month** — the most generous free tier for Google SERP APIs
- **Sub-100ms latency** — fastest Google SERP API available
- **Native LangChain/CrewAI integration** — the default search tool for most AI frameworks


## Available Tools
- **google_image_search**: dev to query Google Images and return structured results including image URLs, titles, and source pages. Useful for visual research, content creation, and reference gathering.

Search Google Images for visual content related to any query. Returns image URLs, titles, and sources
- **google_news_search**: dev to query Google News and return the most recent news articles matching your query. Perfect for monitoring breaking news, industry trends, and competitor announcements.

Search Google News for the latest articles on any topic. Returns headlines, sources, dates, and snippets
- **google_search**: dev to perform a real-time Google Search and return structured organic results. Supports geolocation (gl) and language (hl) parameters for localized results. Returns up to 100 results per query.

Search Google and get organic SERP results instantly. Returns titles, links, snippets, and positions for any query


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Serper** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Search Google for 'best AI agent frameworks 2026' and show me the top 5 results."

**🤖 AI Agent:**
> Found 5 results for 'best AI agent frameworks 2026':

| # | Title | Source |
|---|---|---|
| 1 | Top 10 AI Agent Frameworks | datacamp.com |
| 2 | LangGraph vs CrewAI vs AutoGen | towardsdatascience.com |
| 3 | Best Agent Tools 2026 | dev.to |
| 4 | Building AI Agents Guide | langchain.com |
| 5 | Agent Framework Comparison | medium.com |

---

**👤 You:**
> "Search the latest news about OpenAI."

**🤖 AI Agent:**
> Found 10 news articles about OpenAI:

| # | Title | Source | Date |
|---|---|---|---|
| 1 | OpenAI Launches New Agent API | techcrunch.com | 2h ago |
| 2 | GPT-5 Release Timeline | theverge.com | 5h ago |
| 3 | OpenAI Valued at $300B | bloomberg.com | 1d ago |

---

**👤 You:**
> "Search Google Images for 'neural network architecture diagram'."

**🤖 AI Agent:**
> Found 10 image results for 'neural network architecture diagram':

1. **CNN Architecture Diagram** — researchgate.net
2. **Transformer Model Architecture** — arxiv.org
3. **Deep Learning Layers Visualization** — towardsdatascience.com


## Installation & Usage

To install and use the **Serper** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/serper](https://vinkius.com/mcp/serper)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
