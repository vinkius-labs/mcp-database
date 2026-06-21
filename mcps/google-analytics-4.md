# Google Analytics 4 MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/google-analytics-4)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/google-analytics-4-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/google-analytics-4-mcp)
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


## Installation & Usage

To install and use the **Google Analytics 4** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/google-analytics-4](https://vinkius.com/mcp/google-analytics-4)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
