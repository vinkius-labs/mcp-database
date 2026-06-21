# Mela MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/mela)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [communication-messaging](../categories/communication-messaging.md)

Team communication and project management.

## Description
The Mela MCP server connects your AI agent directly to your workspace. Send channel messages, query project status, and summarize daily team updates without ever leaving your editor.


## Available Tools (12)
- **create_activity**: Create a new job site or activity
- **get_accounting_data**: Retrieve cost and accounting data for an activity
- **get_activity**: Retrieve details for a specific activity
- **get_me**: Retrieve information about the current user
- **list_activities**: List all job sites/activities
- **list_checklists**: Retrieve all checklists associated with an activity
- **list_teams**: List teams in the workspace
- **list_users**: List all workspace members
- **log_materials**: Track material consumption on-site
- **log_work_hours**: Record man-hours for an activity
- **post_message**: Send a text update or note to an activity feed
- **update_activity_status**: Change the status of an activity


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Mela** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Send an update to the 'Engineering' channel saying the build is fixed."

**🤖 AI Agent:**
> Message posted successfully to the 'Engineering' channel.

---

**👤 You:**
> "Summarize the latest tasks completed in Project Alpha."

**🤖 AI Agent:**
> In Project Alpha, 3 tasks were completed today: 'DB Migration', 'Fix CSS on mobile', and 'Update README'.

---

**👤 You:**
> "List all team members currently online."

**🤖 AI Agent:**
> Currently online: Sarah, Marcus, John, and Elena.


## ❓ FAQ

**Q: Can the AI send messages to a specific channel?**
Yes, just mention the channel name or ID, and the AI will post the message directly on your behalf.

**Q: How do I fetch the latest updates from my team?**
You can ask the agent to summarize recent activity in a specific project or channel.

**Q: Does it support reading project task boards?**
Yes, the agent can list tasks, check assignees, and verify current statuses in your Mela projects.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/mela](https://vinkius.com/mcp/mela)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Mela** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `mela` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Mela** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "mela": {
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
