# Spider MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/spider)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [ship-it](../categories/ship-it.md)

High-performance Rust-powered web scraping and crawling — scrape, crawl, and search up to 100K+ pages/second with built-in anti-bot protection.

## Description
Connect your AI agent to **Spider.cloud** — the fastest web scraping API in the market, built in Rust for maximum performance.

### What you can do

- **Scrape Pages** — Extract content from any URL as Markdown, HTML, or plain text. Spider handles JavaScript rendering, anti-bot protection, and proxy rotation
- **Crawl Sites** — Recursively crawl entire websites at speeds exceeding 100K pages/second. Follow internal links and extract structured data at scale
- **Search & Scrape** — Search the web and scrape results in a single API call. Combines discovery with extraction for maximum efficiency

### How it works

1. Subscribe to this server
2. Enter your Spider API key (500 free credits to start)
3. Your agent can now crawl the web at blazing speed

### Why Spider over alternatives?

- **10-20x faster** than Firecrawl for large crawls (Rust engine vs Node.js)
- **Lower cost** per page at high volume
- **Built-in stealth** mode with fingerprint rotation and residential proxies


## Available Tools
- **spider_crawl**: Spider.cloud Rust engine follows internal links and scrapes each page. Configure depth and page limits to control scope.

Crawl an entire website at blazing speed — up to 100K+ pages/second. Returns content from multiple pages following internal links
- **spider_scrape**: cloud Rust-powered engine to scrape a single URL. Handles JavaScript rendering, anti-bot protection, and proxy rotation automatically. Supports multiple output formats: markdown (default), html, text.

Scrape a single web page at high speed using Spider.cloud. Returns clean content in Markdown, HTML, or plain text format
- **spider_search**: Combines search + scrape in one API call for maximum efficiency.

Search the web and scrape results in a single high-performance request via Spider.cloud


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Spider** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Scrape the homepage of spider.cloud and show me what they offer."

**🤖 AI Agent:**
> Scraped spider.cloud (1,200 words):

Spider.cloud is the fastest web crawler, built in Rust. Core features: Scrape, Crawl, Search, AI-powered extraction, and Browser Cloud for full CDP access. Supports markdown, HTML, JSON output formats with built-in anti-bot protection and proxy rotation.

---

**👤 You:**
> "Crawl docs.python.org and get the first 5 pages."

**🤖 AI Agent:**
> Crawled 5 pages from docs.python.org:

1. **Python Documentation** (/) — 3,200 words
2. **Tutorial** (/tutorial) — 4,100 words
3. **Library Reference** (/library) — 2,800 words
4. **FAQ** (/faq) — 1,900 words
5. **What's New** (/whatsnew) — 5,400 words

---

**👤 You:**
> "Search for 'machine learning frameworks comparison 2026' and scrape the top 3 results."

**🤖 AI Agent:**
> Found and scraped 3 results:

1. **ML Framework Comparison 2026** (towardsdatascience.com) — 4,500 words
2. **PyTorch vs TensorFlow vs JAX** (paperswithcode.com) — 3,200 words
3. **Best ML Frameworks Review** (neptune.ai) — 2,900 words


## ❓ FAQ

**Q: How is Spider different from Firecrawl?**
Spider is built in Rust and optimized for raw speed and volume — it can crawl 100K+ pages per second, making it 10-20x faster than Firecrawl for large-scale operations. Spider also offers lower per-page costs at high volume, built-in stealth mode with fingerprint rotation, and multiple request modes (HTTP, Smart, Chrome). Firecrawl excels at simplicity and LLM-specific features like JSON extraction.

**Q: What output formats does Spider support?**
Spider supports Markdown, HTML, raw HTML, plain text, JSON (structured extraction), screenshots, and PDF output. You can specify the desired format via the return_format parameter in each request.

**Q: How does Spider pricing work?**
Spider offers 500 free credits to get started (no credit card required). Paid plans are usage-based with credits consumed per page scraped. The Starter plan begins at $15/month with 12,000 credits. Enterprise plans offer custom pricing with dedicated infrastructure and unlimited concurrency.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/spider](https://vinkius.com/mcp/spider)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Spider** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `spider` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Spider** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "spider": {
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
