# Nimbleway MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/nimbleway)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/nimbleway-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/nimbleway-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [developer-tools](../categories/developer-tools.md)

Web data collection and scraping via Nimbleway — extract content and search the web directly from your AI agent.

## Description
Connect your **Nimbleway** account to your AI agent and leverage high-performance web data collection through natural conversation.

### What you can do

- **Web Extraction** — Fetch and render any web page as raw HTML or clean Markdown using advanced stealth technology to bypass bots.
- **Structured Search** — Execute real-time web searches and receive structured data directly from major search engines.
- **Pipeline Management** — List and inspect your data streams (pipelines) to monitor your scraping workflows.
- **Usage Monitoring** — Track your current bandwidth, remaining credits, and overall account usage in real-time.
- **Job Tracking** — Monitor the progress and metadata of your active data extraction and crawling jobs.
- **Proxy Oversight** — Access configuration details for your residential and data center proxy endpoints.

### How it works

1. Subscribe to this server
2. Enter your Nimbleway API Key
3. Start collecting web data from Claude, Cursor, or any MCP client

### Who is this for?

- **Data Engineers** — quickly test extraction rules or check pipeline statuses without opening the dashboard.
- **Market Researchers** — automate the retrieval of structured web search results for analysis.
- **Developers** — integrate high-fidelity web scraping into your workflows through natural language commands.


## Available Tools
- **extract_html**: Extract web page as HTML
- **extract_markdown**: Extract web page as Markdown
- **get_job**: Get specific job details
- **get_me**: Get current account info
- **get_pipeline**: Get specific pipeline details
- **get_account_usage**: Check account bandwidth and usage
- **list_jobs**: List scraping jobs
- **list_pipelines**: List scraping pipelines
- **list_proxies**: List proxy configuration
- **search_web**: Perform structured web search


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Nimbleway** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Extract the content of 'https://example.com' as Markdown."

**🤖 AI Agent:**
> Initializing extraction... I've successfully fetched the page and converted it to Markdown. The content includes headers, lists, and links from the original site. Shall I summarize it for you?

---

**👤 You:**
> "Search the web for 'latest AI developments 2024' and give me structured results."

**🤖 AI Agent:**
> Executing web search... I've found several top results regarding generative AI, LLM improvements, and new hardware releases. I've retrieved the snippets, titles, and URLs for each. Would you like to extract the full content of the top result?

---

**👤 You:**
> "Check my account usage and remaining credits."

**🤖 AI Agent:**
> Retrieving usage data... You have used 15GB of bandwidth this month out of your 50GB limit. You also have 4,500 successful extraction credits remaining. Your account status is 'ACTIVE'.


## Installation & Usage

To install and use the **Nimbleway** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/nimbleway](https://vinkius.com/mcp/nimbleway)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
