# Head-to-Head Record Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/head-to-head-record-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [statistics](../categories/statistics.md)

Calculate precise historical football performance metrics and H2H records between teams.

## Description
This MCP server provides a precision engine for analyzing historical football performance. It allows AI agents to retrieve detailed head-to-head statistics, including wins, draws, losses, goals, and points. Using `query_h2h_summary`, you can get a complete statistical overview of team matchups. For granular details, `query_match_history` provides individual match results, while `query_team_comparison_efficiency` calculates dominance through win percentages and scoring rates. You can also use `query_competition_breakdown` to see how records are distributed across different leagues. All calculations strictly follow professional football standards, such as excluding penalty shootout goals from total goal counts.


## Available Tools (4)
- **query_competition_breakdown**: Shows how the H2H record is distributed across different competitions
- **query_h2h_summary**: Provides a statistical overview of how specific teams have performed against each other
- **query_match_history**: Retrieves individual match details used to generate the H2H record
- **query_team_comparison_efficiency**: Calculates efficiency ratios to show how dominant one team is over another


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Head-to-Head Record Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is the head-to-head record between Team A and Team B?"

**🤖 AI Agent:**
> In their historical matchups, Team A has 3 wins, Team B has 1 win, and they have had 2 draws. Team A has scored 8 goals while Team B has scored 4 goals.

---

**👤 You:**
> "Show me the match history between these two teams in the Premier League."

**🤖 AI Agent:**
> The matches in the Premier League between these teams are: 2023-05-12 (2-1), 2022-11-05 (1-1), and 2021-08-20 (0-2).

---

**👤 You:**
> "How dominant is Team A compared to Team B?"

**🤖 AI Agent:**
> Team A has a 60% win percentage, an average goal scoring rate of 1.5 goals per match, and a clean sheet rate of 33% against Team B.


## ❓ FAQ

**Q: How are penalty shootouts handled in the statistics?**
Goals scored during penalty shootouts are excluded from the 'Goals For' and 'Goals Against' totals. The match result is recorded based on regulation time, but the shootout winner is used to determine the final win/loss and points.

**Q: Can I filter matches by a specific competition?**
Yes, you can use the `competitionId` filter in tools like `query_h2h_summary` or `query_match_history` to restrict results to a specific league or tournament.

**Q: How are points calculated for team comparisons?**
The engine uses the standard competitive scoring system: 3 points for a win, 1 point for a draw, and 0 points for a loss.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/head-to-head-record-calculator](https://vinkius.com/en/ai-agent-connect/head-to-head-record-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Head-to-Head Record Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `head-to-head-record-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Head-to-Head Record Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "head-to-head-record-calculator": {
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
