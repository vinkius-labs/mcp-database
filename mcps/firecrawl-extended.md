# Firecrawl MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/firecrawl-extended)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [friends-mcp](../categories/friends-mcp.md)

Crawl and scrape entire websites into clean LLM-ready markdown with a single API call that handles JavaScript rendering.

## Description
Connect your **Firecrawl** account to any AI agent and take full control of your web data acquisition and recursive crawling workflows through natural conversation.

### What you can do

- **Web Scrape Orchestration** — Scrape any single URL programmatically into high-fidelity Markdown, excluding boilerplate content like headers and footers automatically
- **Recursive Crawling** — Programmatically discover and scrape all subpages starting from a root URL to build comprehensive knowledge bases and RAG pipelines
- **Site Mapping** — Quickly identify all reachable links on a domain without full content extraction to understand website structures and hierarchies
- **Visual Capture** — Capture full-page screenshots of any URL directly through your agent to maintain a visual record of web data
- **Usage Monitoring** — Track your Firecrawl credit usage, remaining limits, and active crawl job statuses in real-time

### How it works

1. Subscribe to this server
2. Retrieve your **API Key** from the Firecrawl dashboard (API Keys section)
3. Start scraping and crawling the web from Claude, Cursor, or any MCP client

No more manual copy-pasting from websites or complex BeautifulSoup scripts. Your AI acts as your dedicated web data engineer.

### Who is this for?

- **AI Developers** — build RAG applications by programmatically ingesting clean, structured web data via natural language
- **Research Teams** — automate data gathering from across the web for market analysis and competitor monitoring
- **Content Creators** — instantly convert articles into Markdown and capture website screenshots without leaving your workspace


## Available Tools (6)
- **get_api_usage**: Check Firecrawl credit usage
- **cancel_active_crawl**: Stop an ongoing crawl
- **get_crawl_status**: Check the status of a crawl job
- **start_crawl**: Returns a job ID.

Recursively crawl a website
- **map_website_structure**: Discover all URLs on a site
- **scrape_url**: Turn a single URL into clean Markdown


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Firecrawl** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Turn 'https://stripe.com/docs/api' into clean Markdown."

**🤖 AI Agent:**
> Scraping in progress... I've successfully converted the Stripe API documentation into high-fidelity Markdown, excluding the navigation and footers. Would you like me to summarize the main endpoints for you?

---

**👤 You:**
> "Crawl 'https://docs.firecrawl.dev' recursively with a limit of 10 pages."

**🤖 AI Agent:**
> Crawl job started! I've initiated a recursive crawl of the Firecrawl documentation (ID: crl_123). I'll monitor the progress for you and notify you as soon as the 10 pages are indexed.

---

**👤 You:**
> "Map all internal links for 'https://github.com/vinkius'."

**🤖 AI Agent:**
> Mapping site structure... I've identified all reachable links for the requested domain. I found 25 internal URLs, including various repository and profile paths. Would you like the full list of mapped URLs?


## ❓ FAQ

**Q: How do I find my Firecrawl API Key?**
Log in to your [**Firecrawl dashboard**](https://www.firecrawl.dev/app/dashboard), and navigate to the **API Keys** section to copy your unique token.

**Q: Can I scrape content excluding headers and footers?**
Yes! The `scrape_url` tool includes an `onlyMainContent` parameter. When set to true, Firecrawl uses AI to extract only the core article or page content.

**Q: How long does a recursive crawl take?**
Crawl time depends on the site size and depth. Use the `get_crawl_status` tool to monitor progress and retrieve results once the job is complete.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/firecrawl-extended](https://vinkius.com/mcp/firecrawl-extended)
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
3. Set Type to "SSE" (or "streamable HTTP"), enter `firecrawl-extended` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Firecrawl** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "firecrawl-extended": {
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
