# Octoboard MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/octoboard)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/octoboard-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/octoboard-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [industry-titans](../categories/industry-titans.md)

Build client-facing marketing reports automatically by pulling data from Google, Facebook, HubSpot, and 50 other integrations.

## Description
Connect your **Octoboard** account to any AI agent and take full control of your marketing business intelligence and reporting orchestration through natural conversation. Octoboard provides a powerful data visualization platform, and this integration allows you to retrieve dashboard metadata, push custom metrics to widgets, and monitor automated reports directly from your chat interface.

### What you can do

- **Dashboard & Report Orchestration** — List all active dashboards and retrieve detailed report metadata programmatically to ensure your team's visual insights are always synchronized.
- **Custom Data Intelligence** — Push numeric, text, or status metrics directly into Octoboard widgets from the AI interface to maintain real-time tracking of proprietary data.
- **Visual Data Control** — Send bar chart arrays, data tables, and variation metrics via natural language to drive better data transparency across your organization.
- **Agency & Client Oversight** — List managed clients and monitor account usage using simple AI commands to maintain a clear overview of your digital agency operations.
- **Operational Monitoring** — Track system responses and manage API health to ensure your reporting pipelines are always optimized.

### How it works

1. Subscribe to this server
2. Enter your Octoboard API Key from your account settings
3. Start managing your marketing metrics from Claude, Cursor, or any MCP-compatible client

No more manual data entry into reporting tools. Your AI acts as a dedicated data analyst or business intelligence coordinator.

### Who is this for?

- **Marketing Agencies** — quickly update custom client metrics and monitor dashboard health without switching apps.
- **Data Analysts** — automate the pushing of proprietary business data and track report delivery via natural conversation.
- **Business Owners** — streamline the retrieval of high-level revenue metrics and monitor organizational growth directly within the chat.


## Available Tools
- **get_api_status**: Check connection
- **check_api_usage**: Check data limits
- **list_agency_clients**: List managed clients
- **list_active_dashboards**: List dashboards
- **list_automated_reports**: List reports
- **push_bar_chart**: Update bar chart
- **push_numeric_metric**: Update widget number
- **push_status_update**: Update status indicator
- **push_data_table**: Update data table
- **push_text_metric**: Update widget text
- **push_variation_metric**: g. 10.5) to a widget.

Update value + change
- **test_octoboard_auth**: Verify credentials


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Octoboard** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all my active dashboards in Octoboard."

**🤖 AI Agent:**
> I've retrieved your dashboards. You have 3 active environments: 'Client A - Marketing', 'Internal Revenue', and 'SEO Performance'. Which one would you like to see metrics for?

---

**👤 You:**
> "Push a revenue metric of 48750 to my Executive KPI dashboard widget."

**🤖 AI Agent:**
> Done. The numeric metric $48,750 has been pushed to your Executive KPI dashboard. The widget now displays the updated value with a 12% increase indicator compared to the previous period. The dashboard will refresh for all viewers within 30 seconds.

---

**👤 You:**
> "List all automated reports and their delivery schedules."

**🤖 AI Agent:**
> You have 4 automated reports configured. "Weekly SEO Summary" sends every Monday at 9 AM to marketing@company.com. "Monthly Client Report" generates the 1st of each month for 6 agency clients. "Daily Ad Spend" delivers at 8 AM to the growth team. "Quarterly Executive Review" runs every quarter end.


## Installation & Usage

To install and use the **Octoboard** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/octoboard](https://vinkius.com/mcp/octoboard)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
