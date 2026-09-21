# Goal Difference Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/goal-difference-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [analytics](../categories/analytics.md)

Calculate football performance metrics like goal difference, clean sheets, and scoring efficiency.

## Description
This MCP server provides deep analytical insights into football team performance. Use `get_team_performance` to retrieve comprehensive stats including goal difference, goals for, goals against, and shutout rates. You can also use `get_match_history` to see a detailed list of past matches, `get_scoring_efficiency` to find average goals per game, or `validate_team_existence` to confirm a team is in the database.


## Available Tools (4)
- **validate_team_existence**: Verify if a team name is recognized by the system
- **get_match_history**: Retrieve a list of all matches played by a specific team within a specified context
- **get_scoring_efficiency**: Calculate how many goals the team scores relative to the number of matches played
- **get_team_performance**: Calculate comprehensive performance metrics for a team based on specific viewing constraints


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Goal Difference Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is the goal difference for Arsenal in their home matches?"

**🤖 AI Agent:**
> Arsenal has a goal difference of +12 in their home matches.

---

**👤 You:**
> "Show me the match history for Manchester City."

**🤖 AI Agent:**
> Manchester City's recent matches include a 3-0 win against Chelsea, a 1-1 draw with Liverpool, and a 2-0 victory over Everton.

---

**👤 You:**
> "What is the scoring efficiency for Real Madrid?"

**🤖 AI Agent:**
> Real Madrid has a scoring efficiency of 2.45 goals per match.


## ❓ FAQ

**Q: How can I see a team's defensive performance?**
Use the `get_team_performance` tool. It provides clean sheets and shutout rates to help you evaluate defensive solidity.

**Q: Can I filter results by venue?**
Yes, most tools allow you to specify a `viewType` such as 'home', 'away', or 'combined' to filter the match data.

**Q: How do I check if a specific team is available?**
You can use the `validate_team_existence` tool to verify if a team name is recognized in the system.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/goal-difference-calculator](https://vinkius.com/en/ai-agent-connect/goal-difference-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Goal Difference Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `goal-difference-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Goal Difference Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "goal-difference-calculator": {
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
