# Nozbe MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/nozbe)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Task management and team productivity.

## Description
The Nozbe MCP server brings your team's task management directly to your AI agent. List projects, assign tasks, update priorities, and track team collaboration fluidly without navigating away from your chat interface.


## Available Tools (12)
- **create_project**: Create a new project
- **create_task**: Create a new task
- **delete_task**: Permanently remove a task
- **get_me**: Check API connectivity and get current user context
- **get_project**: Retrieve details for a specific project
- **get_task**: Retrieve details for a specific task
- **get_team**: Retrieve details for a specific team
- **list_comments**: Retrieve discussion comments for a task
- **list_tasks**: List all accessible tasks
- **list_teams**: List teams you have access to
- **update_task**: Edit a specific task
- **list_projects**: List all accessible projects


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Nozbe** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all my priority tasks for today."

**🤖 AI Agent:**
> You have 3 priority tasks: 'Finish quarterly report', 'Review marketing copy', and 'Email client'.

---

**👤 You:**
> "Create a task 'Update website banner' and assign it to Sarah."

**🤖 AI Agent:**
> Task 'Update website banner' created and successfully assigned to Sarah.

---

**👤 You:**
> "Mark task ID 5402 as completed."

**🤖 AI Agent:**
> Task 5402 has been marked as completed. Great job!


## ❓ FAQ

**Q: Can I retrieve all tasks from a specific project?**
Yes, just provide the project name or ID, and the agent will list all active and completed tasks within it.

**Q: How do I assign a task to a team member?**
You can tell the AI to create a task and mention the assignee, and the integration will route the task to them in Nozbe.

**Q: Is it possible to complete a task directly?**
Absolutely. By providing the task ID to the agent, you can mark it as completed instantly.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/nozbe](https://vinkius.com/mcp/nozbe)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Nozbe** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `nozbe` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Nozbe** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "nozbe": {
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
