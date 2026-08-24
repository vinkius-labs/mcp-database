# Running Pace & Split Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/running-pace-split-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [utilities](../categories/utilities.md)

Generate precise running pace schedules and cumulative time markers.

## Description
This MCP server provides deterministic tools for runners to plan their races. Use `generate_split_plan` to create a full schedule of paces and cumulative time markers for any distance. You can also use `project_finish_time` to estimate your final time based on your current pace, or `validate_pace_integrity` to ensure your split data matches your target goal.


## Available Tools (3)
- **generate_split_plan**: Calculates a full schedule of paces and cumulative times to meet a specific target
- **project_finish_time**: Predicts the end time based on a runner's current performance
- **validate_pace_integrity**: Verifies if a set of splits actually results in the target time


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Running Pace & Split Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Generate a split plan for a 10km run with a target time of 00:50:00 and 1km splits."

**🤖 AI Agent:**
> Here is your 10km split plan for a 50-minute target: 1km: 05:00 (00:05:00), 2km: 05:00 (00:10:00), 3km: 05:00 (00:15:00), 4km: 05:00 (00:20:00), 5km: 05:00 (00:25:00), 6km: 05:00 (00:30:00), 7km: 05:00 (00:35:00), 8km: 05:00 (00:40:00), 9km: 05:00 (00:45:00), 10km: 05:00 (00:50:00).

---

**👤 You:**
> "I have run 5km at a pace of 05:30. I have 5km left. What is my projected finish time?"

**🤖 AI Agent:**
> Your projected total time is 00:55:00.

---

**👤 You:**
> "Check if these splits are correct for a 00:40:00 target: [{"splitPace": "08:00"}, {"splitPace": "08:00"}, {"splitPace": "08:00"}, {"splitPace": "08:00"}, {"splitPace": "08:00"}]"

**🤖 AI Agent:**
> Yes, the splits are consistent with the target time.


## ❓ FAQ

**Q: How do I create a race plan?**
Use the `generate_split_plan` tool by providing your total distance, target time, and desired split interval.

**Q: Can I predict my finish time?**
Yes, use `project_finish_time` with your current distance, remaining distance, and current pace.

**Q: Does it support both kilometers and miles?**
Yes, all tools support both 'km' and 'miles' units.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/running-pace-split-calculator](https://vinkius.com/ai-agent-connect/running-pace-split-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Running Pace & Split Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `running-pace-split-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Running Pace & Split Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "running-pace-split-calculator": {
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
