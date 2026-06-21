# Web Scraper MCP Server

Equip your AI agent with the ability to read web pages, extract metadata, and crawl documentation sites as clean Markdown.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/web-scraper)

## Overview
**Category:** developer-tools
**Tools Count:** 5

## Description
Connect the **Web Scraper** utility to any AI agent to give it direct access to the public internet. Instead of letting the AI hallucinate facts, allow it to read real-time articles, parse documentation, and fetch clean text from any URL you provide.

### What you can do

- **Reader View** — Convert any cluttered webpage into pristine, readable Markdown by stripping out ads, navbars, and boilerplate using Mozilla Readability logic
- **Site Crawling** — Instruct the AI to crawl a starting URL (like a documentation hub or wiki) up to 10 pages deep automatically
- **Batch Processing** — Fetch up to 10 different URLs in parallel to compare articles or summarize multiple sources at once
- **Metadata Extraction** — Quickly pull SEO titles, descriptions, OG tags, canonical links, and all outbound hyperlinks without downloading the entire page body

### How it works

1. Subscribe to this server
2. No API keys or authentication required
3. Simply paste a link in your chat and tell your agent to 'read this URL' or 'crawl this documentation'

### Who is this for?

- **Developers** — point the agent to a new library's API docs and have it write code using the absolute latest syntax
- **Researchers** — drop a handful of Wikipedia links and ask the AI to synthesize a comprehensive summary from the fetched data
- **SEO Specialists** — audit a webpage's metadata, extracted titles, and outbound link structure dynamically


## Available Tools
- **read**: Uses @mozilla/readability (Firefox Reader View) to extract the main article content, then converts to Markdown. Works best for articles, docs, blogs, and Wikipedia.

Fetch any public web page and return its full content as clean Markdown
- **extract**: Returns: title, description, OG tags, lang, author, robots, canonical, link count. For the full page content, use the read tool instead.

Extract structured metadata from a web page: title, description, OG tags, and more
- **list_links**: Internal links share the same hostname as the source page.

Extract all hyperlinks from a web page
- **batch_read**: All URLs are fetched in parallel. Maximum 10 URLs per batch.

Fetch multiple web pages in parallel
- **crawl**: Maximum 10 pages to keep response size manageable.

Crawl a website starting from a URL


## Installation & Usage

To install and use the **Web Scraper** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/web-scraper](https://vinkius.com/mcp/web-scraper)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
