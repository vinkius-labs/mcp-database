# Linear MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/linear-alternative)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [loved-by-devs](../categories/loved-by-devs.md)

Ship software faster with issue tracking built for modern teams that combines speed, keyboard shortcuts, and beautiful design.

## Description
Connect your **Linear** workspace to any AI agent and take full control of your agile software delivery and high-fidelity issue orchestration through natural conversation.

### What you can do

- **Issue Portfolio Orchestration** — List all active tickets, retrieve detailed high-fidelity metadata, and monitor delivery status programmatically
- **Agile Execution Intelligence** — Programmatically generate and update high-fidelity issues for specific teams directly through your agent
- **Project & Cycle Monitoring** — Access your complete directory of high-fidelity projects and active cycles to ensure perfectly coordinated development
- **Resource Architecture** — List team members and collaborators to understand and orchestrate your organizational structure programmatically
- **Communication Stream Access** — Programmatically add high-fidelity comments to specific issues to maintain perfect contextual alignment
- **Operational Monitoring** — Verify account-level API connectivity and monitor issue orchestration volume directly through your agent for perfectly coordinated service scaling

### How it works

1. Subscribe to this server
2. Retrieve your **Personal API Key** from your Linear account (Settings > API)
3. Start managing your agile growth from Claude, Cursor, or any MCP client

No more manual status updates or missing project gaps. Your AI acts as your dedicated project coordinator and agile architect.

### Who is this for?

- **Software Engineers** — instantly retrieve issue lists and update ticket statuses using natural language commands without leaving your creative workspace
- **Product Managers** — monitor high-fidelity project progress and team utilization to ensure healthy software delivery
- **DevOps Leads** — verify technical issue logs and team assignments to optimize resource allocation through simple AI queries


## Available Tools (11)
- **create_linear_comment**: Add a comment to an issue
- **create_linear_issue**: Create a new issue
- **get_linear_issue**: Get details for a specific issue
- **list_linear_cycles**: List active cycles
- **list_linear_issues**: List Linear issues
- **list_linear_labels**: List issue labels
- **list_linear_projects**: List active projects
- **list_linear_teams**: List workspace teams
- **list_linear_users**: List workspace members
- **check_linear_status**: Check API Status
- **update_linear_issue**: Update an existing issue


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Linear** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all active issues and show their status."

**🤖 AI Agent:**
> I've retrieved your issues. You currently have 15 active high-fidelity tickets, including 'API Integration' (In Progress) and 'UI Bug' (Backlog). Would you like to see the detailed metadata for any of them?

---

**👤 You:**
> "Create a new issue for the 'Frontend' team titled 'Implement Dashboard'."

**🤖 AI Agent:**
> Issue orchestrated! I've successfully created 'Implement Dashboard' (ID: FRONT-45) for the Frontend team. This high-fidelity update is now live in Linear. Shall I verify the team's current technical velocity?

---

**👤 You:**
> "Check the team members in the 'Mobile' team."

**🤖 AI Agent:**
> Team directory orchestrated! The 'Mobile' team currently has 8 high-fidelity profiles assigned. Your API connection is healthy. Shall I retrieve the detailed resource utilization metadata for this team?


## ❓ FAQ

**Q: How do I find my Linear Personal API Key?**
Log in to your account, navigate to **Settings** > **API**, and generate a new high-fidelity **Personal API Key**.

**Q: Can I check project progress via AI?**
Yes! The `get_linear_project` tool allows your agent to retrieve high-fidelity progress metrics and health data for any specific project.

**Q: How do I list my active cycles?**
Use the `list_linear_cycles` tool to retrieve the complete high-fidelity directory of cycles along with their technical status and progress metrics.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/linear-alternative](https://vinkius.com/mcp/linear-alternative)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Linear** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `linear-alternative` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Linear** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "linear-alternative": {
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
