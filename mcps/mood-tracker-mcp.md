# Mood Tracker MCP MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/mood-tracker-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Analyze daily mood logs to identify emotional trends and weekly patterns.

## Description
The Mood Tracker MCP connects AI agents to your longitudinal mood data. Use `get_weekly_summary` to track if your emotional state is improving or declining over time. You can use `identify_difficulty_peaks` to pinpoint specific dates with low scores and `analyze_weekday_patterns` to discover if certain days of the week consistently impact your well-being.


## Available Tools
- **identify_difficulty_peaks**: Identify days with particularly low mood scores
- **analyze_weekday_patterns**: Analyze patterns by day of the week
- **get_weekly_summary**: Get a summary of the mood for a specific week


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Mood Tracker MCP** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What was my overall mood this week and is it improving?"

**🤖 AI Agent:**
> The `get_weekly_summary` tool would return the average score, total entries, and whether your trend is improving, declining, or stable for the requested week.

---

**👤 You:**
> "Which days have been hard for me in the last 10 days?"

**🤖 AI Agent:**
> The `identify_difficulty_peaks` tool would return a list of dates where your mood score fell below the threshold during that 10-day period.

---

**👤 You:**
> "Do I have any patterns on certain weekdays?"

**🤖 AI Agent:**
> The `analyze_weekday_patterns` tool would provide the average scores for each day of the week and identify your most positive and negative days.


## ❓ FAQ

**Q: How does the weekly summary work?**
The `get_weekly_summary` tool calculates your average mood score for a specific week and compares it to the previous week to determine if your trend is improving, declining, or stable.

**Q: Can I identify my most difficult days?**
Yes, by using the `identify_difficulty_peaks` tool, you can specify a lookback period and a threshold to find dates where your mood score was particularly low.

**Q: Does it show patterns for specific days?**
Yes, the `analyze_weekday_patterns` tool aggregates your historical data to reveal which days of the week (like Mondays or Fridays) typically correlate with higher or lower emotional states.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/mood-tracker-mcp](https://vinkius.com/mcp/mood-tracker-mcp)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Mood Tracker MCP** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `mood-tracker-mcp` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Mood Tracker MCP** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "mood-tracker-mcp": {
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
