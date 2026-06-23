# Spaceflight News MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/spaceflight-news)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [scientific-research](../categories/scientific-research.md)

Access real-time spaceflight news, blogs, and technical reports from major space agencies and news outlets worldwide.

## Description
Connect your AI agent to the **Spaceflight News API (SNAPI)** to stay updated with the latest developments in space exploration, satellite launches, and astronomical discoveries.

### What you can do

- **Latest Articles** — List and search through thousands of news articles from verified space news providers.
- **Blog Feed** — Access specialized blog posts and opinion pieces from the spaceflight community.
- **Technical Reports** — Retrieve official reports and technical documents, including ISS daily status updates.
- **Deep Search** — Filter content by news site, search terms, or specific IDs to find exactly what you need.
- **API Metadata** — Check the current status of the API and see which news sources are being tracked in real-time.

### How it works

1. Subscribe to this server
2. Configure your API access (if required for higher rate limits)
3. Start querying space data from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Space Enthusiasts** — get the latest updates on SpaceX, NASA, and ESA missions without browsing multiple sites.
- **Researchers & Journalists** — quickly find historical reports or specific articles for data-driven storytelling.
- **Developers** — integrate real-time space news feeds into your own applications or dashboards via your AI assistant.


## Available Tools (7)
- **get_article**: Get a specific spaceflight news article
- **list_articles**: List spaceflight news articles
- **list_blogs**: List spaceflight blogs
- **get_blog**: Get a specific spaceflight blog post
- **get_report**: Get a specific spaceflight report
- **get_info**: Get Spaceflight News API info
- **list_reports**: g., ISS Daily Reports).

List spaceflight reports


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Spaceflight News** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Show me the 5 most recent spaceflight articles about the James Webb telescope."

**🤖 AI Agent:**
> I've found 5 recent articles using `list_articles`. They cover the latest deep-space images and calibration updates from the James Webb Space Telescope. Would you like the full details for any of them?

---

**👤 You:**
> "Get the latest technical reports from the ISS."

**🤖 AI Agent:**
> Fetching reports via `list_reports`... I've retrieved the latest International Space Station daily status reports. They include details on crew activities and station maintenance.

---

**👤 You:**
> "Search for blog posts from 'SpaceX' about Starship."

**🤖 AI Agent:**
> Searching blogs... Using `list_blogs` with the term 'Starship' and filtering for 'SpaceX', I found several updates regarding recent flight tests and orbital attempts.


## ❓ FAQ

**Q: How can I find news articles specifically about Mars or SpaceX?**
You can use the `list_articles` tool and provide a keyword in the `search` parameter. For example, searching for 'Mars' will return all articles containing that term in the title or summary.

**Q: Can I filter news by a specific source like NASA or SpaceNews?**
Yes! Use the `list_articles` or `list_blogs` tools with the `news_site` parameter to filter results from a specific provider.

**Q: How do I see which news sites are currently supported by the API?**
Simply run the `get_info` tool. It returns metadata about the API, including a list of all news sites currently being tracked.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/spaceflight-news](https://vinkius.com/mcp/spaceflight-news)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Spaceflight News** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `spaceflight-news` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Spaceflight News** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "spaceflight-news": {
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
