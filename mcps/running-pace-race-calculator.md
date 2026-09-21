# Running Pace & Race Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/running-pace-race-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [utilities](../categories/utilities.md)

Calculate race split plans, pace conversions, and elevation adjustments.

## Description
This MCP server provides specialized tools for runners to manage their race strategies. Use `pace_convert` to switch between speed and pace or metric and imperial units. Generate detailed pacing strategies with `split_plan_generator`, allowing for even or progressive split plans. Account for course difficulty using `elevation_impact_calculator` to adjust target times based on climb, and use `race_checkpoint_query` to find exact elapsed times at specific distance markers.


## Available Tools (4)
- **elevation_impact_calculator**: Adjusts the target finish time or required pace based on the course's total elevation gain
- **race_checkpoint_query**: Calculates the exact time a runner should reach specific distance markers during a race
- **split_plan_generator**: Generates detailed split strategies (even or progressive) for a specific race distance and target time
- **pace_convert**: Converts between pace and speed or between distance/time units


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Running Pace & Race Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Convert a pace of 5:00 min/km to speed in km/h."

**🤖 AI Agent:**
> 12 km/h

---

**👤 You:**
> "Generate an even split plan for a 10km race with a target time of 50 minutes, divided into 5 segments."

**🤖 AI Agent:**
> The even split plan for 10km in 50 minutes consists of 5 segments of 2km each, with a constant pace of 5:00 min/km.

---

**👤 You:**
> "What is the estimated time for a 42.2km marathon if I have 1000m of elevation gain and my flat time is 3 hours?"

**🤖 AI Agent:**
> The adjusted time for the marathon with 1000m of elevation gain is approximately 3 hours and 12 minutes.


## ❓ FAQ

**Q: How do I create a pacing plan for a marathon?**
You can use the `split_plan_generator` tool. Provide the total distance, your target finish time in seconds, and choose between an even or progressive split strategy.

**Q: Can I adjust my target time for hilly courses?**
Yes, the `elevation_impact_calculator` tool allows you to estimate how much extra time elevation gain will add to your base time.

**Q: Does this support both metric and imperial units?**
Yes, all tools like `pace_convert` support both metric and imperial systems for distance, pace, and elevation.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/running-pace-race-calculator](https://vinkius.com/en/ai-agent-connect/running-pace-race-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Running Pace & Race Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `running-pace-race-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Running Pace & Race Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "running-pace-race-calculator": {
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
