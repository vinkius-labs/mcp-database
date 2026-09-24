# Team Roster Count MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/team-roster-count)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Track and manage player statuses including active, reserve, and absent counts.

## Description
This MCP server provides real-time management of sports team rosters. It allows AI agents to monitor player availability and maintain roster integrity by tracking three distinct statuses: Active, Reserve, and Absent. Use `get_roster_summary` to see the full breakdown of a team, `get_player_status` to check an individual, `update_player_status` to modify availability, or `list_players_by_status` to filter players by their current role.


## Available Tools (4)
- **get_roster_summary**: Get a summary of the team roster counts
- **list_players_by_status**: List all players with a specific status
- **update_player_status**: Update a player's status
- **get_player_status**: Get the status and name of a specific player


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Team Roster Count** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is the current breakdown of my team (ID: team-123)?"

**🤖 AI Agent:**
> The team (team-123) has 15 active players, 3 reserve players, and 2 absent players, for a total of 20 players.

---

**👤 You:**
> "What is the status of player 'p-99' in team 'team-123'?"

**🤖 AI Agent:**
> Player p-99 (John Doe) is currently in Reserve status.

---

**👤 You:**
> "Set player 'p-45' in team 'team-123' to Active."

**🤖 AI Agent:**
> The status for player p-45 (Jane Smith) has been successfully updated to Active.


## ❓ FAQ

**Q: How can I see the total number of players in a team?**
You can use the `get_roster_summary` tool to retrieve the total count along with the breakdown of active, reserve, and absent players.

**Q: Can I change a player's status?**
Yes, use the `update_player_status` tool to change a player's status to Active, Reserve, or Absent.

**Q: How do I find all players who are currently absent?**
You can use the `list_players_by_status` tool and set the status filter to 'Absent'.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/team-roster-count](https://vinkius.com/en/ai-agent-connect/team-roster-count)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Team Roster Count** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `team-roster-count` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Team Roster Count** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "team-roster-count": {
      "url": "https://edge.vinkius.com/[TOKEN]/mcp"
    }
  }
}
```

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius connector registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
