# Team Form Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/team-form-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [analytics](../categories/analytics.md)

Quantify football team performance trends using recent match windows.

## Description
Analyze football momentum with precision. This MCP allows AI agents to calculate a team's recent form by processing a specific window of recent match results. Use `get_team_form_summary` to retrieve points, goal differences, and unbeaten streaks, or `get_comparative_form_ranking` to rank multiple teams by their current momentum. You can also use `get_match_sequence_details` for specific scoring histories and `get_split_performance_analysis` to evaluate home vs away performance.


## Available Tools (4)
- **get_comparative_form_ranking**: Which teams in a specific group/league have the best momentum right now?
- **get_match_sequence_details**: What were the specific scoring details of a team's recent run?
- **get_split_performance_analysis**: Is this team's form driven by home advantage or away resilience?
- **get_team_form_summary**: How has this team performed over their last N matches?


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Team Form Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "How has Arsenal performed in their last 5 matches?"

**🤖 AI Agent:**
> Arsenal has a form score of 13 from their last 5 matches, with a result sequence of W, W, D, W, W. They have scored 12 goals and conceded 2, resulting in a goal difference of +10.

---

**👤 You:**
> "Which of these teams has the best momentum: Man City, Liverpool, or Chelsea, looking at the last 3 games?"

**🤖 AI Agent:**
> Based on the last 3 matches, Man City has the best momentum with a form score of 9.

---

**👤 You:**
> "Show me the scoring details for Real Madrid's last 3 matches."

**🤖 AI Agent:**
> In their last 3 matches, Real Madrid won 2-1 against Atletico, drew 1-1 against Valencia, and won 3-0 against Osasuna.


## ❓ FAQ

**Q: How is the form score calculated?**
The form score is based on the selected weighting scheme. If no weighting is applied, it is the sum of points (3 for a win, 1 for a draw) within the specified match window.

**Q: Can I compare multiple teams at once?**
Yes, you can use the ranking tool to compare a list of teams and see who has the best momentum based on their recent results.

**Q: What happens if two teams have the same form score?**
Ties are broken deterministically using goal difference, followed by the number of wins in the window.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/team-form-calculator](https://vinkius.com/en/ai-agent-connect/team-form-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Team Form Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `team-form-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Team Form Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "team-form-calculator": {
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
