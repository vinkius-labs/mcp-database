# SerpApi MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/serpapi-extended)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/serpapi-extended-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/serpapi-extended-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [data-analytics](../categories/data-analytics.md)

Access real-time search engine results from Google, Bing, and more via SerpApi — perform structured searches, find locations, and monitor account usage.

## Description
Connect **SerpApi** to your AI agent to scrape and analyze search engine results pages (SERPs) with ease. Get structured data from Google, Bing, Baidu, and other major search engines directly within your conversation.

### What you can do

- **Global Search** — Execute queries across multiple search engines with support for specific locations, languages, and devices.
- **Location Discovery** — Find and validate supported geographic locations to ensure localized search accuracy.
- **Account Monitoring** — Keep track of your API usage, plan limits, and account status in real-time.
- **Structured Results** — Receive clean, parsed data instead of messy HTML, perfect for data analysis and SEO tracking.

### How it works

1. Subscribe to this server
2. Enter your SerpApi API Key
3. Start querying search engines from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **SEO Specialists** — track rankings and analyze SERP features without manual searching
- **Data Scientists** — gather real-world data from the web for analysis and training
- **Market Researchers** — monitor competitor visibility and global search trends


## Available Tools
- **get_account**: Retrieve SerpApi account information
- **get_locations**: Find supported locations for SerpApi searches
- **search**: ) and returns structured results.

Perform a search using SerpApi


## 💬 Prompt Examples

Here are some examples of how you can interact with the **SerpApi** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Search for 'latest breakthroughs in quantum computing' on Google."

**🤖 AI Agent:**
> I've performed the search. The top results include articles from Nature and MIT Technology Review discussing new error-correction methods and 1000-qubit processors. Would you like a summary of the top 3 results?

---

**👤 You:**
> "Check my SerpApi account usage and plan details."

**🤖 AI Agent:**
> You are currently on the 'Developer' plan. You have used 450 out of 2,500 searches this month, leaving you with 2,050 searches remaining.

---

**👤 You:**
> "Find supported search locations for 'San Francisco'."

**🤖 AI Agent:**
> I found several matches: 'San Francisco, California, United States', 'San Francisco, Cordoba, Argentina', and 'San Francisco, Heredia, Costa Rica'. Which one would you like to use for your search?


## Installation & Usage

To install and use the **SerpApi** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/serpapi-extended](https://vinkius.com/mcp/serpapi-extended)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
