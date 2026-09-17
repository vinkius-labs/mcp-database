# Steady-State Pace Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/steady-state-pace-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [health](../categories/health.md)

Calculate target paces, split times, and training progressions for aerobic endurance.

## Description
This MCP server provides specialized tools for endurance athletes to manage steady-state aerobic training. Use `calculate_target_pace` to determine the exact speed needed to maintain a specific heart rate for running, cycling, or swimming. You can also use `get_split_times` to plan segment intervals, `calculate_progression_plan` to systematically increase training volume over several weeks, and `verify_zone_intensity` to ensure your target heart rate is appropriate for aerobic efforts.


## Available Tools (4)
- **calculate_progression_plan**: Generates a weekly training progression plan
- **calculate_target_pace**: Calculates target pace and estimated duration based on modality and heart rate
- **get_split_times**: Calculates cumulative split times for a given distance and interval
- **verify_zone_intensity**: Verifies if a heart rate is appropriate for steady-state aerobic training


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Steady-State Pace Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What pace should I run to keep my heart rate at 140 bpm for a 10km run?"

**🤖 AI Agent:**
> To maintain a heart rate of 140 bpm for a 10km run, your target pace is 06:15 min/km, with an estimated total duration of 01:02:30.

---

**👤 You:**
> "Give me split times for a 5km run at a pace of 05:00 min/km, every 1 km."

**🤖 AI Agent:**
> For a 5km run at 05:00 min/km, your splits are: 1km at 05:00, 2km at 10:00, 3km at 15:00, 4km at 20:00, and 5km at 25:00.

---

**👤 You:**
> "I currently run 5km in 30 minutes. Create a 4-week progression plan with a 10% weekly increase."

**🤖 AI Agent:**
> Your 4-week progression plan is: Week 1: 5.50 km / 33:00 min; Week 2: 6.05 km / 36:30 min; Week 3: 6.66 km / 40:18 min; Week 4: 7.33 km / 44:19 min.


## ❓ FAQ

**Q: How do I know if my heart rate is correct for steady-state training?**
You can use the `verify_zone_intensity` tool. By providing your target heart rate and maximum heart rate, the tool will confirm if you are within the appropriate physiological zone for aerobic effort.

**Q: Can I plan my training increase for multiple weeks?**
Yes, the `calculate_progression_plan` tool allows you to generate a weekly schedule that systematically increases your distance or duration based on a specific percentage increment.

**Q: What modalities are supported?**
The calculator supports running, cycling, and swimming through the `calculate_target_pace` tool, adjusting for the specific metabolic costs of each activity.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/steady-state-pace-calculator](https://vinkius.com/en/ai-agent-connect/steady-state-pace-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Steady-State Pace Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `steady-state-pace-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Steady-State Pace Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "steady-state-pace-calculator": {
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
