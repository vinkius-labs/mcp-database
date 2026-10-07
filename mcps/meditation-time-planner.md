# Meditation Time Planner MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/meditation-time-planner)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Automated scheduling engine for optimizing meditation sessions within daily time windows.

## Description
This MCP server provides a specialized scheduling engine designed to place meditation sessions into available daily time windows. It respects session durations, frequency requirements, and user-defined preferred time ranges. The engine uses `plan_meditation_schedule` to map sessions to free blocks, `check_schedule_conflicts` to ensure mandatory separation between practices, `find_optimal_windows` to prioritize preferred times, and `get_session_capacity_report` to verify if a schedule is mathematically possible given the available time.


## Available Tools (4)
- **get_session_capacity_report**: Calculates whether the current daily windows can mathematically support the requested meditation frequency
- **check_schedule_conflicts**: Validates an existing schedule against a set of conflict rules
- **find_optimal_windows**: Identifies the best time slots within the available windows that align with user preferences
- **plan_meditation_schedule**: Generates a complete schedule by mapping requested sessions into available time windows


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Meditation Time Planner** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Can you create a schedule for two 20-minute mindfulness sessions and one 30-minute zen session in my available windows from 08:00 to 12:00 and 14:00 to 18:00?"

**🤖 AI Agent:**
> I have scheduled your sessions: Mindfulness at 08:00-08:20, Mindfulness at 09:00-09:20, and Deep Zen at 14:00-14:30.

---

**👤 You:**
> "Check if I have enough time today for three 15-minute meditations if my free windows are 09:00-10:00 and 15:00-16:00."

**🤖 AI Agent:**
> Yes, you have 120 minutes of available time, which is sufficient for the 45 minutes of total required meditation time.

---

**👤 You:**
> "Verify if my current schedule has any overlapping sessions with a 10-minute buffer."

**🤖 AI Agent:**
> The schedule is valid and respects the 10-minute separation requirement between all sessions.


## ❓ FAQ

**Q: How does the planner handle preferred times?**
The engine uses `find_optimal_windows` to identify time slots that best match your preferences, prioritizing them during the scheduling process.

**Q: Can I prevent sessions from being too close together?**
Yes, you can define conflict rules. The `check_schedule_conflicts` tool ensures that all scheduled sessions respect the mandatory minimum separation time you specify.

**Q: What happens if I request more meditation time than I have available?**
You can use `get_session_capacity_report` to check if your requested frequency and durations can fit into your available windows before attempting to build a full schedule.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/meditation-time-planner](https://vinkius.com/en/ai-agent-connect/meditation-time-planner)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Meditation Time Planner** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `meditation-time-planner` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Meditation Time Planner** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "meditation-time-planner": {
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
