# Garden Task Season Calendar MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/garden-task-season-calendar)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

A specialized scheduling engine that transforms raw gardening tasks into a seasonally-aware execution calendar.

## Description
This MCP server provides a sophisticated scheduling engine for gardeners. It reconciles task frequency with regional growth windows and restricted periods to produce a precise, dated calendar. Use `generate_consolidated_calendar` to create a unified timeline, or `calculate_task_schedule` to project specific recurring dates. The engine accounts for crop stages, regional seasons, and blackout dates to ensure your gardening activities align perfectly with the natural growing cycle.


## Available Tools (4)
- **filter_blackout_dates**: Removes scheduled tasks that conflict with restricted periods
- **generate_consolidated_calendar**: Orchestrates the full flow to produce a single unified timeline
- **get_regional_season_window**: Retrieves the valid date ranges for a specific region's seasons
- **calculate_task_schedule**: Generates a chronological list of specific dates for a single task based on its rules


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Garden Task Season Calendar** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Generate a gardening calendar for the Northern Hemisphere with a watering task every 3 days starting May 1st."

**🤖 AI Agent:**
> Your gardening calendar for the Northern Hemisphere is ready. The watering task is scheduled for May 1st, May 4th, May 7th, and continues every 3 days throughout the valid seasonal window.

---

**👤 You:**
> "What are the seasonal windows for the Southern Hemisphere?"

**🤖 AI Agent:**
> In the Southern Hemisphere, the seasons are defined as: Spring (September to November), Summer (December to February), Autumn (March to May), and Winter (June to August).

---

**👤 You:**
> "Calculate the schedule for a 'Fertilizing' task every 14 days starting June 10th for the Vegetative stage in the Northern Hemisphere."

**🤖 AI Agent:**
> The fertilizing schedule is set for June 10th, June 24th, July 8th, and July 22nd.


## ❓ FAQ

**Q: How do I generate a full gardening schedule?**
You can use the `generate_consolidated_calendar` tool. Provide your list of tasks, the target region, and any blackout dates to receive a sorted, complete timeline.

**Q: Can I exclude specific dates from my calendar?**
Yes. By using `filter_blackout_dates`, you can remove any scheduled task occurrences that fall within your specified restricted periods.

**Q: How does the tool handle different seasons?**
The engine uses `get_regional_season_window` to retrieve valid date ranges for your specific region, ensuring tasks like flowering or germination are only scheduled during appropriate seasonal windows.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/garden-task-season-calendar](https://vinkius.com/en/ai-agent-connect/garden-task-season-calendar)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Garden Task Season Calendar** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `garden-task-season-calendar` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Garden Task Season Calendar** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "garden-task-season-calendar": {
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
