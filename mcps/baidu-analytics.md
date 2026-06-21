# Baidu Analytics / 百度统计 MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/baidu-analytics)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [industry-titans](../categories/industry-titans.md)

China's leading web analytics platform — audit traffic, track visitors, and query site metrics via AI.

## Description
Empower your AI agent to orchestrate your web analytics and visitor insights with **Baidu Analytics** (百度统计), the dominant traffic analysis platform in China. By connecting Baidu Analytics to your agent, you transform complex metric reporting, real-time visitor tracking, and source auditing into a natural conversation. Your agent can instantly retrieve site lists, query real-time PV/UV data, audit daily visitor trends, and generate custom performance reports without you ever needing to navigate the comprehensive Baidu Tongji Dashboard. Whether you are conducting a digital marketing audit or monitoring the performance of a new landing page, your agent acts as a real-time data coordinator, providing accurate results from a single, authorized source.

### What you can do

- **Site Orchestration** — List all registered sites and verify target Site ID configurations for precise data access.
- **Real-time Auditing** — Retrieve immediate visitor metrics including Page Views (PV), Unique Visitors (UV), and online user counts.
- **Trend Analysis** — Audit daily traffic trends and high-level performance summaries for specific date ranges.
- **Performance Auditing** — Query page rankings, geographic distributions, and traffic source details.
- **Custom Reporting** — Execute advanced queries on site data using flexible API methods and metrics.

### How it works

1. Subscribe to this server
2. Enter your Baidu Analytics Username, Password, Token, and Site ID
3. Start managing your site analytics through Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Digital Marketers** — automate routine traffic reports and monitor campaign performance through natural language.
- **Product Managers** — audit visitor behavior and page rankings directly from your AI-powered workspace.
- **Developers** — integrate professional-grade web analytics into your AI-driven daily routines.
- **Baidu Analytics Power Users** — integrate your existing Tongji workflows into your AI-driven daily routines.


## Available Tools
- **get_daily_trend**: Get daily traffic trend
- **get_geo_distribution**: Get visitor geographic data
- **get_page_rankings**: Get top visited pages
- **get_realtime_metrics**: Get real-time statistics
- **get_source_data**: g., search, direct).

Get visitor sources
- **get_yesterday_overview**: Get yesterday traffic summary
- **list_sites**: List all analytics sites
- **query_custom_metrics**: Execute custom report query


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Baidu Analytics / 百度统计** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Check the real-time visitor stats for my site."

**🤖 AI Agent:**
> I've retrieved the real-time metrics. You currently have 45 users online. Total Page Views (PV) for today so far is 1,240, with 850 Unique Visitors (UV). Would you like me to check which pages they are currently visiting?

---

**👤 You:**
> "Show me the visitor trend for the last 7 days."

**🤖 AI Agent:**
> I've analyzed the traffic trend for the past week. Daily UV peaked on Wednesday at 2,500 and averaged around 1,800. Overall traffic is up by 12% compared to the previous week. Should I provide a breakdown of the traffic sources for this period?

---

**👤 You:**
> "List all sites in my Baidu Analytics account."

**🤖 AI Agent:**
> I've retrieved your site list. You have 3 sites registered: 'myshop.com' (ID: `8821`), 'blog.example.cn' (ID: `9920`), and 'app-landing.com' (ID: `1024`). Which site would you like to audit today?


## ❓ FAQ

**Q: How do I find my Baidu Analytics Token and Site ID?**
Log in to the [Baidu Analytics Console](https://tongji.baidu.com/), navigate to [Management] -> [Site List] to find your numeric Site ID. The API Token is usually provided in the API settings or developer services section after account verification.

**Q: What metrics are supported in real-time queries?**
Real-time tools provide access to Page Views (PV), Unique Visitors (UV), IP counts, and the current number of online users on your site.

**Q: Can I query data for specific dates?**
Yes! Use the trend and metric tools with `start_date` and `end_date` in `YYYYMMDD` format. Your agent will retrieve the historical data for the requested period.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/baidu-analytics](https://vinkius.com/mcp/baidu-analytics)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Baidu Analytics / 百度统计** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `baidu-analytics` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Baidu Analytics / 百度统计** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "baidu-analytics": {
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
