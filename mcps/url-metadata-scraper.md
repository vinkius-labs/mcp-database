# URL Metadata Scraper MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/url-metadata-scraper)
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


## ❓ FAQ

**Q: Does it run a headless browser?**
No, it uses a lightweight fetch to grab the raw HTML, making it incredibly fast.

**Q: What fields does it extract?**
Title, description, featured image URL, and site name.

**Q: Can it bypass captchas?**
No, this is a lightweight HTTP scraper. It will fail on sites protected by Cloudflare or advanced bot protection.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/url-metadata-scraper](https://vinkius.com/mcp/url-metadata-scraper)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **URL Metadata Scraper** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `url-metadata-scraper` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **URL Metadata Scraper** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "url-metadata-scraper": {
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
