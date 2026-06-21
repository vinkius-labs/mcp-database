# GrowingIO MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/growingio)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/growingio-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/growingio-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [marketing-automation](../categories/marketing-automation.md)

Leading product analytics platform in China — manage events, segments, and metrics via AI.

## Description
Empower your AI agent to orchestrate your product analytics and user behavioral data with **GrowingIO**, the premier analytical platform in China. By connecting GrowingIO to your agent, you transform complex event tracking, user segmentation, and metric analysis into a natural conversation. Your agent can instantly list tracked events, retrieve detailed user segment metadata, monitor conversion funnels, and execute quantitative metric queries without you ever needing to navigate the comprehensive GrowingIO web interface. Whether you are conducting a product health audit or monitoring real-time campaign performance, your agent acts as a real-time data analyst assistant, keeping your product data accurate and your growth moving.

### What you can do

- **Event Orchestration** — List and retrieve detailed metadata for all tracked behavioral events in your project.
- **User Segmentation** — Browse and monitor user segments to identify high-value cohorts and behavioral patterns.
- **Metric Querying** — Execute quantitative queries to retrieve specific performance metrics via natural language.
- **Funnel Auditing** — Retrieve detailed configuration and data for conversion funnels to identify drop-off points.
- **Campaign Insights** — Browse tracked advertising campaigns and identify successful growth drivers.

### How it works

1. Subscribe to this server
2. Enter your GrowingIO Project ID, Client ID, and API Token
3. Start managing your product analytics through Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Product Managers** — monitor feature adoption and audit user behavior through natural language queries.
- **Growth Engineers** — coordinate user segments and monitor campaign performance directly from your AI-powered workspace.
- **Data Analysts** — retrieve system metrics and perform funnel analysis via a unified AI interface.
- **GrowingIO Power Users** — integrate your existing analytics workflows into your AI-driven daily routines.


## Available Tools
- **get_event**: Get event details
- **get_funnel**: Get conversion funnel details
- **get_metrics**: Query project metrics
- **get_project_info**: Get project metadata
- **get_segment_users**: Get users in a segment
- **list_ads**: List advertising campaigns
- **list_events**: List project events
- **list_log_sources**: ).

List data log sources
- **list_segments**: List user segments
- **list_variables**: List tracked variables


## 💬 Prompt Examples

Here are some examples of how you can interact with the **GrowingIO** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all user segments in GrowingIO."

**🤖 AI Agent:**
> I've retrieved your GrowingIO segments. You have 15 defined cohorts, including 'Power Users', 'At-Risk Users', and 'New Signups'. Which one would you like to see the user list for?

---

**👤 You:**
> "Show me the conversion funnel for 'Checkout Flow'."

**🤖 AI Agent:**
> I've retrieved the details for the Checkout Flow funnel. Current conversion rate is 42% from 'Add to Cart' to 'Purchase Complete'. The biggest drop-off is at the 'Shipping Info' step. Would you like to see the breakdown per device type?

---

**👤 You:**
> "Query the DAU for the last 7 days."

**🤖 AI Agent:**
> Across the last 7 days, your Daily Active Users (DAU) averaged 12,500, peaking at 14,200 on Wednesday. This represents a 5% increase compared to the previous week. Should I retrieve the metrics for Weekly Active Users (WAU) as well?


## Installation & Usage

To install and use the **GrowingIO** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/growingio](https://vinkius.com/mcp/growingio)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
