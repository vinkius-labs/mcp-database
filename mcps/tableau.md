# Tableau MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/tableau)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/tableau-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/tableau-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [industry-titans](../categories/industry-titans.md)

Access workbooks, views, data sources, and dashboard insights from Tableau — the enterprise BI and analytics platform.

## Description
Connect your **Tableau Cloud** or **Tableau Server** to any AI agent and explore business intelligence through natural conversation.

### What you can do

- **Workbooks** — List, search, and retrieve workbook metadata and connections
- **Views** — Query dashboard views, download rendered images, and access underlying data
- **Data Sources** — List published data sources with freshness and connection details
- **Sites & Projects** — Navigate the site hierarchy and project structure
- **Users & Groups** — Query user membership, roles, and permissions
- **Jobs** — Monitor extract refresh jobs and background task status

### Who is this for?

- **Data Analysts** — find and explore dashboards without navigating the portal
- **BI Admins** — monitor extract jobs and data freshness through chat
- **Executives** — ask questions about KPIs and get dashboard summaries
- **Data Engineers** — audit data source connections and refresh schedules


## Available Tools
- **list_workbooks**: List Tableau workbooks
- **get_workbook**: Get workbook details
- **list_views**: List all views (dashboards)
- **list_datasources**: Useful for monitoring data freshness.

List published data sources
- **list_projects**: List projects in the site
- **list_users**: List site users
- **list_jobs**: List background jobs


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Tableau** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Show me all workbooks in the Sales project."

**🤖 AI Agent:**
> Found 12 workbooks in 'Sales': 1. 'Q1 Pipeline Dashboard' (updated 2h ago, 3 views). 2. 'Revenue by Region' (updated yesterday, 5 views). 3. 'Win Rate Analysis' (updated 3d ago, 2 views).

---

**👤 You:**
> "What data sources haven't been refreshed in over 24 hours?"

**🤖 AI Agent:**
> 3 stale data sources: 1. 'Salesforce_Opps' — last refresh: 36h ago (FAILED). 2. 'GA4_Metrics' — 28h ago (success). 3. 'HR_Headcount' — 48h ago (FAILED). Recommend checking extract schedules.

---

**👤 You:**
> "How many active users accessed Tableau this week?"

**🤖 AI Agent:**
> Active users this week: 142 unique logins. Viewers: 98 (69%). Explorers: 31 (22%). Creators: 13 (9%). Peak activity: Tuesday 10AM (89 concurrent). Most viewed: 'Executive KPI Dashboard' (245 views).


## Installation & Usage

To install and use the **Tableau** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/tableau](https://vinkius.com/mcp/tableau)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
