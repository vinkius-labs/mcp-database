# Pointagram MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/pointagram)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Motivate your sales team with gamified leaderboards, competitions, and rewards that turn KPIs into engaging daily challenges.

## Description
Connect your **Pointagram** account to any AI agent to streamline your team gamification and engagement workflows. Pointagram provides a powerful platform for programmatically managing players, teams, and score series through its robust v2.0 REST API.

### What you can do

- **Player Orchestration** — List and create player profiles with detailed tracking of levels, nicknames, and avatars
- **Scoring Event Automation** — Post real-time scoring events to update player points across different score series programmatically
- **Team Management** — Access and monitor your gamification teams and retrieve detailed membership metadata
- **Score Series Discovery** — List all your active score series to understand how points are accumulated and distributed
- **Performance Intelligence** — Retrieve granular player stats and rankings using natural language commands

### How it works

1. Subscribe to this server
2. Enter your Pointagram API Key and API User (email) from your dashboard settings
3. Start managing your gamification data from Claude, Cursor, or any MCP client

### Who is this for?

- **Sales Managers & HR** — monitor team performance and trigger gamified rewards using natural language
- **Engagement Specialists** — automate the recognition of employee achievements more efficiently
- **Developers** — integrate real-time gamification data and player stats into custom business dashboards


## Available Tools (6)
- **create_player**: Pass data as a JSON string.

Create a new player
- **get_player_stats**: Get stats for a player
- **list_players**: List all Pointagram players
- **list_score_series**: List all score series
- **list_teams**: List all Pointagram teams
- **post_event**: Pass data as a JSON string.

Post a scoring event


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Pointagram** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all active players in Pointagram."

**🤖 AI Agent:**
> I've retrieved your player list. You have 50 active participants, including 'John Doe' (Level 12) and 'Maria Garcia' (Level 15). Would you like to see the stats for any of them?

---

**👤 You:**
> "Post 100 points for player '123' in the 'Sales Bonus' series."

**🤖 AI Agent:**
> Points posted successfully! I've added 100 points to player '123' in the 'Sales Bonus' series. The leaderboard will be updated shortly.

---

**👤 You:**
> "Show me the top 5 score series."

**🤖 AI Agent:**
> I've retrieved your score series. Your top active series include 'Monthly Sales Target', 'Customer Support Excellence', and 'Bug Squashing Challenge'. Which one would you like to explore?


## ❓ FAQ

**Q: How do I get my Pointagram API credentials?**
Log in to your Pointagram account, navigate to the **Settings** or **API** section, and you will find your Api-Key. Your Api-User is your login email.

**Q: Can I update points programmatically?**
Yes, the `post_event` tool allows you to send new scoring activities for any player, which will automatically update their score in the corresponding series.

**Q: Does it support team stats?**
Absolutely. You can use the `list_teams` tool to view all teams and their members, and use individual player tools to build aggregate team views.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/pointagram](https://vinkius.com/mcp/pointagram)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Pointagram** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `pointagram` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Pointagram** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "pointagram": {
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
