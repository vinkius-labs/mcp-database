# HTML DOM Query Engine MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/html-dom-query-engine)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/html-dom-query-engine-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/html-dom-query-engine-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [loved-by-devs](../categories/loved-by-devs.md)

Extract specific text and attributes from massive HTML payloads instantly using CSS selectors. Fast, memory-efficient DOM parsing.

## Description
If an AI agent needs to scrape a product price from a 20,000-line e-commerce HTML page, passing the entire raw HTML to the LLM destroys its token limit and leads to hallucination. This MCP allows the LLM to pass the raw string and a CSS selector, instantly returning just the target data.

### The Superpowers

- **Token Saver:** Offloads heavy DOM parsing to the native V8 runtime via Cheerio.
- **Precision Scraping:** Supports complex CSS selectors (e.g. `#main .price`) and extracts specific attributes like `href` or `src`.


## Available Tools
- **query_dom**: Pass the HTML string and a CSS query (e.g. "h1", ".price", "#title"). Returns the matched text content or attributes.

Parses a raw HTML string and extracts text or attributes using a CSS selector deterministically


## 💬 Prompt Examples

Here are some examples of how you can interact with the **HTML DOM Query Engine** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Extract the text from `.product-price` from this 5,000 line HTML file."

**🤖 AI Agent:**
> ✅ **Matches Found:**
1. `$149.99`

---

**👤 You:**
> "Extract all image source URLs (`src`) from the `.gallery img` selector."

**🤖 AI Agent:**
> ✅ **Matches:** Extracted 12 `src` attributes successfully.

---

**👤 You:**
> "Get the text inside the `<h1>` tag."

**🤖 AI Agent:**
> ✅ **Matched Text:** 'Welcome to our API documentation.'


## Installation & Usage

To install and use the **HTML DOM Query Engine** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/html-dom-query-engine](https://vinkius.com/mcp/html-dom-query-engine)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
