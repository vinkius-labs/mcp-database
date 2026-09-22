# Board Game Player Count MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/board-game-player-count)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [gaming](../categories/gaming.md)

Monitor player occupancy and table capacity across all game sessions.

## Description
This MCP server provides real-time insights into board game table occupancy. It allows AI agents to track total player headcounts, analyze table distribution (full, partial, or empty), check specific table details like remaining seats, and calculate the overall attendance rate across the gaming area. Use `get_total_player_count` to see how many people are playing, `get_table_occupancy_status` to check table availability, `get_table_details` for specific table capacity, and `get_aggregate_attendance_rate` to monitor venue utilization.


## Available Tools (4)
- **get_table_details**: Answers specific questions about the capacity and current state of a single table
- **get_table_occupancy_status**: Answers how many tables are currently full, partially full, or empty
- **get_total_player_count**: Answers how many people are playing games in total across all tables
- **get_aggregate_attendance_rate**: Answers what percentage of total game capacity is currently being used


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Board Game Player Count** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "How many players are currently at the game tables?"

**🤖 AI Agent:**
> There are currently 24 players participating in games across all tables.

---

**👤 You:**
> "Is table T-101 full?"

**🤖 AI Agent:**
> Table T-101 has 4 players and a maximum capacity of 6, so there are 2 seats remaining.

---

**👤 You:**
> "What is the current attendance rate for the gaming area?"

**🤖 AI Agent:**
> The current attendance rate is 75%.


## ❓ FAQ

**Q: How can I see how many people are playing games right now?**
You can use the `get_total_player_count` tool to get the total number of players across all tables.

**Q: Can I check if a specific table has any available seats?**
Yes, use the `get_table_details` tool with the specific table ID to see the current occupancy and remaining seats.

**Q: How do I know how many tables are currently empty?**
The `get_table_occupancy_status` tool provides a breakdown of empty, partial, and full tables.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/board-game-player-count](https://vinkius.com/en/ai-agent-connect/board-game-player-count)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Board Game Player Count** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `board-game-player-count` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Board Game Player Count** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "board-game-player-count": {
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
