# Pomodoro Day Planner MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/pomodoro-day-planner)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Plan your productivity by calculating Pomodoro cycles and generating detailed work/break itineraries within any time window.

## Description
The Pomodoro Day Planner MCP server helps you maximize focus by partitioning available time into productive segments. Using tools like `generate_pomodoro_itinerary`, you can input a start and end time to receive a precise schedule of work periods and breaks. It also provides `predict_cycle_capacity` to estimate how many full cycles fit in a window and `calculate_available_minutes` for quick duration checks.

### Available Tools

`generate_itinerary`


## Available Tools (1)
- **generate_itinerary**: Generates a chronological itinerary for tasks


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Pomodoro Day Planner** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "I have from 9:00 AM to 12:00 PM today. How many 25-minute Pomodoro cycles can I fit if my breaks are 5 minutes?"

**🤖 AI Agent:**
> You can complete 6 full Pomodoro cycles within this 180-minute window.

---

**👤 You:**
> "Generate an itinerary for a session starting at 2024-05-20T14:00:00Z and ending at 2024-05-20T15:30:00Z with 30-minute work blocks and 10-minute breaks."

**🤖 AI Agent:**
> Your schedule is: 14:00:00 - Start Work, 14:30:00 - Start Break, 14:40:00 - Start Work, 15:10:00 - Start Break, 15:20:00 - Start Work.

---

**👤 You:**
> "Calculate the total minutes available between 2024-06-01T08:00:00Z and 2024-06-01T10:00:00Z."

**🤖 AI Agent:**
> The total duration is 120 minutes.


## ❓ FAQ

**Q: How do I use the planner?**
Provide a start and end time, then specify your preferred work and break durations to generate an itinerary. Tools available: `generate_itinerary`.

**Q: Can it handle residual work periods?**
Yes, if there is enough time for a work block but not a full break, the tool includes it in the schedule.

**Q: Does it support custom durations?**
Absolutely. You can define any number of minutes for your work and break intervals.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/pomodoro-day-planner](https://vinkius.com/mcp/pomodoro-day-planner)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Pomodoro Day Planner** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `pomodoro-day-planner` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Pomodoro Day Planner** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "pomodoro-day-planner": {
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
