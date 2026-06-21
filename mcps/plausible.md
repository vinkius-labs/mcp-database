# Plausible MCP Server

Monitor website analytics via Plausible — track visitors, pageviews, and bounce rates directly from any AI agent.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/plausible)

## Overview
**Category:** data-analytics
**Tools Count:** 10

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


## Available Tools
- **get_aggregate_stats**: , for a period (e.g., "30d", "7d", "day").

Get aggregate site statistics
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


## Installation & Usage

To install and use the **Plausible** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/plausible](https://vinkius.com/mcp/plausible)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
