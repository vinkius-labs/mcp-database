# Habit Completion Rate MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/habit-completion-rate)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Track habit adherence and streaks with precise completion metrics.

## Description
This MCP server provides tools to monitor habit discipline and consistency. Use `get_habit_completion_rate` to calculate success percentages, `get_habit_streak_info` to track consecutive days, `get_habit_consistency_trend` to analyze performance shifts, and `validate_habit_schedule` to ensure your planned routines are logically sound.


## Available Tools (4)
- **get_habit_completion_rate**: Calculates the percentage of successful habit completions against planned commitments
- **get_habit_consistency_trend**: Provides a comparison of completion rates across different time segments
- **get_habit_streak_info**: Determines the current consecutive success streak and the longest historical streak for a habit
- **validate_habit_schedule**: Checks for logical inconsistencies in a user's planned habit schedule


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Habit Completion Rate** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is my completion rate for habit 'water-intake' from 2024-01-01 to 2024-01-07?"

**🤖 AI Agent:**
> Your completion rate for water-intake is 85.7% (6 out of 7 planned days).

---

**👤 You:**
> "What is my current streak for 'daily-meditation'?"

**🤖 AI Agent:**
> Your current streak for daily-meditation is 12 days.

---

**👤 You:**
> "Is my habit schedule for 'gym' between 2024-05-01 and 2024-05-05 valid?"

**🤖 AI Agent:**
> Yes, your schedule for gym is valid.


## ❓ FAQ

**Q: How is the completion rate calculated?**
The rate is the number of completed days divided by the number of planned days for the selected period.

**Q: Can I check my current streak?**
Yes, you can use `get_habit_streak_info` to see your current consecutive success streak and your historical record.

**Q: How do I know if my habit schedule is valid?**
You can use `validate_habit_schedule` to check for logical errors or impossible frequencies in your planned routine.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/habit-completion-rate](https://vinkius.com/en/ai-agent-connect/habit-completion-rate)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Habit Completion Rate** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `habit-completion-rate` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Habit Completion Rate** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "habit-completion-rate": {
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
