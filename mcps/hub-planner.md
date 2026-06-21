# Hub Planner MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/hub-planner)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Manage resources, projects, and bookings via Hub Planner API.

## Description
Connect your AI agents to Hub Planner to optimize your resource management. This MCP server allows you to list resources, track project progress, manage bookings, and view client information directly through the Hub Planner API. Ideal for project managers and operations teams.


## Available Tools
- **get_me**: Gets current authenticated user info
- **list_bookings**: Lists resource bookings
- **list_categories**: Lists booking categories
- **list_clients**: Lists all clients
- **list_events**: Lists events/time-off
- **list_projects**: Lists all projects
- **list_resources**: Lists resources (people, equipment)
- **list_tags**: Lists tags used in projects and resources
- **list_teams**: Lists all teams
- **list_unassigned**: Lists unassigned bookings


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Hub Planner** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all resources in Hub Planner."

**🤖 AI Agent:**
> I'll fetch the list of your team members and resources.

---

**👤 You:**
> "Show me active projects."

**🤖 AI Agent:**
> I'll retrieve your active project list.

---

**👤 You:**
> "Check bookings for the next 7 days."

**🤖 AI Agent:**
> I'll look up the resource bookings for you.


## ❓ FAQ

**Q: Where do I find my Hub Planner API Key?**
Log in as Administrator, go to Settings > Integrations > API, and enable the API to generate your key.

**Q: Should I use 'Bearer' in the Authorization header?**
No, Hub Planner requires the raw API key without any prefix in the Authorization header.

**Q: Can I see resource availability?**
Yes, the list_resources and list_bookings tools help you understand resource allocation and availability.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/hub-planner](https://vinkius.com/mcp/hub-planner)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Hub Planner** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `hub-planner` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Hub Planner** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "hub-planner": {
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
