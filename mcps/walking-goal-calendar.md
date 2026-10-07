# Walking Goal Calendar MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/walking-goal-calendar)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Distributes weekly walking goals into a daily distance and time plan.

## Description
This MCP server helps you manage your fitness by distributing a weekly walking goal across your active days. It calculates daily distance and duration based on your chosen pace and ensures all activities fit within your available time windows. Use `calculate_weekly_schedule` to generate a full weekly plan, `validate_pace_safety` to check if your speed is realistic, `get_rest_day_summary` to track recovery, and `check_window_compliance` to ensure your walks fit your schedule.


## Available Tools (4)
- **calculate_weekly_schedule**: Generates a complete daily plan for a single week based on a goal and user preferences
- **validate_pace_safety**: Checks if a proposed walking pace is within realistic human limits
- **check_window_compliance**: Verifies that no walking activity is scheduled to exceed the allowed time constraints
- **get_rest_day_summary**: Calculates the total recovery time and verifies rest days


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Walking Goal Calendar** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "I want to walk 20km this week on Monday, Wednesday, and Friday. My pace is 5 km/h, and I have 60 minutes available each of those days. Can you make a plan?"

**🤖 AI Agent:**
> Your plan for the week is: Monday: 6.67 km (80 mins), Wednesday: 6.67 km (80 mins), Friday: 6.67 km (80 mins). Wait, your time window is only 60 minutes, so we must adjust the pace or distance.

---

**👤 You:**
> "Is a walking pace of 12 km/h safe?"

**🤖 AI Agent:**
> No, a pace of 12 km/h is generally considered running rather than walking and may exceed standard walking safety limits.

---

**👤 You:**
> "I have 30 minutes to walk 3km at a pace of 6 km/h. Will I finish in time?"

**🤖 AI Agent:**
> Yes, walking 3km at 6 km/h takes exactly 30 minutes, which fits within your available time.


## ❓ FAQ

**Q: How do I create a weekly walking plan?**
You can use the `calculate_weekly_schedule` tool by providing your total weekly distance, the days you want to walk, your pace, and your available time windows.

**Q: Can I check if my walking pace is too fast?**
Yes, the `validate_pace_safety` tool checks if your proposed speed is within realistic human limits for walking.

**Q: How does the tool handle rest days?**
Any day you do not designate as an active day is automatically treated as a rest day. You can use `get_rest_day_summary` to see a list of these days.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/walking-goal-calendar](https://vinkius.com/en/ai-agent-connect/walking-goal-calendar)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Walking Goal Calendar** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `walking-goal-calendar` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Walking Goal Calendar** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "walking-goal-calendar": {
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
