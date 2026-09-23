# Habit Streak Analyzer MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/habit-streak-analyzer)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Calculate current and longest streaks from a list of completion dates.

## Description
This MCP server provides tools to analyze habit consistency. You can use `get_current_streak` to find the active streak, `get_longest_streak` to find the historical maximum, `get_streak_stats` for a full performance summary, and `verify_streak_continuity` to check if a specific date belongs to an unbroken sequence.


## Available Tools (4)
- **get_current_streak**: Determines the current consecutive streak of habit completion
- **get_longest_streak**: Finds the longest consecutive streak in the history
- **get_streak_stats**: Provides a comprehensive summary of habit performance
- **verify_streak_continuity**: Checks if a specific date is part of an ongoing unbroken streak


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Habit Streak Analyzer** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is my current streak for the dates 2023-10-01, 2023-10-02, and 2023-10-03?"

**🤖 AI Agent:**
> Your current streak is 3 days.

---

**👤 You:**
> "What was my longest streak given these dates: 2023-01-01, 2023-01-02, 2023-01-05, 2023-01-06, 2023-01-07?"

**🤖 AI Agent:**
> Your longest streak was 3 days.

---

**👤 You:**
> "Give me a full summary of my habit performance for 2023-11-01, 2023-11-02, 2023-11-04."

**🤖 AI Agent:**
> Current streak: 2, Longest streak: 2, Total days completed: 3, Streak break count: 1.


## ❓ FAQ

**Q: What format should the dates be in?**
All dates must be provided in ISO 8601 format (e.g., '2023-10-01').

**Q: How is a streak considered broken?**
A streak is broken if there is a gap of one or more full calendar days between two completion dates.

**Q: Can I see my total number of completed days?**
Yes, you can use `get_streak_stats` to retrieve the total number of unique days completed.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/habit-streak-analyzer](https://vinkius.com/en/ai-agent-connect/habit-streak-analyzer)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Habit Streak Analyzer** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `habit-streak-analyzer` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Habit Streak Analyzer** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "habit-streak-analyzer": {
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
