# Training Pace Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/training-pace-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Calculate running training intensity zones and race pace predictions based on performance or VO2max.

## Description
The Training Pace Calculator MCP server provides precise tools for runners to determine their optimal training intensities. By using `calculate_zones_from_pace`, you can derive specific zones (Easy, Aerobic, Tempo, Interval, and VO2max) in both metric (min/km) and imperial (min/mile) formats based on a recent race result. Alternatively, if you only know your physiological capacity, `calculate_zones_from_vo2max` uses your VO2max value to estimate these same training zones. For runners looking to plan for future goals, the `estimate_distance_conversion` tool utilizes Riegel's formula to predict how your pace might change as you move from shorter distances like a 5K to longer ones like a Marathon.


## Available Tools (3)
- **estimate_distance_conversion**: Uses Riegel's formula.

Predict pace for a different distance based on current performance
- **calculate_zones_from_pace**: g., 5K, 10K). Returns training zones in km and mile formats.

Calculate training intensity zones based on a recent race pace
- **calculate_zones_from_vo2max**: Returns training zones in km and mile formats.

Calculate training intensity zones based on VO2max


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Training Pace Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Calculate my training zones based on a 5K pace of 05:00."

**🤖 AI Agent:**
> Based on your 5K pace of 05:00, your training zones are: Easy (05:45 min/km), Aerobic (05:25 min/km), Tempo (05:10 min/km), Interval (04:55 min/km), and VO2max (04:45 min/km).

---

**👤 You:**
> "What is my predicted 10K pace if my current 5K pace is 04:30?"

**🤖 AI Agent:**
> Your predicted 10K pace is approximately 04:52.

---

**👤 You:**
> "Calculate training zones using a VO2max of 45."

**🤖 AI Agent:**
> With a VO2max of 45 ml/kg/min, your estimated training zones are: Easy (06:10 min/km), Aerobic (05:50 min/km), Tempo (05:35 min/km), Interval (05:20 min/km), and VO2max (05:05 min/km).


## ❓ FAQ

**Q: How do I calculate my training zones from a recent race?**
Use the `calculate_zones_from_pace` tool. Provide your recent race pace in 'mm:ss' format and the distance of that race (e.g., 5K or 10K).

**Q: Can I estimate my marathon pace from a 5K result?**
Yes, you can use the `estimate_distance_conversion` tool. Input your current 5K pace and set the target distance to 'Marathon' to see the predicted performance.

**Q: What if I don't have a recent race time?**
You can use the `calculate_zones_from_vo2max` tool. Simply provide your VO2max value in ml/kg/min to get your estimated training zones.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/training-pace-calculator](https://vinkius.com/mcp/training-pace-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Training Pace Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `training-pace-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Training Pace Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "training-pace-calculator": {
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
