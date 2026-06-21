# Insightful MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/insightful)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Manage employee productivity, time tracking, and activity via Insightful API.

## Description
Empower your AI agents to analyze and manage workforce productivity with Insightful (formerly Workpuls). This MCP server allows you to list employees and teams, track project progress, monitor real-time activity, and retrieve productivity and attendance reports directly through the Insightful API. Ideal for automating team management and performance monitoring.


## Available Tools
- **get_attendance**: Retrieves aggregated attendance and time tracking reports
- **get_employee**: Retrieves details for a specific employee
- **get_productivity**: Retrieves aggregated productivity reports
- **list_activity**: Lists recent employee activity logs
- **list_employees**: Lists all employees in the organization
- **list_locations**: Lists all registered organization locations
- **list_projects**: Lists all active and past projects
- **list_tasks**: Lists all tasks across projects
- **list_teams**: Lists all organization teams
- **list_webhooks**: Lists all configured webhooks


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Insightful** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all employees in the 'Engineering' team."

**🤖 AI Agent:**
> I'll fetch the employee list and filter for the engineering team from Insightful.

---

**👤 You:**
> "Show me the productivity report for last week."

**🤖 AI Agent:**
> I'll retrieve the aggregated productivity metrics for your organization.

---

**👤 You:**
> "Check recent activity logs for project ID '789'."

**🤖 AI Agent:**
> I'll look up the activity logs associated with that specific project.


## ❓ FAQ

**Q: How do I get Insightful API credentials?**
Log in to your Insightful dashboard as an Admin, navigate to Settings > API Tokens, and create a new token. Note that the token is only displayed once.

**Q: What is the productivity report?**
The get_productivity tool provides aggregated data on active, productive, and unproductive time for your employees and teams.

**Q: Can I see real-time activity?**
Yes, the list_activity tool provides access to recent activity logs recorded in your organization.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/insightful](https://vinkius.com/mcp/insightful)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Insightful** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `insightful` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Insightful** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "insightful": {
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
