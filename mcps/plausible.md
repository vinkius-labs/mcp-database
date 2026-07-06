# Plausible MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/plausible)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [data-analytics](../categories/data-analytics.md)

Monitor website analytics via Plausible — track visitors, pageviews, and bounce rates directly from any AI agent.

## Description
Connect your **Plausible Analytics** account to any AI agent and take full control of your website performance metrics through natural conversation.

### What you can do

- **Real-time Insights** — Get the current number of active visitors on your site.
- **Aggregate Performance** — Retrieve total visitors, pageviews, bounce rates, and visit durations for any period (30d, 7d, today).
- **Growth Tracking** — Fetch timeseries data to understand your traffic trends over time.
- **Audience Breakdown** — Analyze your visitors by top sources, pages, countries, devices, browsers, and operating systems.
- **Custom Property Analysis** — Break down stats by any custom property supported by the Plausible API.

### How it works

1. Subscribe to this server
2. Enter your Plausible API Key and Site ID (domain)
3. Start analyzing your traffic directly from Claude, Cursor, or any MCP client

### Who is this for?

- **Website Owners** — quickly check how many people are on your site or review yesterday's traffic while having a coffee.
- **Digital Marketers** — monitor top traffic sources and page performance during campaign reviews.
- **Product Managers** — audit feature adoption and user behavior trends directly from your chat interface.


## Available Tools (10)
- **get_custom_breakdown**: g., "visit:source", "event:page").

Get breakdown by custom property
- **get_realtime_visitors**: Get current active visitors
- **get_timeseries_stats**: Get site stats over time
- **get_top_browsers**: Get visitors by browser
- **get_top_countries**: Get visitors by country
- **get_top_devices**: Get visitors by device type
- **get_top_os**: Get visitors by operating system
- **get_top_pages**: Get most visited pages
- **get_top_sources**: Get top traffic sources
- **get_aggregate_stats**: , for a period (e.g., "30d", "7d", "day").

Get aggregate site statistics


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Plausible** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "How many visitors are on my site right now?"

**🤖 AI Agent:**
> There are currently 12 active visitors on your site.

---

**👤 You:**
> "Show me the top 5 pages by traffic for the last 7 days."

**🤖 AI Agent:**
> I've retrieved the top pages. The most visited are: 1. Home (/), 2. Pricing (/pricing), 3. Features (/features), 4. Blog (/blog/new-launch), and 5. Contact (/contact).

---

**👤 You:**
> "What was my bounce rate for the last 30 days?"

**🤖 AI Agent:**
> Your aggregate bounce rate for the last 30 days was 42.5%.


## ❓ FAQ

**Q: How do I find my Plausible API Key?**
In your Plausible account, go to **Settings** > **API keys**. There you can generate and copy your access token.

**Q: What is the Site ID?**
The Site ID is usually the domain of your website as registered in Plausible (e.g., `example.com`).

**Q: Can I see stats for today only?**
Yes! Use the `get_aggregate_stats` tool and provide `day` as the period parameter.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/plausible](https://vinkius.com/mcp/plausible)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Plausible** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `plausible` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Plausible** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "plausible": {
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
