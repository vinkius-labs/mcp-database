# Promotion & Relegation Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/promotion-relegation-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [data-analysis](../categories/data-analysis.md)

Analyze football league standings to determine promotion, playoff, safety, and relegation status.

## Description
This MCP server provides professional-grade tools for analyzing football league standings. It allows AI agents to calculate the exact status of every team, identify critical boundary teams sitting on the edge of promotion or relegation, and simulate how specific point changes or tiebreak adjustments will impact the league table. Use `calculate_status` to get a full league overview, `get_boundary_analysis` to find the points gap between status zones, and `simulate_status_change` to predict future outcomes.


## Available Tools (4)
- **calculate_status**: Determines the final status for every team in the league based on current standings and defined thresholds
- **filter_teams_by_status**: Retrieves a subset of teams that fall into a specific status category
- **get_boundary_analysis**: Identifies the teams sitting on the edge of status changes and calculates the distance to a different status
- **simulate_status_change**: Predicts how a specific change in a team's performance would impact their status and the status of others


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Promotion & Relegation Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Calculate the status for these teams: Team A (10 pts, 5 GD), Team B (10 pts, 2 GD), Team C (5 pts, 0 GD). Thresholds: 1 promotion, 1 relegation. Tiebreak: GD."

**🤖 AI Agent:**
> Team A is in the automatic promotion position, Team B is in the safety zone, and Team C is in the relegation zone.

---

**👤 You:**
> "Who is at the boundary between safety and relegation for this league?"

**🤖 AI Agent:**
> The boundary is between Team X (15 pts) and Team Y (14 pts). Team Y needs 1 more point to reach the safety zone.

---

**👤 You:**
> "What happens to the league if Team Alpha gains 3 points?"

**🤖 AI Agent:**
> Team Alpha will move from the playoff position to the automatic promotion position, and Team Beta will drop from the last promotion spot to the playoff zone.


## ❓ FAQ

**Q: How does the tool handle tiebreaks?**
You can specify a `tiebreakOrder` in the tool inputs. The engine will use these metrics in the provided order to rank teams with equal points.

**Q: Can I predict what happens if a team wins their next match?**
Yes, use the `simulate_status_change` tool to apply a points adjustment to a specific team and see how it affects their rank and the status of others.

**Q: What information is needed to calculate league status?**
You need the current standings (JSON), the threshold counts for each status (JSON), and the list of tiebreak metrics (JSON array).


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/promotion-relegation-calculator](https://vinkius.com/en/ai-agent-connect/promotion-relegation-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Promotion & Relegation Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `promotion-relegation-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Promotion & Relegation Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "promotion-relegation-calculator": {
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
