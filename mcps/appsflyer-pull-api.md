# AppsFlyer (Pull API) MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/appsflyer-pull-api)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/appsflyer-pull-api-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/appsflyer-pull-api-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [marketing-automation](../categories/marketing-automation.md)

Retrieve raw and aggregate attribution data from AppsFlyer — track installs, events, and performance via AI.

## Description
The **AppsFlyer Pull API MCP Server** provides your AI agent with direct access to your mobile attribution and marketing analytics data. Effortlessly retrieve raw reports for installs and in-app events, or get aggregate performance metrics by day, geography, or media source using natural language.

### Key Features

- **Raw Data Retrieval** — Download non-organic installs, in-app events, and uninstalls reports for granular analysis.
- **Aggregate Reporting** — Access high-level performance summaries by partner (media source), geography, or day.
- **Customizable Timeframes** — Specify exact start and end dates for any report to focus on specific campaigns or periods.
- **CSV Output Support** — Reports are delivered in structured CSV format, allowing for further data processing or direct review.
- **Security & Privacy** — Uses AppsFlyer API Token V2 (JWT) for secure, authenticated access to your data.

### Who is this for?

- **UA Managers** — Quickly audit campaign performance and install trends across different partners.
- **Data Analysts** — Retrieve raw event data for deeper investigation into user behavior and LTV.
- **Growth Marketers** — Monitor daily performance and geographic trends to optimize spend and targeting.


## Available Tools
- **get_account_check**: Verify AppsFlyer account connection
- **get_daily_report**: Get aggregate daily performance report
- **get_geo_report**: Get aggregate performance report by geography
- **get_in_app_events_report**: Get in-app events raw data report
- **get_installs_report**: Get non-organic installs raw data report
- **get_partners_report**: Get aggregate performance report by media source
- **get_uninstalls_report**: Get uninstalls raw data report


## 💬 Prompt Examples

Here are some examples of how you can interact with the **AppsFlyer (Pull API)** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Get the installs report for last week."

**🤖 AI Agent:**
> I've retrieved your installs report for the last 7 days. It includes details for 1,250 non-organic installs from various media sources.

---

**👤 You:**
> "Show me the aggregate daily performance for February 2024."

**🤖 AI Agent:**
> I've pulled the daily performance report for February. You had a total of 15,400 installs and 45,000 sessions during this period.

---

**👤 You:**
> "Retrieve in-app events data for today."

**🤖 AI Agent:**
> The in-app events report for today has been retrieved. There are 250 records so far, including 'purchase' and 'level_complete' events.


## Installation & Usage

To install and use the **AppsFlyer (Pull API)** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/appsflyer-pull-api](https://vinkius.com/mcp/appsflyer-pull-api)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
