# timeghost MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/timeghost)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Log working hours directly from Microsoft Teams and Outlook with time tracking that integrates into the tools you already use.

## Description
Connect your **timeghost** account to any AI agent and take full control of your Microsoft 365 integrated time tracking and project orchestration through natural conversation.

### What you can do

- **Timesheet Portfolio Orchestration** — List all time entries, retrieve detailed high-fidelity status metadata, and monitor team productivity programmatically
- **Project Intelligence Architecture** — Query projects and budgets, retrieve detailed technical metadata, and access real-time project health metrics
- **Task Pipeline Management** — Access your complete directory of high-fidelity tasks, manage assignments, and stay on top of operational delivery directly through your agent
- **Workspace Discovery** — Access complete high-fidelity workspace profiles and organizational settings to understand and orchestrate your environment programmatically
- **Contact & Team Monitoring** — List team members and collaborators to maintain perfect contextual alignment for every time log and project assignment
- **Operational Monitoring** — Verify account-level API connectivity and monitor time log orchestration volume directly through your agent for perfectly coordinated service scaling

### How it works

1. Subscribe to this server
2. Retrieve your **API Token** from your timeghost account (Settings > API Keys)
3. Start managing your time-tracking growth from Claude, Cursor, or any MCP client

No more manual timesheet entries or missing project budget gaps. Your AI acts as your dedicated project coordinator and time tracking architect.

### Who is this for?

- **Project Managers** — instantly retrieve task lists and project budget statuses using natural language commands without leaving your creative workspace
- **Team Leads** — monitor high-fidelity time entries and team utilization to ensure healthy and productive operations
- **HR & Payroll Admins** — verify technical time logs and workspace assignments to optimize resource allocation through simple AI queries


## Available Tools (10)
- **list_timeghost_clients**: List clients
- **get_timeghost_project**: Get details for a specific project
- **get_timeghost_task**: Get details for a specific task
- **get_timeghost_entry**: Get a specific time entry
- **list_timeghost_projects**: List projects
- **check_timeghost_status**: Check API Status
- **list_timeghost_tasks**: Filter by project ID to isolate specific technical pipelines.

List tasks
- **list_timeghost_entries**: Optionally filter by date range or specific user.

List time entries
- **list_timeghost_members**: List workspace members
- **list_timeghost_workspaces**: List workspaces


## 💬 Prompt Examples

Here are some examples of how you can interact with the **timeghost** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all active projects in my timeghost account."

**🤖 AI Agent:**
> I've retrieved your projects. You currently have 8 active high-fidelity projects, including 'App Development' (Budget: 80% used) and 'Q2 Marketing'. Would you like the detailed health metadata for any of them?

---

**👤 You:**
> "Show the last 5 time entries for task 'API Design'."

**🤖 AI Agent:**
> Timesheet orchestrated! For the task 'API Design', I've identified 5 recent high-fidelity time entries, totaling 12 hours. I've retrieved the technical logs and duration for your review. Need help summarizing the productivity?

---

**👤 You:**
> "Check the connectivity status for the 'Marketing' workspace."

**🤖 AI Agent:**
> Workspace directory orchestrated! The 'Marketing' workspace is currently 'ACTIVE' and fully synchronized with Microsoft 365. Your API connection is healthy. Shall I retrieve the detailed resource utilization metadata for this workspace?


## ❓ FAQ

**Q: How do I find my timeghost API Token?**
Log in to your account, navigate to **Settings** > **API Keys**, and generate a new high-fidelity **API Token**.

**Q: Can I check project budgets via AI?**
Yes! The `get_timeghost_project` tool allows your agent to retrieve high-fidelity budget metadata and financial health data for any specific project.

**Q: How do I list my workspace members?**
Use the `list_timeghost_users` tool to retrieve the complete high-fidelity directory of members along with their unique identifiers for precise orchestration.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/timeghost](https://vinkius.com/mcp/timeghost)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **timeghost** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `timeghost` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **timeghost** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "timeghost": {
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
