# Match Statistics Aggregator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/match-statistics-aggregator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [statistics](../categories/statistics.md)

Aggregate football performance metrics for teams and players.

## Description
This MCP server provides deep statistical insights into football performance. It allows AI agents to calculate totals, averages, medians, and per-90 rates for any metric. Use `aggregate_team_stats` to analyze team performance, `aggregate_player_stats` for individual player metrics, `rank_entities` to find top performers, and `compare_periods` to track performance changes over time.


## Available Tools (4)
- **aggregate_player_stats**: Aggregates individual performance metrics for a specific player
- **aggregate_team_stats**: Aggregates statistics for a specific team over a given period or competition
- **compare_periods**: Compares performance between two different timeframes for an entity
- **rank_entities**: Ranks entities based on a specific metric


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Match Statistics Aggregator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What were the total goals and average shots for Manchester City this season?"

**🤖 AI Agent:**
> Manchester City has scored 72 goals and averaged 14.5 shots per match this season.

---

**👤 You:**
> "Who are the top 5 goal scorers in the Premier League right now?"

**🤖 AI Agent:**
> The top 5 goal scorers in the Premier League are Erling Haaland (18), Mohamed Salah (14), Ollie Watkins (13), Son Heung-min (12), and Alexander Isak (12).

---

**👤 You:**
> "How has Kylian Mbappé's scoring rate changed between the first half and second half of the season?"

**🤖 AI Agent:**
> Kylian Mbappé's scoring rate increased by 12% in the second half of the season compared to the first.


## ❓ FAQ

**Q: How are per-90 rates calculated?**
Per-90 rates are calculated by dividing the total metric value by the total minutes played, then multiplying by 90.

**Q: Can I compare two different seasons?**
Yes, you can use `compare_periods` to see how performance changed between two specific timeframes.

**Q: How are ties handled in rankings?**
Rankings use a deterministic secondary sort key, which is the entity name in ascending alphabetical order.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/match-statistics-aggregator](https://vinkius.com/en/ai-agent-connect/match-statistics-aggregator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Match Statistics Aggregator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `match-statistics-aggregator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Match Statistics Aggregator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "match-statistics-aggregator": {
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
