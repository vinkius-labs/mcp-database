# RSS Feed Parser MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/rss-feed-parser)
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


## ❓ FAQ

**Q: Does it work with podcast feeds?**
Yes. Podcast RSS feeds include enclosure elements with audio/video URLs, MIME types, and file sizes. The parser extracts all of them.

**Q: Can it handle both RSS 2.0 and Atom?**
Yes. Both formats are auto-detected and parsed into the same unified JSON structure. Your agent doesn't need to know which format the source uses.

**Q: Does it fetch the feed URL or do I pass the XML?**
Pass the feed URL and the engine fetches + parses in one step. No manual XML handling needed.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/rss-feed-parser](https://vinkius.com/mcp/rss-feed-parser)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **RSS Feed Parser** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `rss-feed-parser` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **RSS Feed Parser** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "rss-feed-parser": {
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
