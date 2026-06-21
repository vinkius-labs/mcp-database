# URL Metadata Scraper MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/url-metadata-scraper)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/url-metadata-scraper-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/url-metadata-scraper-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [developer-tools](../categories/developer-tools.md)

Stop wasting tokens scraping entire websites. Instantly extract clean OpenGraph metadata (title, description, image) from any URL.

## Description
When an AI Agent needs to summarize a link for a social media post, loading the entire HTML into the context window is slow, expensive, and leads to hallucinations. This MCP solves that by natively fetching only the OpenGraph and SEO tags.

### The Superpowers

- **Token Optimization:** Uses Cheerio to parse HTML instantly in the Edge runtime, returning only the 4 fields you care about.
- **Social Ready:** Perfect for agents building marketing dashboards or Twitter threads.


## Available Tools
- **scrape_url**: Pass the full URL and receive structured metadata without loading a headless browser. Useful for link previews, SEO audits, and social sharing validation.

Extracts OpenGraph and SEO metadata (Title, Description, Image) from a URL instantly without loading a full headless browser


## 💬 Prompt Examples

Here are some examples of how you can interact with the **URL Metadata Scraper** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Extract the OpenGraph metadata from `https://vinkius.com`."

**🤖 AI Agent:**
> Metadata: {"title": "Vinkius", "description": "The Agentic Platform", "image": "url.jpg"}

---

**👤 You:**
> "Get the main image for this news article so I can post it on Twitter."

**🤖 AI Agent:**
> Extracted: `https://news.com/cover.jpg`.

---

**👤 You:**
> "Check the SEO description for this landing page URL."

**🤖 AI Agent:**
> SEO Description: The best platform for AI automation.


## Installation & Usage

To install and use the **URL Metadata Scraper** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/url-metadata-scraper](https://vinkius.com/mcp/url-metadata-scraper)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
