# Ideanote MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/ideanote)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Manage ideas, missions, and innovation workspaces via Ideanote API.

## Description
Empower your AI agents to manage your innovation pipeline with Ideanote. This MCP server allows you to list submitted ideas, track innovation missions, manage workspaces, and view user engagement directly through the Ideanote API. Ideal for automating idea management and fostering a culture of innovation.


## Available Tools (10)
- **list_teams**: Lists all teams
- **list_users**: Lists all users in the workspace
- **list_webhooks**: Lists all configured webhooks
- **list_workspaces**: Lists all workspaces
- **get_idea**: Retrieves details for a specific idea
- **get_me**: Gets current authenticated user info
- **get_mission**: Retrieves details for a specific mission
- **list_ideas**: Lists all ideas
- **list_missions**: Lists all missions
- **list_phases**: Lists idea phases


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Ideanote** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List the top ideas from the current innovation mission."

**🤖 AI Agent:**
> I'll fetch the ideas submitted for your active missions.

---

**👤 You:**
> "Show me details for idea ID 'idea-789'."

**🤖 AI Agent:**
> I'll retrieve the full details and engagement metrics for that idea.

---

**👤 You:**
> "Check for any new innovation missions."

**🤖 AI Agent:**
> I'll look up the list of available missions in your workspace.


## ❓ FAQ

**Q: How do I get Ideanote API credentials?**
You can generate an API key in your Ideanote workspace under Settings > Integrations > API. Ensure you have administrator permissions.

**Q: Can I see all submitted ideas?**
Yes, the list_ideas tool provides access to all ideas submitted across your missions and workspaces.

**Q: Are innovation missions supported?**
Yes, you can list and retrieve details for innovation missions using the list_missions and get_mission tools.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/ideanote](https://vinkius.com/mcp/ideanote)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Ideanote** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `ideanote` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Ideanote** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "ideanote": {
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
