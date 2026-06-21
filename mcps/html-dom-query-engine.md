# HTML DOM Query Engine MCP Server

Extract specific text and attributes from massive HTML payloads instantly using CSS selectors. Fast, memory-efficient DOM parsing.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/html-dom-query-engine)

## Overview
**Category:** loved-by-devs
**Tools Count:** 1

## Description
If an AI agent needs to scrape a product price from a 20,000-line e-commerce HTML page, passing the entire raw HTML to the LLM destroys its token limit and leads to hallucination. This MCP allows the LLM to pass the raw string and a CSS selector, instantly returning just the target data.

### The Superpowers

- **Token Saver:** Offloads heavy DOM parsing to the native V8 runtime via Cheerio.
- **Precision Scraping:** Supports complex CSS selectors (e.g. `#main .price`) and extracts specific attributes like `href` or `src`.


## Available Tools
- **query_dom**: Pass the HTML string and a CSS query (e.g. "h1", ".price", "#title"). Returns the matched text content or attributes.

Parses a raw HTML string and extracts text or attributes using a CSS selector deterministically


## Installation & Usage

To install and use the **HTML DOM Query Engine** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/html-dom-query-engine](https://vinkius.com/mcp/html-dom-query-engine)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
