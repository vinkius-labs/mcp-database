# Plecto MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/plecto)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/plecto-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/plecto-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Automate KPI dashboards and data tracking via Plecto — manage registrations, dashboards, and teams directly from any AI agent.

## Description
Connect your **Plecto** account to any AI agent and simplify your KPI tracking, performance management, and dashboard orchestration through natural conversation.

### What you can do

- **Data Registrations** — List all data entries for any data source, retrieve detailed metadata, and monitor real-time values
- **Direct Execution** — Create new data registrations programmatically directly from your agent to feed your dashboards
- **KPI Dashboards** — Query all configured KPI dashboards and retrieve detailed metadata to monitor performance
- **Team Coordination** — List organizational teams and employees to manage access and resource allocation
- **Data Sources** — Query all configured data sources to choose the right context for each interaction

### How it works

1. Subscribe to this server
2. Enter your Plecto API Token from your account settings
3. Start managing your performance dashboards from Claude, Cursor, or any MCP-compatible client


## Available Tools
- **get_dashboard**: Get details for a specific dashboard
- **get_employee**: Get details for a specific employee
- **get_registration**: Get details for a specific data registration
- **list_formulas**: List all KPI formulas
- **list_widgets**: List all widgets on a dashboard
- **create_data_registration**: Add a new data entry
- **list_kpi_dashboards**: List Plecto dashboards
- **list_data_sources**: List Plecto data sources
- **list_account_employees**: List account employees
- **list_data_registrations**: List Plecto registrations
- **list_organizational_teams**: List teams


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Plecto** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all my KPI dashboards in Plecto."

**🤖 AI Agent:**
> I've retrieved your dashboards. You have 5 active KPI boards, including 'Sales Team Overview' and 'Customer Support Live'.

---

**👤 You:**
> "Show me the sales leaderboard for the current month with all team member performance metrics."

**🤖 AI Agent:**
> Sales leaderboard for May 2025. Top performer: Sarah Chen with $127,400 in closed revenue (142% of target). Second: James Park at $98,200 (109%). Third: Lisa Wang at $87,600 (97%). Team average: $72,300. Total team revenue: $578,400 against a $600,000 target (96.4%). 3 team members are below 80% of their individual targets. The "Enterprise Deals" data source was last synced 15 minutes ago.

---

**👤 You:**
> "Register a new data point for Sarah Chen with $45,000 in closed deals today on the Revenue data source."

**🤖 AI Agent:**
> Data registration created successfully. Employee: Sarah Chen. Data source: Revenue. Value: $45,000. Date: May 13, 2025. This brings Sarah's monthly total to $172,400 (191% of target). She is now #1 on the leaderboard. The dashboard widgets have been updated automatically and a notification was sent to her team manager. Achievement badge "Top Closer" triggered.


## Installation & Usage

To install and use the **Plecto** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/plecto](https://vinkius.com/mcp/plecto)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
