# Bing Search MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/bing-search-1)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [industry-titans](../categories/industry-titans.md)

Power your AI agent with global web data via Bing Search — query web pages, images, news, videos, and local businesses in real-time.

## Description
Connect your Microsoft **Bing Search** API key to any AI agent and empower it with real-time web intelligence and graph data.

### What you can do

- **Web & Local Search** — Query the entire web or prioritize local business listings and geographical places.
- **Media Extraction** — Search specifically for images and videos with native physical metadata tracking.
- **News Tracking** — Pull real-time syndicated global news and discover macro trending topics instantly.
- **Entities & NLP** — Resolve famous persons, places, and objects using the Knowledge Graph, and run semantic NLP spellchecks.
- **Custom Search** — Lock queries to specific whitelisted domains explicitly using custom configurations.

### How it works

1. Subscribe to this server
2. Enter your Bing Search API Key from Azure
3. Start exploring the web through Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Researchers** — pull deep knowledge graph entities and recent news articles instantly.
- **Marketers** — track trending viral news topics and natively search custom whitelisted PR domains.
- **Content Creators** — rapidly search for image media and video links without leaving your AI environment.


## Available Tools
- **search_local**: Force explicit Local Business listing extraction over standard web nodes
- **search_news**: 0/news/search` resolving syndicated global PR articles grouped by timestamp clusters.

Query explicitly syndicated News articles across global PR sources
- **custom_search**: 0/custom/search` restricting queries strictly into pre-built whitelist domains.

Perform search locked explicitly to a predefined Configuration ID
- **search_entities**: 0/entities` bounding rich structured data resolving Famous Persons, Places, or Objects.

Retrieve deeply structured Entity graphs (Knowledge Graph mappings)
- **search_images**: 0/images/search` filtering explicit image thumbnails parsing pixel dimensions natively.

Search for explicit Image results matching a keyword string
- **spellcheck**: 0/spellcheck` correcting string tokens natively via semantic NLP boundaries.

Execute explicit semantic NLP spell checking on short strings
- **autosuggest**: 0/Suggestions` matching high-velocity partial queries directly against ML autosuggest logs.

Fetch automated real-time query completion suggestions
- **trending_news**: 0/news/trendingtopics` surfing fully decoupled virality indexes completely ignoring keywords.

Discover explicit macroscopic viral Trending News topics
- **search_videos**: 0/videos/search` tracking streaming bounds capturing native motion array metadata.

Retrieve explicitly indexed Video stream links and metadata
- **search_web**: 0/search` scraping up to 50 organic results mapped directly from the Microsoft Graph.

Perform an explicit Web search using the Microsoft Bing Graph


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Bing Search** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Search the web for the latest advancements in solid-state batteries."

**🤖 AI Agent:**
> I found the top organic results from the Microsoft Graph. Recent breakthroughs from early 2026 show improvements in energy density... [Top 5 source URLs].

---

**👤 You:**
> "Show me the trending global news right now."

**🤖 AI Agent:**
> Currently, the major trending topics are: 1. Launch of the new orbital telescope, 2. Global market indexes surge, 3. The latest international sports finals updates.

---

**👤 You:**
> "Find images of modern minimalist architecture."

**🤖 AI Agent:**
> I extracted several image thumbnails with native pixel dimensions directly from Bing Images. Here they are... (Provides 10 high-resolution thumbnail URLs).


## ❓ FAQ

**Q: Can my agent search for recent news on a specific topic?**
Yes. By using the 'search_news' tool, your AI agent can gather syndicated global PR articles grouped by timestamp, allowing you to instantly stay updated on competitive intelligence without opening multiple tabs.

**Q: Does the agent understand specific entities like famous people or places?**
Absolutely. The 'search_entities' tool taps directly into Microsoft's Knowledge Graph, returning deeply structured contextual data about notable people, places, or objects beyond normal organic links.

**Q: Can I restrict AI searches to only my company's domain?**
Yes. If you have a predefined Custom Configuration ID, the 'custom_search' tool strictly locks queries to your pre-built whitelisted domains, ensuring clean and verified business results.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/bing-search-1](https://vinkius.com/mcp/bing-search-1)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Bing Search** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `bing-search-1` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Bing Search** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "bing-search-1": {
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
