# Simple Analytics MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/simple-analytics)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [data-analytics](../categories/data-analytics.md)

Privacy-first web analytics without cookies. Fetch aggregated stats, export raw data, and manage your websites directly from your AI agent.

## Description
Connect **Simple Analytics** to your AI agent for privacy-first insights. Simple Analytics provides clean, simple, and privacy-friendly web analytics without tracking users or using cookies.

### What you can do

- **Aggregated Stats** — Use `get_stats` to fetch pageviews, visitors, and histograms for any of your domains with custom date ranges.
- **Data Export** — Use `export_datapoints` to retrieve raw, non-sampled data for deep analysis or custom reporting.
- **Site Management** — List all managed websites with `list_websites` or add new domains to your account using `add_website`.
- **Server-Side Tracking** — Send custom events or pageviews directly from your server using `send_server_event` to track conversions or backend actions.

### How it works

1. Subscribe to this server
2. Enter your Simple Analytics API Key
3. Start querying your web traffic data through natural language in Claude, Cursor, or any MCP client

### Who is this for?

- **Data Analysts** — quickly pull traffic metrics and export raw data for spreadsheets or BI tools without manual exports
- **Marketing Managers** — check campaign performance and visitor trends across multiple domains using simple questions
- **Developers** — integrate server-side event tracking and monitor site health directly from the terminal or IDE


## Available Tools
- **add_website**: Requires Business or Enterprise plan.

Add a new website to Simple Analytics
- **export_datapoints**: Requires User-Id credential to be set.

Export raw, non-sampled data points
- **list_websites**: List all websites associated with the user
- **send_server_event**: Submit a server-side event or pageview
- **get_stats**: ) for a specific domain.

Get aggregated statistics for a website


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Simple Analytics** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Get the visitor count for example.com for the last 30 days."

**🤖 AI Agent:**
> I've retrieved the stats for example.com. In the last 30 days, you had 1,240 unique visitors and 3,100 total pageviews. Would you like to see a breakdown by day?

---

**👤 You:**
> "List all the websites I have registered in Simple Analytics."

**🤖 AI Agent:**
> You currently have 3 websites registered: 'example.com', 'blog.mysite.io', and 'app.dashboard.net'. Which one would you like to analyze?

---

**👤 You:**
> "Add a new website 'newproject.com' and set its timezone to 'Europe/London'."

**🤖 AI Agent:**
> Successfully added 'newproject.com' to your account with the Europe/London timezone. You can now start sending data to this hostname.


## ❓ FAQ

**Q: Can I see how many visitors my site had last week?**
Yes! Use the `get_stats` tool with your domain and set the `start` parameter to 'today-7d'. Your agent will return aggregated visitors and pageviews for that period.

**Q: Is it possible to export raw data for custom analysis?**
Absolutely. The `export_datapoints` tool allows you to retrieve raw, non-sampled data points in JSON or CSV format, provided you have your User-Id configured.

**Q: Can I track events that happen on my server, like a successful payment?**
Yes, use the `send_server_event` tool. You can specify the event name, hostname, and even include custom metadata to track backend conversions without any client-side scripts.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/simple-analytics](https://vinkius.com/mcp/simple-analytics)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Simple Analytics** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `simple-analytics` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Simple Analytics** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "simple-analytics": {
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
