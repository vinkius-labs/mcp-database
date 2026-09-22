# Board Game Session Tracker MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/board-game-session-tracker)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Track and aggregate total time spent playing board games.

## Description
This MCP server allows AI agents to manage board game session data. You can record new play sessions using `add_game_session`, calculate the total time spent on a specific game with `get_total_game_time`, view a summary of all games via `get_all_game_totals`, or find the average session length for a game using `get_average_session_length`.


## Available Tools (4)
- **get_all_game_totals**: 
- **get_average_session_length**: 
- **get_total_game_time**: 
- **add_game_session**: 


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Board Game Session Tracker** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "I just finished playing Catan for 90 minutes. Please record this session."

**🤖 AI Agent:**
> Session recorded successfully. You have now played Catan for a total of 90 minutes.

---

**👤 You:**
> "How much total time have I spent playing Pandemic?"

**🤖 AI Agent:**
> You have spent a total of 120 minutes playing Pandemic.

---

**👤 You:**
> "What is the average session length for Terraforming Mars?"

**🤖 AI Agent:**
> The average session length for Terraforming Mars is 115 minutes.


## ❓ FAQ

**Q: How do I record a new game session?**
Use the `add_game_session` tool by providing the name of the game and the duration in minutes.

**Q: Can I see how much time I've spent on all my games?**
Yes, you can use `get_all_game_totals` to get a summary of every game recorded in the system.

**Q: How do I find the average length of a game session?**
You can use the `get_average_session_length` tool for a specific game name.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/board-game-session-tracker](https://vinkius.com/en/ai-agent-connect/board-game-session-tracker)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Board Game Session Tracker** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `board-game-session-tracker` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Board Game Session Tracker** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "board-game-session-tracker": {
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
