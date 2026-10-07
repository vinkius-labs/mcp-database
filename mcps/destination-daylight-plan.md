# destination-daylight-plan MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/destination-daylight-plan)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Optimizes outdoor activity schedules based on daylight windows and travel constraints.

## Description
This MCP server provides specialized tools to maximize usable daylight for outdoor excursions. By analyzing sunrise and sunset times against travel requirements and activity priorities, it generates efficient schedules. Use `plan_daylight_schedule` to create a prioritized sequence of activities, `calculate_daylight_availability` to find your usable window, or `validate_activity_fit` to check if a specific task is feasible within your constraints.


## Available Tools (4)
- **get_priority_summary**: Provides a high-level overview of how many activities were prioritized versus how many were skipped
- **plan_daylight_schedule**: Generates a prioritized sequence of activities that fit within the available daylight
- **validate_activity_fit**: Checks if a specific activity can be performed given the current daylight constraints
- **calculate_daylight_availability**: Determines the raw window of time available for any outdoor activity


## 💬 Prompt Examples

Here are some examples of how you can interact with the **destination-daylight-plan** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Plan my day: Sunrise is 06:00, sunset is 18:00. I have 60 minutes of travel. My activities are: Hiking (120 mins, priority 5) and Bird Watching (60 mins, priority 3)."

**🤖 AI Agent:**
> Your planned activities are: Hiking from 06:00 to 08:00 and Bird Watching from 08:00 to 09:00.

---

**👤 You:**
> "How much daylight do I have if sunrise is 05:30, sunset is 20:00, and I need a 30-minute safety buffer?"

**🤖 AI Agent:**
> You have 885 minutes of available daylight between 05:30 and 19:30.

---

**👤 You:**
> "Can I fit a 3-hour photography session if I have 150 minutes of daylight left and 20 minutes of travel?"

**🤖 AI Agent:**
> No, the photography session is not feasible as it requires 180 minutes plus travel, exceeding your 150 minutes of available daylight.


## ❓ FAQ

**Q: How does the scheduling work?**
The engine calculates the total daylight window and subtracts travel time. It then sorts your activities by priority to ensure the most important tasks are scheduled first.

**Q: Can I include travel time in my planning?**
Yes, you can provide travel duration to ensure the `plan_daylight_schedule` tool accounts for transit time when determining activity windows.

**Q: What happens if an activity is too long?**
If an activity's duration exceeds the remaining available daylight, the tool will skip it to ensure the schedule remains realistic.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/destination-daylight-plan](https://vinkius.com/en/ai-agent-connect/destination-daylight-plan)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **destination-daylight-plan** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `destination-daylight-plan` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **destination-daylight-plan** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "destination-daylight-plan": {
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
