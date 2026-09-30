# Game Night Planner MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/game-night-planner)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Orchestrate perfect game nights by planning schedules, teams, snacks, and shared costs.

## Description
The Game Night Planner connects your AI assistant to the logistics of your social gatherings. Use `plan_games` to create a timed schedule for your favorite titles, `organize_players_and_teams` to balance competition, `manage_snacks` to track food logistics, and `calculate_shared_costs` to ensure everyone pays their fair share. It handles everything from game duration to expense splitting.


## Available Tools (4)
- **organize_players_and_teams**: Manages the list of attendees and creates balanced teams for specific game rounds
- **plan_games**: Schedules the sequence of games and rounds to ensure the night fits within the desired timeframe
- **calculate_shared_costs**: Calculates the total expenditure and the individual split for all participants
- **manage_snacks**: Tracks the food and beverage requirements for the event


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Game Night Planner** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Plan a game night with Catan and Uno. We want 2 rounds each, 30 minutes per round, with 5 minutes between rounds."

**🤖 AI Agent:**
> Your game night schedule is ready: Catan will have two 30-minute rounds, and Uno will have two 30-minute rounds, with a total duration of 130 minutes including buffer time.

---

**👤 You:**
> "We have 6 players. Can you split them into teams of 3?"

**🤖 AI Agent:**
> I have organized your 6 players into 2 teams of 3 members each.

---

**👤 You:**
> "Calculate the costs: we spent 50 on pizza and 20 on drinks. There are 4 people."

**🤖 AI Agent:**
> The total spent is 70, which means each of the 4 participants owes 17.50.


## ❓ FAQ

**Q: How do I schedule my games?**
You can use the `plan_games` tool to define your game list, the number of rounds, and the duration per round to get a complete schedule.

**Q: Can I split the bill with my friends?**
Yes, the `calculate_shared_costs` tool calculates the total spent and the exact amount each participant owes.

**Q: How are teams created?**
The `organize_players_and_teams` tool takes your list of attendees and groups them into balanced teams based on your preferred team size.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/game-night-planner](https://vinkius.com/en/ai-agent-connect/game-night-planner)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Game Night Planner** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `game-night-planner` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Game Night Planner** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "game-night-planner": {
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
