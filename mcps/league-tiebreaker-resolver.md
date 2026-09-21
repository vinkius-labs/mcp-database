# League Tiebreaker Resolver MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/league-tiebreaker-resolver)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [utilities](../categories/utilities.md)

Resolves football league ties using a custom sequence of rules.

## Description
This MCP server provides a specialized engine for resolving deadlocks in football league standings. By using the `resolve_league_ties` tool, you can apply a specific hierarchy of rules--such as points, goal difference, or fair-play score--to a set of competing teams. The engine evaluates rules sequentially until a unique ranking is achieved or all rules are exhausted, in which case it defaults to a stable alphabetical order. It is designed to handle both performance-based metrics and disciplinary metrics like fair-play score.


## Available Tools (4)
- **get_tiebreaker_metadata**: Provides a reference of all valid rule names and their direction
- **identify_tie_group**: Identifies which teams are currently tied based on a specific metric
- **resolve_league_ties**: Resolves ties between a group of teams using a provided ordered list of tie-breaking rules
- **validate_team_data**: Ensures a set of team statistics is complete and logically consistent


## 💬 Prompt Examples

Here are some examples of how you can interact with the **League Tiebreaker Resolver** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Resolve the tie between Team A (10 pts, 5 GD) and Team B (10 pts, 3 GD) using goalDifference."

**🤖 AI Agent:**
> Team A: rank 1, separationRule: goalDifference; Team B: rank 2, separationRule: null.

---

**👤 You:**
> "Check if my team data is valid for the resolver."

**🤖 AI Agent:**
> The team data is valid and ready for tie-breaking.

---

**👤 You:**
> "Which teams are tied on points in this list: Team X (15 pts), Team Y (15 pts), Team Z (12 pts)?"

**🤖 AI Agent:**
> The tied teams are Team X and Team Y.


## ❓ FAQ

**Q: How do I know which rule separated the teams?**
The `resolve_league_ties` tool returns a `separationRule` field for each team, indicating exactly which rule was responsible for distinguishing that team from the next in the ranking.

**Q: Can I use fair-play score as a tiebreaker?**
Yes. The engine treats the fair-play score as an ascending metric, meaning a lower score is considered better during the tie-breaking process.

**Q: What happens if all tie-breaking rules are exhausted?**
If no rules can separate the teams, the engine provides a stable output by sorting the remaining tied teams alphabetically by their name.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/league-tiebreaker-resolver](https://vinkius.com/en/ai-agent-connect/league-tiebreaker-resolver)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **League Tiebreaker Resolver** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `league-tiebreaker-resolver` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **League Tiebreaker Resolver** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "league-tiebreaker-resolver": {
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
