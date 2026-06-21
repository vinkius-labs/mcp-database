# Northbeam MCP Server

Analyze marketing attribution via Northbeam — track metrics, breakdowns, and data exports directly from your AI agent.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/northbeam)

## Overview
**Category:** ecommerce
**Tools Count:** 10

## Description
Connect your **Northbeam** account to your AI agent and gain deep insights into your marketing performance and attribution data through natural conversation.

### What you can do

- **Metric Discovery** — List all available performance metrics such as Attributed Revenue, Transactions, and Spend.
- **Data Breakdowns** — Access the labels used to group your data, including Platform, Campaign, Ad Set, and more.
- **Attribution Modeling** — View supported attribution models to understand how credit is assigned across touchpoints.
- **Programmatic Exports** — Initialize new data exports for specific date ranges and sets of metrics.
- **Export Monitoring** — Track the status of your active data exports and retrieve direct download URLs for results.
- **Workspace Oversight** — Monitor active webhooks, scheduled recurring exports, and recent export history.
- **Account Insights** — Access high-level configuration, dashboard settings, and authenticated account metadata.

### How it works

1. Subscribe to this server
2. Enter your Northbeam API Key and Data Client ID
3. Start analyzing your marketing attribution from Claude, Cursor, or any MCP client

### Who is this for?

- **Marketing Managers** — quickly check available metrics or export statuses without opening the Northbeam dashboard.
- **Data Analysts** — automate the retrieval of complex attribution data for deeper reporting and modeling.
- **Growth Teams** — monitor recently completed exports and verify data synchronization in real-time.


## Available Tools
- **get_dashboard_settings**: Get workspace dashboard settings
- **list_breakdowns**: g., Platform, Campaign, Ad Set) in attribution reports.

List available data breakdowns
- **list_metrics**: g., Attributed Revenue, Transactions, Spend) available for export.

List available attribution metrics
- **list_attribution_models**: g., Clicks only, Modeled).

List supported attribution models
- **list_recent_exports**: List recently completed exports
- **list_scheduled_exports**: List scheduled data exports
- **list_webhooks**: List active webhooks
- **create_data_export**: Initialize a new data export
- **get_export_status**: Check data export status
- **get_account_info**: Get account metadata


## Installation & Usage

To install and use the **Northbeam** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/northbeam](https://vinkius.com/mcp/northbeam)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
