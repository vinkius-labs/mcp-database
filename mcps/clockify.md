# Clockify MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/clockify)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Manage time tracking and projects via Clockify — track entries, monitor projects, and audit team hours directly from any AI agent.

## Description
Connect your **Clockify** account to any AI agent and take full control of your time tracking and project management through natural conversation. Streamline how you monitor work hours and team productivity natively.

### What you can do

- **Workspace Oversight** — List and retrieve details for all workspaces you have access to natively
- **Project Intelligence** — Access and monitor all projects and clients configured in your account flawlessly
- **Time Tracking** — List and retrieve details for all time entries for any user in your team securely
- **Timer Management** — Start and stop timers directly from your chat interface to ensure accurate logging flawlessly
- **Team Logistics** — List all users and team members within a workspace to understand allocation securely
- **Productivity Auditing** — Retrieve detailed time entry metadata including descriptions and project associations flawlessly

### How it works

1. Subscribe to this server
2. Enter your Clockify API Key (found in Settings > My Profile)
3. Start managing your time tracking from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Project Managers** — monitor team hours and project progress using natural language
- **Freelancers** — quickly log time and verify billable hours without opening the dashboard
- **Operations Teams** — quickly look up project assignments and user rosters straight from their chat interface
- **HR Teams** — verify timesheet completeness and team member status


## Available Tools (8)
- **add_new_time_entry**: Add a new time entry to a workspace
- **get_my_clockify_profile**: Retrieve information about the authenticated user
- **list_workspace_clients**: List all clients configured in a workspace
- **list_workspace_projects**: List all projects within a specific workspace
- **list_user_time_entries**: List time entries for a specific user in a workspace
- **list_workspace_users**: List all users within a specific workspace
- **list_clockify_workspaces**: List all workspaces the user has access to
- **stop_current_timer**: Stop the currently running timer for a specific user


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Clockify** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all my Clockify workspaces."

**🤖 AI Agent:**
> Retrieving your Clockify workspaces... I found 2: 'Engineering Team' (ID: 1234) and 'Marketing Ops' (ID: 5678). Which one would you like to see projects for?

---

**👤 You:**
> "Show me the last 5 time entries for user 'John Doe'."

**🤖 AI Agent:**
> Checking time entries for John Doe... I found 5 items: 'Bug fixing' (2.0 hrs), 'API Integration' (4.5 hrs), 'Team Sync' (1.0 hr), and 2 others. All were logged against the 'Vinkius Cloud' project.

---

**👤 You:**
> "Stop my running timer in the 'Engineering' workspace."

**🤖 AI Agent:**
> Stopping your timer... The active timer for 'API Research' has been successfully stopped. It was logged for 1 hour and 15 minutes.


## ❓ FAQ

**Q: Can I stop a running timer through the agent?**
Yes! Use the `stop_current_timer` tool. Provide your workspace and user ID, and the agent will instruct Clockify to stop the active timer immediately.

**Q: How do I see the projects for a specific workspace?**
Use the `list_workspace_projects` tool with the workspace ID. Your agent will fetch all projects, allowing you to see which ones are billable and their associated clients.

**Q: Where do I find my Clockify API Key?**
Log in to Clockify, go to **Settings**, and select **My Profile**. Scroll to the bottom to find and generate your API Key.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/clockify](https://vinkius.com/mcp/clockify)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Clockify** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `clockify` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Clockify** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "clockify": {
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
