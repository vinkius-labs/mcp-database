# Zyte MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/zyte)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [data-analytics](../categories/data-analytics.md)

Extract structured web data, perform browser automation, and fetch search engine results directly through the Zyte API.

## Description
Connect your **Zyte API** account to any AI agent to bypass anti-bot measures and extract data from any website or search engine through natural conversation.

### What you can do

- **Web Extraction** — Download raw HTTP responses or browser-rendered HTML from any target URL.
- **Browser Automation** — Perform complex sequences of actions like clicking, scrolling, or waiting for elements before extraction.
- **Search Engine Results** — Fetch structured organic results from Google and other supported search domains.
- **Screenshots & Geolocation** — Capture JPEG/PNG screenshots and route requests through specific countries to see localized content.
- **Usage Monitoring** — Track your API consumption, costs, and success rates directly within the chat.

### How it works

1. Subscribe to this server
2. Enter your Zyte API Key (and optionally your Dashboard API Key for stats)
3. Start scraping and searching from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Data Scientists** — quickly gather datasets from the web without worrying about proxy rotation or headless browser management
- **SEO Specialists** — monitor search engine rankings and localized results across different geolocations
- **Developers** — debug web scrapers and inspect browser-rendered content directly from the code editor


## Available Tools (3)
- **extract_data**: Uses POST under the hood but acts as a read query.

Extract web data using Zyte API
- **search_data**: Uses POST under the hood but acts as a read query.

Search engine results via Zyte API
- **get_stats**: Requires ZYTE_DASHBOARD_API_KEY to be configured.

Get Zyte API usage stats


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Zyte** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Extract the browser-rendered HTML from https://news.ycombinator.com"

**🤖 AI Agent:**
> I've extracted the rendered content from Hacker News. The page contains the latest tech stories and discussions. Would you like me to parse the top headlines for you?

---

**👤 You:**
> "Search Google for 'best MCP servers' and give me the top 10 organic results."

**🤖 AI Agent:**
> Searching Google... I've found 10 organic results. The top links include GitHub repositories, developer blogs, and official documentation for Model Context Protocol servers.

---

**👤 You:**
> "Show me my current Zyte API usage and success rates."

**🤖 AI Agent:**
> Fetching your stats... You have made 1,250 requests this month with a 99.2% success rate. Your total estimated cost so far is $5.40.


## ❓ FAQ

**Q: Can I take a screenshot of a website using this server?**
Yes! Use the `extract_data` tool and set the `screenshot` parameter to true. The agent will return the visual state of the page as requested.

**Q: How do I get organic search results from Google?**
Use the `search_data` tool, specifying 'google.com' as the domain and your keywords as the query. You can also set `maxResults` to control the list length.

**Q: Is it possible to monitor my Zyte API spending?**
Yes, by using the `get_stats` tool. Note that this requires you to provide your `ZYTE_DASHBOARD_API_KEY` during setup.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/zyte](https://vinkius.com/mcp/zyte)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Zyte** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `zyte` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Zyte** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "zyte": {
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
