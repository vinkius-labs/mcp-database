# COR MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/cor)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Optimize creative agency profitability with project tracking, resource allocation, and real-time margin analysis for every job.

## Description
Connect your **COR** account to any AI agent and take full control of your professional services project management and profitability orchestration through natural conversation.

### What you can do

- **Project Portfolio Orchestration** — List all active projects, retrieve detailed high-fidelity status metadata, and access profitability metrics programmatically
- **Task Pipeline Intelligence** — Query tasks for any project, retrieve detailed technical metadata, and stay on top of your team's operational delivery in real-time
- **Profitability Monitoring** — Access high-fidelity financial insights and project health metrics to ensure sustainable growth directly through your agent
- **Time Tracking Discovery** — Access recorded technical time entries to understand workload distribution and project efficiency across your organization
- **Resource Architecture** — List team members, teams, and user profiles to understand and orchestrate your organizational structure programmatically
- **Client Database Access** — Query the complete high-fidelity directory of client organizations to maintain perfect contextual alignment for every project

### How it works

1. Subscribe to this server
2. Retrieve your **Personal API Token** from your COR account (Settings > API Tokens)
3. Start managing your professional services growth from Claude, Cursor, or any MCP client

No more manual status updates or missing profitability gaps. Your AI acts as your dedicated project coordinator and profitability architect.

### Who is this for?

- **Project Managers** — instantly retrieve task lists and project statuses using natural language commands without leaving your creative workspace
- **Agency Leads** — monitor high-fidelity profitability metrics and team utilization to ensure healthy business operations
- **Operations Managers** — verify technical time logs and team assignments to optimize resource allocation through simple AI queries


## Available Tools (13)
- **list_cor_clients**: List customer clients
- **create_cor_project**: Create a new project
- **get_cor_project**: Get details for a specific project
- **get_cor_task**: Get details for a specific task
- **get_cor_me**: Get current user details
- **list_cor_projects**: List COR projects
- **check_cor_status**: Check API Status
- **list_cor_task_types**: List defined task types
- **list_cor_tasks**: Optionally filter by project ID to isolate specific technical pipelines.

List tasks
- **list_cor_team_users**: List users in a team
- **list_cor_teams**: List organization teams
- **list_cor_time_entries**: List recorded time entries
- **list_cor_team_members**: List team users


## 💬 Prompt Examples

Here are some examples of how you can interact with the **COR** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all active projects and show their status."

**🤖 AI Agent:**
> I've retrieved your projects. You currently have 12 active high-fidelity projects, including 'Website Redesign' (In Progress) and 'Mobile App Launch' (Planning). Would you like to see the profitability metrics for any of them?

---

**👤 You:**
> "Show tasks assigned to project 'COR Integration'."

**🤖 AI Agent:**
> Pipeline orchestrated! For the project 'COR Integration', I've identified 8 active high-fidelity tasks, including 'API Mapping' and 'Presenter Logic'. I've retrieved the current status and assignee for each. Shall I summarize the progress?

---

**👤 You:**
> "Check the team members in the 'Development' team."

**🤖 AI Agent:**
> Team directory orchestrated! The 'Development' team currently has 5 high-fidelity profiles, including 'Alex' (Dev Lead) and 'Sarah' (Senior FE). Your API connection is healthy. Shall I retrieve the detailed time log metadata for this team?


## ❓ FAQ

**Q: How do I find my COR API Token?**
Log in to your account, navigate to **Personal Settings** > **API Tokens**, and generate a new high-fidelity **Personal API Token**.

**Q: Can I check project profitability via AI?**
Yes! The `get_cor_project` tool allows your agent to retrieve high-fidelity profitability metrics and financial health data for any specific project.

**Q: How do I list my organization's teams?**
Use the `list_cor_teams` tool to retrieve the complete high-fidelity directory of teams along with their unique identifiers for precise orchestration.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/cor](https://vinkius.com/mcp/cor)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **COR** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `cor` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **COR** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "cor": {
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
