# Firecrawl MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/firecrawl)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [friends-mcp](../categories/friends-mcp.md)

Turn any website into clean, LLM-ready Markdown with a single API call — scrape, crawl, search, and map the entire web for your AI agent.

## Description
Connect your AI agent to **Firecrawl** — the most popular web scraping API built specifically for AI and LLM applications.

### What you can do

- **Scrape Pages** — Extract clean Markdown from any URL. Firecrawl handles JavaScript rendering, anti-bot protection, cookie banners, and dynamic content automatically
- **Search the Web** — Search and scrape in one call. Get Google-like search results with full page content already extracted
- **Crawl Websites** — Recursively crawl entire sites, following internal links. Perfect for indexing documentation, blogs, or product catalogs
- **Map Sites** — Discover all URLs on a domain without scraping content. Understand site structure before deciding what to extract

### How it works

1. Subscribe to this server
2. Enter your Firecrawl API key (500 free credits to start)
3. Your agent can now read any webpage on the internet

### Who is this for?

- **AI Agent Developers** — give agents the ability to read and understand any web page
- **Research Teams** — automate web research by extracting structured data from multiple sources
- **Data Engineers** — build pipelines that convert web content into structured data


## Available Tools (4)
- **crawl_site**: Each page is scraped and converted to Markdown. Returns a job ID to track progress.

Crawl an entire website and extract content from multiple pages. Returns a job ID for async tracking
- **map_site**: Useful for understanding site architecture before deciding which pages to scrape.

Discover all URLs on a website without scraping content. Returns a sitemap of discovered links
- **scrape_page**: Handles anti-bot protection, cookie banners, and dynamic content automatically.

Scrape a single web page and extract its content as clean Markdown. Perfect for reading articles, documentation, and product pages
- **search_web**: Ideal for research, fact-checking, and gathering information on any topic.

Search the web and return scraped content from the top results. Combines Google-like search with automatic content extraction


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Firecrawl** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Scrape the main page of docs.firecrawl.dev and give me a summary of what Firecrawl offers."

**🤖 AI Agent:**
> Scraped docs.firecrawl.dev (2,450 words):

Firecrawl offers four core capabilities: Scrape (single page → Markdown), Crawl (recursive site traversal), Map (URL discovery), and Search (web search + scraping). It supports multiple output formats and handles JavaScript rendering, anti-bot protection, and dynamic content automatically.

---

**👤 You:**
> "Search the web for 'best practices for RAG pipelines 2026' and return the top 3 results with content."

**🤖 AI Agent:**
> Found 3 results for 'best practices for RAG pipelines 2026':

1. **Building Production RAG Systems in 2026** (langchain.dev) — 3,200 words
   Full guide covering chunking strategies, embedding models, and retrieval optimization...

2. **RAG Pipeline Architecture** (docs.llamaindex.ai) — 2,800 words
   Comprehensive overview of modern RAG architectures...

3. **Advanced RAG Techniques** (arxiv.org) — 4,100 words
   Research paper on hybrid search, re-ranking, and query transformation...

---

**👤 You:**
> "Map all pages on example.com to see the site structure."

**🤖 AI Agent:**
> Site Map: 47 URLs found on example.com

/
/about
/products
/products/alpha
/products/beta
/blog
/blog/post-1
/blog/post-2
/docs
/docs/getting-started
/docs/api-reference
... and 36 more URLs


## ❓ FAQ

**Q: How does Firecrawl pricing work?**
Firecrawl uses a credit-based system. You get 500 free lifetime credits to start (no credit card required). Base cost is 1 credit per page scraped. Advanced features like JSON extraction (+4 credits) or enhanced mode (+4 credits) consume additional credits per page. Paid plans start at $16/month with 3,000 monthly credits.

**Q: Can Firecrawl handle JavaScript-heavy websites?**
Yes! Firecrawl renders pages in a full browser environment before extracting content — this means it handles React, Next.js, Angular, and any other JavaScript framework. It also automatically bypasses common anti-bot protections, removes cookie consent banners, and waits for dynamic content to load before extraction.

**Q: What formats does Firecrawl return?**
Firecrawl can return content in multiple formats: Markdown (default and most popular for LLM consumption), HTML, raw HTML, structured JSON (with LLM-powered extraction), screenshots, links, and page metadata. You can request multiple formats in a single call.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/firecrawl](https://vinkius.com/mcp/firecrawl)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Firecrawl** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `firecrawl` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Firecrawl** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "firecrawl": {
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
