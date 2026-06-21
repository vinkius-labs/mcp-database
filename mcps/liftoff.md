# Liftoff MCP Server

Access mobile advertising performance reports and metadata via the Liftoff REST API.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/liftoff)

## Overview
**Category:** data-analytics
**Tools Count:** 7

## Description
Connect your **Liftoff** (formerly Vungle) advertising account to any AI agent to automate your mobile marketing analytics and reporting. This MCP server enables your agent to list campaigns, request detailed performance reports, and monitor spend in real-time directly from natural language interfaces.

### What you can do

- **Campaign Oversight** — List all apps, campaigns, and creative assets to map performance IDs to readable names
- **Automated Reporting** — Request asynchronous performance reports (v1) for deep dives into historical data
- **Real-time Spend** — Query synchronous spend and install metrics (v2) for immediate operational awareness
- **Lifecycle Tracking** — Monitor the status of report generation and download completed results effortlessly
- **Dimension Filtering** — Filter your data by app, campaign, country, and platform to identify growth opportunities

### How it works

1. Subscribe to this server
2. Enter your Liftoff API Key and API Secret
3. Start managing your advertising data from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **UA Managers** — Monitor campaign performance and spend totals via simple natural language commands
- **Data Analysts** — Automate the extraction of advertising metadata and performance logs into your workflow
- **Growth Marketers** — Quickly check recent install trends and click-through rates across different countries


## Available Tools
- **list_liftoff_apps**: List all applications in your Liftoff account
- **list_liftoff_campaigns**: List all advertising campaigns
- **request_performance_report**: Requires start and end dates.

Initialize a performance report request (v1)
- **list_liftoff_creatives**: List all creative assets
- **download_report_results**: Retrieve the data for a completed report
- **get_report_status**: Check the status of a requested report
- **get_spend_metrics**: Get a synchronous spend and performance report (v2)


## Installation & Usage

To install and use the **Liftoff** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/liftoff](https://vinkius.com/mcp/liftoff)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
