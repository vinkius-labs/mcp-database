# Healthy Habit Streak Plan MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/healthy-habit-streak-plan)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Generate structured habit schedules, tracking targets, and streak logic.

## Description
This MCP server provides a complete toolkit for managing habit formation. It allows AI agents to generate precise habit calendars using `get_habit_calendar`, predict future milestones with `generate_habit_targets`, and manage psychological safety through `calculate_streak_status` which accounts for allowed skips. Users can also ensure their settings are logically sound using `validate_habit_configuration` before committing to a plan.


## Available Tools (4)
- **calculate_streak_status**: Determines if a user's current streak is active, broken, or utilizing an allowed skip
- **generate_habit_targets**: Calculates the number of completions required to reach specific milestones
- **get_habit_calendar**: Generates a list of all specific dates a user is expected to perform a habit
- **validate_habit_configuration**: Checks if a user's habit settings are logically sound


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Healthy Habit Streak Plan** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Generate a daily habit calendar for 'Morning Meditation' starting from 2024-01-01 to 2024-01-31."

**🤖 AI Agent:**
> The scheduled dates for Morning Meditation are: 2024-01-01, 2024-01-02, 2024-01-03, 2024-01-04, 2024-01-05, 2024-01-06, 2024-01-07, 2024-01-08, 2024-01-09, 2024-01-10, 2024-01-11, 2024-01-12, 2024-01-13, 2024-01-14, 2024-01-15, 2024-01-16, 2024-01-17, 2024-01-18, 2024-01-19, 2024-01-20, 2024-01-21, 2024-01-22, 2024-01-23, 2024-01-24, 2024-01-25, 2024-01-26, 2024-01-27, 2024-01-28, 2024-01-29, 2024-01-30, 2024-01-31.

---

**👤 You:**
> "Check my streak for 'Running' if I completed it on 2024-05-01 and 2024-05-02, with 1 allowed skip, as of 2024-05-04."

**🤖 AI Agent:**
> Your current streak for Running is 'paused_by_skip' with a current streak count of 2 and 1 remaining skip.

---

**👤 You:**
> "When will I hit 10 completions for 'Reading' if I start on 2024-06-01 and read every 3 days?"

**🤖 AI Agent:**
> You are expected to reach your 10th completion on 2024-06-28.


## ❓ FAQ

**Q: How does the streak logic handle missed days?**
The `calculate_streak_status` tool uses an 'allowed skips' parameter. If you miss a day but have skips remaining, your streak is marked as 'paused_by_skip' instead of 'broken'.

**Q: Can I plan for specific days of the week?**
Yes, by using `get_habit_calendar` with the 'specific_days' frequency type, you can generate a schedule for any set of weekdays.

**Q: How do I know when I will reach my habit goals?**
You can use `generate_habit_targets` to provide a list of milestones, and the tool will return the estimated completion dates for each.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/healthy-habit-streak-plan](https://vinkius.com/en/ai-agent-connect/healthy-habit-streak-plan)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Healthy Habit Streak Plan** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `healthy-habit-streak-plan` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Healthy Habit Streak Plan** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "healthy-habit-streak-plan": {
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
