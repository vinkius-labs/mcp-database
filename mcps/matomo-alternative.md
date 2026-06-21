# Matomo MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/matomo-alternative)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/matomo-alternative-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/matomo-alternative-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [data-analytics](../categories/data-analytics.md)

Track website traffic, analyze visitor behavior, and generate detailed analytics reports directly from your AI agent.

## Description
Connect your **Matomo** analytics instance to any AI agent and gain deep insights into your web traffic through natural conversation.

### What you can do

- **Real-time Tracking** — Track page views, custom events, and ecommerce actions using the `track_action` tool
- **Visits Summary** — Retrieve core metrics like total visits, unique visitors, and bounce rates with `get_visits_summary` 
- **Detailed Reporting** — Access human-readable processed reports for any site ID and time period using `get_processed_report` 
- **Metadata Discovery** — Explore all available API reports and functions for your specific instance via `get_report_metadata` 
- **Bulk Operations** — Send multiple tracking requests simultaneously to optimize data ingestion with `track_bulk` 

### How it works

1. Subscribe to this server
2. Enter your Matomo Instance URL and Auth Token
3. Start querying your analytics data from Claude, Cursor, or any MCP-compatible client

No more digging through complex dashboards to find your conversion rates or top-performing pages. Your AI acts as a dedicated data analyst.

### Who is this for?

- **Data Analysts** — quickly pull specific metrics and summaries without manual exports
- **Marketing Teams** — track campaign performance and event conversions in real-time
- **Developers** — verify tracking implementation and event triggers directly from the IDE


## Available Tools
- **get_image_graph**: get for a specific site and period.

Generate static PNG graph data
- **get_processed_report**: getProcessedReport to return full data set including metadata and processed metrics.

Get a processed human-readable report
- **get_report_metadata**: getReportMetadata to list available API functions and their metadata.

Get metadata for all available API reports
- **track_bulk**: Send multiple tracking requests in bulk
- **track_action**: Requires idsite.

Track a page view, event, or ecommerce action in Matomo
- **get_visits_summary**: get to retrieve metrics like nb_visits, nb_actions, bounce_count.

Get visits summary metrics
- **get_wp_processed_report**: Get processed report via WordPress REST API


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Matomo** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Get the visits summary for site ID 1 for the last 30 days."

**🤖 AI Agent:**
> I've retrieved the summary for site 1. In the last 30 days, you had 12,450 visits, 38,200 actions, and a bounce rate of 28.5%.

---

**👤 You:**
> "Track a page view for 'Pricing Page' on site 2 with URL 'https://example.com/pricing'."

**🤖 AI Agent:**
> The page view for 'Pricing Page' has been successfully tracked for site ID 2.

---

**👤 You:**
> "Show me the processed report for site 5 for today."

**🤖 AI Agent:**
> I've generated the processed report for site 5. Today's data shows 450 visits and 1,200 actions, with top referrers being Google and Direct entry.


## Installation & Usage

To install and use the **Matomo** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/matomo-alternative](https://vinkius.com/mcp/matomo-alternative)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
