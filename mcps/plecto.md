# Plecto MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/plecto)
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


## Available Tools (11)
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


## ❓ FAQ

**Q: Can I add a new data registration using my AI agent?**
Yes! Use the `create_data_registration` action. Provide the Data Source ID along with your data fields to feed your dashboard programmatically.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/plecto](https://vinkius.com/mcp/plecto)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Plecto** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `plecto` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Plecto** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "plecto": {
      "url": "https://edge.vinkius.com/[TOKEN]/mcp"
    }
  }
}
```

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
