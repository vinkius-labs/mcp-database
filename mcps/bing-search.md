# Bing Search MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/bing-search)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [industry-titans](../categories/industry-titans.md)

Empower your AI agent with real-time web, image, and news search via Bing.

## Description
Connect your **Bing Search API** account to any AI agent and integrate comprehensive search capabilities into your workflows through natural conversation.

### What you can do

- **Web Search** — Retrieve top results, snippets, and deep links from across the entire web.
- **Image Discovery** — Search for relevant images and retrieve metadata including dimensions and source URLs.
- **News Monitoring** — Stay up to date with the latest news articles and trending social topics.
- **Local Search** — Find businesses, services, and places relevant to your queries.
- **Trending Insights** — Retrieve currently trending images and topics to monitor viral content.
- **Autocomplete Suggestions** — Get real-time search suggestions to refine your AI's queries.

### How it works

1. Subscribe to this server
2. Enter your Bing Search API Key (from Azure Portal)
3. Start searching the world from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Researchers & Analysts** — quickly gather information and sources from the web without leaving their editor.
- **Content Creators** — find trending topics and relevant images for their work using natural language.
- **Developers** — integrate real-time web data into their automated agent workflows.


## Available Tools
- **get_trending_images**: Retrieve currently trending images
- **get_trending_news**: Retrieve currently trending news topics
- **search_images**: Search for images using Bing
- **search_videos**: Search for videos using Bing
- **search_local**: Search for local businesses or places
- **search_news**: Search for news articles using Bing
- **search_suggestions**: Get search autocomplete suggestions
- **search_web**: Search the web using Bing


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Bing Search** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Search the web for the latest developments in quantum computing."

**🤖 AI Agent:**
> I've found the latest articles. Key topics include advances in error correction and new partnerships between major tech firms. Would you like a summary of the top 3 results?

---

**👤 You:**
> "Find images of high-tech office spaces."

**🤖 AI Agent:**
> Retrieving images... I found several relevant photos showcasing modern, ergonomic, and tech-focused office designs. Which ones would you like to see details for?

---

**👤 You:**
> "Show me the top trending news in Technology."

**🤖 AI Agent:**
> Retrieving trending technology news... The top stories currently involve new AI regulations, a breakthrough in renewable energy storage, and the launch of a new flagship smartphone.


## ❓ FAQ

**Q: Can I filter web search results to only return specific types of content?**
Yes! While the `search_web` tool returns a broad mix, you can use specialized tools like `search_images`, `search_news`, or `search_videos` to target specific media types directly.

**Q: How do I see what is currently trending on the web?**
Simply ask the agent to `get_trending_news`. It will retrieve currently viral topics and news summaries from the Bing Trending engine.

**Q: Does this integration provide ad-free results?**
Yes. The Bing Search API returns raw structured data (JSON), which does not include the typical search engine advertisements found on the public website.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/bing-search](https://vinkius.com/mcp/bing-search)
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
3. Set Type to "SSE", enter `bing-search` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Bing Search** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "bing-search": {
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
