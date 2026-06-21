# RSS Feed Parser MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/rss-feed-parser)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/rss-feed-parser-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/rss-feed-parser-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Turn any RSS 2.0 or Atom feed into clean, structured JSON. Extract titles, links, dates, authors, and full content from blogs, news sites, and podcasts — ready for your agent to process.

## Description
Your content marketing agent needs to monitor 20 competitor blogs, 5 industry news feeds, and 3 podcast channels. Without a parser, it scrapes HTML — inconsistent, slow, and full of noise.

RSS and Atom feeds are the web's native content API. This MCP parses them into clean JSON objects with titles, links, publication dates, authors, categories, and full content — ready for summarization, curation, or automated distribution.

### The Superpowers

- **RSS 2.0 + Atom:** Both formats parsed identically into a unified JSON structure.
- **Full Content:** Extracts title, link, date, author, categories, enclosures (podcasts), and content/summary.
- **No Scraping:** Clean, structured data from the feed XML — no HTML parsing, no DOM traversal.
- **Podcast Ready:** Enclosure extraction for audio/video URLs, durations, and file sizes.


## Available Tools
- **parse_rss_feed**: Pass the raw XML string and receive a structured JSON with feed metadata and up to 20 items. This is essential for content marketing agents monitoring blogs, news aggregators, and podcast feeds. Never try to parse XML manually — use this engine for deterministic extraction.

Parses RSS 2.0 and Atom feed XML into structured JSON objects. Extracts title, description, items with links, dates, categories, and content snippets


## 💬 Prompt Examples

Here are some examples of how you can interact with the **RSS Feed Parser** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Monitor TechCrunch's RSS feed and give me the latest 5 articles with titles and publish dates."

**🤖 AI Agent:**
> 5 articles extracted: title, link, pubDate, author, and content snippet for each.

---

**👤 You:**
> "Parse our company blog feed and extract all articles tagged 'product-update' from the last 30 days."

**🤖 AI Agent:**
> 8 articles found with 'product-update' category in the last 30 days.

---

**👤 You:**
> "Get the latest episode URLs from this podcast RSS feed for our newsletter."

**🤖 AI Agent:**
> 3 episodes with audio URLs, durations, and descriptions extracted.


## Installation & Usage

To install and use the **RSS Feed Parser** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/rss-feed-parser](https://vinkius.com/mcp/rss-feed-parser)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
