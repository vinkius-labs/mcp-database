# ClickTime MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/clicktime)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Manage time tracking and resource planning via ClickTime — track entries, monitor projects, and audit client hours directly from any AI agent.

## Description
Connect your **ClickTime** account to any AI agent and take full control of your time tracking and resource management through natural conversation. Streamline how you monitor billable hours and project progress natively.

### What you can do

- **Time Oversight** — List and retrieve details for all time entries including hours and descriptions natively
- **Project Intelligence** — Access and monitor all projects and clients configured in your account flawlessly
- **Resource Management** — List all users and people in the company to understand team allocation securely
- **Task Logistics** — Access work types and tasks available for time tracking to ensure accurate data entry flawlessly
- **Reporting Deep-Dives** — Retrieve high-volume time reports and daily completeness summaries flawlessly
- **User Visibility** — Access your own profile and API authentication details directly within your workspace

### How it works

1. Subscribe to this server
2. Enter your ClickTime API Token (obtainable via the /Me endpoint with your credentials)
3. Start managing your time tracking from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Project Managers** — monitor project hours and billable time using natural language
- **Accountants** — audit time entry completeness and user rosters without opening the dashboard
- **Operations Teams** — quickly look up client IDs and task types straight from their chat interface
- **Individual Contributors** — verify their own time entries and profile information


## Available Tools
- **get_my_clicktime_profile**: Retrieve information about the currently authenticated user
- **get_high_volume_time_report**: Retrieve a high-volume report of time entries (up to 2500 records)
- **list_clicktime_clients**: List all clients configured in ClickTime
- **list_clicktime_jobs**: List all jobs (active and inactive) in the system
- **list_clicktime_projects**: List all projects configured in ClickTime
- **list_clicktime_tasks**: List all tasks (work types) available for time tracking
- **list_time_entries**: List time tracking entries
- **list_clicktime_users**: List all people and users in the company


## 💬 Prompt Examples

Here are some examples of how you can interact with the **ClickTime** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all time entries from today in ClickTime."

**🤖 AI Agent:**
> Retrieving your time entries for today... I found 2 entries: 'Internal Meeting' (1.5 hrs) and 'Feature Development' (4.0 hrs). Total so far is 5.5 hours.

---

**👤 You:**
> "Show me all clients configured in my account."

**🤖 AI Agent:**
> Checking client list... You have 5 active clients: Acme Corp, Global Tech, Startup Inc, Fast Services, and Blue Media. Would you like to see projects for any of these?

---

**👤 You:**
> "What is the high-volume time report status?"

**🤖 AI Agent:**
> Retrieving high-volume report... The system returned 2,150 time entries for the current period. All records are processed and ready for analysis.


## ❓ FAQ

**Q: Can I see my total hours for this week?**
Yes! Use the `list_time_entries` tool. The agent will return your recent entries, and you can ask it to sum the hours for the current week.

**Q: How do I check which projects are currently active?**
Use the `list_clicktime_projects` tool. Your agent will fetch all projects in the system, including their names and statuses.

**Q: Where do I find my ClickTime API Token?**
You can obtain your token by making a Basic Auth request to the `GET /Me` endpoint using your email and password. Alternatively, check your ClickTime profile or contact your administrator.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/clicktime](https://vinkius.com/mcp/clicktime)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **ClickTime** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `clicktime` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **ClickTime** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "clicktime": {
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
