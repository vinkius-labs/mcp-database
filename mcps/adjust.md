# Adjust MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/adjust)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/adjust-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/adjust-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [marketing-automation](../categories/marketing-automation.md)

Mobile measurement and attribution — track app installs, events, and performance via AI.

## Description
Connect your **Adjust** account to your AI agent to unlock professional mobile measurement and attribution insights. From auditing app settings to inspecting device attribution and monitoring key performance indicators (KPIs), your agent handles your mobile growth data through natural conversation.

### What you can do

- **App Automation** — Retrieve and audit technical settings for your mobile applications, including event tokens and partner parameters
- **Device Inspection** — Verify the attribution status of specific devices using their advertising IDs (ADID) for testing and support
- **KPI Monitoring** — Retrieve aggregated performance metrics like installs, clicks, and sessions to monitor app growth
- **Event Tracking Audit** — List active event tokens and verify that your in-app events are correctly configured
- **Attribution Oversight** — Quickly identify which networks and campaigns are driving the most high-value users directly from chat

### How it works

1. Subscribe to this server
2. Enter your Adjust API Token
3. Start managing your mobile measurement and monitoring attribution through Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **User Acquisition (UA) Managers** — monitor campaign performance and attribution patterns instantly
- **Mobile Developers** — verify event configurations and inspect device attribution during integration tests
- **Growth Analysts** — retrieve KPI reports for daily performance audits and ROI analysis
- **Marketing Operations** — audit app settings and event tokens across multiple mobile platforms


## Available Tools
- **get_app_settings**: Get app configuration
- **inspect_device**: Inspect device attribution
- **get_kpi_report**: Filterable by date.

Get aggregated KPI metrics


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Adjust** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Retrieve the settings for my app with token 'abcdef123456'."

**🤖 AI Agent:**
> I've retrieved the settings for app 'abcdef123456'. I can see your active event tokens, attribution windows, and configured partners. Would you like to check a specific event configuration?

---

**👤 You:**
> "Inspect the attribution status for ADID '12345-67890'."

**🤖 AI Agent:**
> I've inspected ADID '12345-67890'. This device is currently attributed to the 'Summer Campaign' on Google Ads. It was last seen 2 hours ago.

---

**👤 You:**
> "Show me the total installs for last week."

**🤖 AI Agent:**
> I've pulled the KPI report. Last week, your apps generated a total of 15,400 installs, which is an 8% increase compared to the previous week. Would you like to see the breakdown by platform?


## Installation & Usage

To install and use the **Adjust** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/adjust](https://vinkius.com/mcp/adjust)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
