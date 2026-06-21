# Web Scraper MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/web-scraper)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [developer-tools](../categories/developer-tools.md)

Equip your AI agent with the ability to read web pages, extract metadata, and crawl documentation sites as clean Markdown.

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


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Web Scraper** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Read https://en.wikipedia.org/wiki/Artificial_intelligence and summarize its history."

**🤖 AI Agent:**
> I've fetched the Wikipedia page. The history of AI spans back to antiquity with myths of artificial beings, but the formal field was founded in 1956 at Dartmouth College. It experienced cycles of immense optimism followed by disappointment ('AI winters'), eventually leading to the modern deep learning revolution fueled by huge datasets and compute power.

---

**👤 You:**
> "Extract the links from https://news.ycombinator.com/"

**🤖 AI Agent:**
> I've extracted the outbound links. The site currently links out to 30 primary article sources including domains like github.com, weired.com, and nytimes.com, along with many internal navigational links to user profiles and comment threads.

---

**👤 You:**
> "Compare these two links: url1.com and url2.com"

**🤖 AI Agent:**
> Using the batch reading tool, I've loaded both URLs simultaneously. URL 1 discusses a 'React-first' architecture and uses component styling. URL 2 advocates for 'HTML-first', server-rendered patterns. While both aim to increase web performance, they take fundamentally opposite approaches to client-side hydration.


## ❓ FAQ

**Q: Can it read documentation sites that are split into multiple pages?**
Yes! You can use the `crawl` tool. For example: 'Crawl the getting started guide at https://example.com/docs'. The agent will fetch the starting page and automatically follow inner links to gather up to 10 pages of context.

**Q: How does it handle ads and cluttered websites?**
The `read` tool uses the same underlying technology as Firefox's 'Reader View' (@mozilla/readability). It intelligently strips out standard website boilerplate—like navbars, sidebars, footers, and ads—leaving only the title and the clean main article text converted to Markdown.

**Q: Is there a limit on how many URLs I can batch process?**
Yes, to ensure conversational AI latency remains reasonable, the `batch_read` tool accepts a maximum of 10 URLs in a single request. All 10 URLs are fetched simultaneously in parallel for maximum speed.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/web-scraper](https://vinkius.com/mcp/web-scraper)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Web Scraper** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `web-scraper` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Web Scraper** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "web-scraper": {
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
