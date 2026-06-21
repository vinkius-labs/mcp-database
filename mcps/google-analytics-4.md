# Google Analytics 4 MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/google-analytics-4)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [industry-titans](../categories/industry-titans.md)

Understand your website and app traffic with event-based analytics that reveal user behavior, conversions, and growth trends.

## Description
Connect your **Google Analytics 4** property to any AI agent and access web analytics through natural conversation.

### What you can do

- **Custom Reports** — Run fully customizable GA4 reports with any combination of dimensions, metrics, and date ranges
- **Real-Time Analytics** — Monitor active users and current page views in real time
- **Page Performance** — Retrieve the top 25 pages ranked by views for any time period
- **Traffic Sources** — Analyze session sources and mediums to understand where visitors come from
- **User Demographics** — View user distribution by country for geographic insights
- **Device Breakdown** — See user distribution across desktop, mobile, and tablet
- **Conversions** — Track conversion events with counts and revenue data
- **Advanced Reporting** — Run pivot reports and batch multiple reports in a single request
- **Metadata & Compatibility** — List all available dimensions and metrics, and verify compatibility before building reports

### How it works

1. Subscribe to this server
2. Enter your Google OAuth Access Token and GA4 Property ID
3. Start querying your analytics from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Marketing Teams** — track campaign performance, traffic sources, and conversion funnels without opening the GA4 dashboard
- **Product Managers** — monitor feature adoption through page views and user engagement metrics
- **Growth Engineers** — analyze device breakdown, demographics, and real-time traffic patterns to optimize user experience


## Available Tools
- **batch_run_reports**: Batch run reports
- **check_compatibility**: Check report compatibility
- **get_conversions**: Get conversions
- **get_device_breakdown**: Get device breakdown
- **get_metadata**: Get available dimensions and metrics
- **get_page_views**: Get top pages by views
- **get_traffic_sources**: Get traffic sources
- **get_user_demographics**: Get user demographics
- **list_audience_exports**: List audience exports
- **run_pivot_report**: Run pivot report
- **run_realtime_report**: Run realtime report
- **run_report**: Data JSON must include dateRanges, dimensions, and metrics arrays.

Run a custom report


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Google Analytics 4** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Show me the top 10 pages by views this month and where the traffic is coming from."

**🤖 AI Agent:**
> Top 10 pages by views (this month): 1) /home — 42,300 views. 2) /pricing — 18,900. 3) /features — 12,400. 4) /blog/ai-tools-guide — 9,800. 5) /signup — 7,200. 6) /docs/getting-started — 6,100. 7) /about — 5,400. 8) /blog/2025-trends — 4,900. 9) /contact — 3,200. 10) /integrations — 2,800. Traffic sources: Google Organic (45.2%), Direct (22.1%), LinkedIn (12.8%), Twitter/X (8.4%), Referral (6.3%), Email (5.2%). Would you like to run a conversion report or see the device breakdown?

---

**👤 You:**
> "How many conversions did we get this week and which pages drove them?"

**🤖 AI Agent:**
> This week: 234 total conversion events. Breakdown by event: 'sign_up' (98 events, $0 revenue), 'purchase' (52 events, $4,680 revenue), 'begin_checkout' (84 events). Top converting pages: 1) /pricing → sign_up (42 conversions). 2) /features → sign_up (28). 3) /checkout → purchase (52). 4) /blog/ai-tools-guide → sign_up (18). Conversion rate (sessions → sign_up): 2.8%. Purchase conversion rate: 0.7%. Would you like to compare with last week or run a funnel report?

---

**👤 You:**
> "What devices are our users on and which countries are generating the most traffic?"

**🤖 AI Agent:**
> Device breakdown (last 30 days): Desktop 58.4% (24,100 users), Mobile 35.2% (14,500 users), Tablet 6.4% (2,640 users). User demographics by country: 1) United States — 34.2% (14,100 users). 2) United Kingdom — 12.8% (5,280). 3) Germany — 8.4% (3,460). 4) Canada — 7.1% (2,930). 5) Brazil — 6.3% (2,600). 6) France — 5.2% (2,140). Mobile traffic has grown 15% month-over-month. Would you like to run a device-specific conversion analysis?


## ❓ FAQ

**Q: Can I run custom reports with specific dimensions and metrics?**
Yes! The `run_report` tool accepts a JSON configuration with dateRanges, dimensions (e.g., pagePath, sessionSource), and metrics (e.g., sessions, screenPageViews, conversions). Use `get_metadata` to list all available dimensions and metrics, and `check_compatibility` to verify your combination is valid before running.

**Q: Does GA4 require two credentials — an access token and a property ID?**
Yes. You need a Google OAuth **Access Token** (for authentication via Bearer header) and a **GA4 Property ID** (numeric ID identifying your specific GA4 property). The Access Token can be generated via a Google Cloud Service Account with the Analytics Data API enabled. The Property ID is found in GA4 Admin > Property Settings.

**Q: Can I see real-time active users on my website?**
Yes. The `run_realtime_report` tool provides current active user data with real-time dimensions and metrics. For pre-built convenience reports, use `get_page_views` for top pages, `get_traffic_sources` for session sources, and `get_device_breakdown` for device distribution.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/google-analytics-4](https://vinkius.com/mcp/google-analytics-4)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Google Analytics 4** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `google-analytics-4` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Google Analytics 4** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "google-analytics-4": {
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
