# Serper MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/serper-alternative)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [data-analytics](../categories/data-analytics.md)

Perform fast Google searches — audit web results, images, news, and places via AI.

## Description
Empower your AI agent to orchestrate your entire web discovery workflow with **Serper**, the high-speed Google Search API. By connecting Serper to your agent, you transform complex search tasks into a natural conversation. Your agent can instantly audit organic search results, track news trends, and retrieve local business data without you ever touching a browser. Whether you are conducting market research or monitoring brand mentions, your agent acts as a real-time data analyst, ensuring your web intelligence is always grounded in live search data.

### What you can do

- **Web Auditing** — Query organic Google search results and retrieve detailed snippets and links for any topic instantly.
- **Visual Intelligence** — Search for images and videos on Google to maintain a clear view of visual content trends.
- **News & Trend Oversight** — Monitor real-time news results to stay on top of industry developments and PR updates.
- **Local Discovery** — Search for places and local businesses to understand geographic distributions and venue details.
- **Academic & IP Intelligence** — Query Google Scholar for research papers and search for patents to maintain strict control over intellectual property research.

### How it works

1. Subscribe to this server
2. Enter your Serper API Key
3. Start managing your web intelligence through Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Market Researchers** — monitor search engine results and competitor snippets straight from your workflow.
- **Content Strategists** — verify trending news and image results to plan your next publication.
- **Operations Leads** — automate place querying to orchestrate cross-functional geographic strategy smoothly.
- **IP Analysts** — perform rapid audits of patents and scholarly articles without manual browser searches.


## Available Tools (10)
- **get_autocomplete**: Get Google autocomplete suggestions
- **search_google**: Perform a Google search for organic results
- **search_images**: Search for images on Google
- **search_maps**: Search for locations on Google Maps
- **search_news**: Search for news results on Google
- **search_patents**: Search for patents on Google
- **search_places**: Search for places and local businesses
- **search_scholar**: Search for academic papers on Google Scholar
- **search_shopping**: Search for shopping results on Google
- **search_videos**: Search for videos on Google


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Serper** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Search Google for 'best MCP servers 2024'."

**🤖 AI Agent:**
> I've retrieved the organic search results. Top matches include articles from Vinkius and GitHub. Would you like the snippets and links for the top 5 results?

---

**👤 You:**
> "What is the latest news about 'SpaceX Starship'?"

**🤖 AI Agent:**
> I've scanned Google News. There are 3 recent reports about the latest launch attempt and upcoming mission milestones. Would you like the full headlines and sources?

---

**👤 You:**
> "Find pizza restaurants in 'Seattle, WA'."

**🤖 AI Agent:**
> I've found 5 top-rated pizza places in Seattle. Notable results include 'Serious Pie' and 'Delancey'. I can provide the addresses and average ratings for each.


## ❓ FAQ

**Q: How do I find my Serper API Key?**
Log in to your [**Serper.dev dashboard**](https://serper.dev/dashboard), and you will find your API Key on the main page. Copy and paste it below.

**Q: Can the agent search for images and news separately?**
Yes. This server includes specialized tools for Google Images (`search_images`) and Google News (`search_news`), allowing your agent to query specific verticals based on your needs.

**Q: Is it possible to retrieve local business details via the agent?**
Yes. The `search_places` tool allows your agent to query Google Places for business information, including addresses and ratings, ensuring your local research is accurate.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/serper-alternative](https://vinkius.com/mcp/serper-alternative)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Serper** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `serper-alternative` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Serper** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "serper-alternative": {
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
