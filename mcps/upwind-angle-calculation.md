# Upwind Angle Calculation MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/upwind-angle-calculation)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [marine](../categories/marine.md)

Physics-based kiteboarding performance analysis.

## Description
This MCP server provides specialized physics-based tools for kiteboarders to analyze their sailing performance. By calculating the relationship between wind, board velocity, and rider proficiency, it helps determine the most efficient paths. Use `getMaxUpwindAngle` to find the tightest possible sailing angle, `calculateVmgOptimization` to maximize progress toward the wind, `analyzeTackEfficiency` to evaluate maneuver performance, and `getEnvironmentalImpactReport` to understand how current and waves degrade performance.


## Available Tools (4)
- **analyzeTackEfficiency**: Evaluates how much performance is lost during a turn (tack) based on environmental and skill factors
- **calculateVmgOptimization**: Finds the optimal heading to maximize progress toward the wind
- **getEnvironmentalImpactReport**: Provides a summary of how current and waves specifically degrade the achievable sailing performance
- **getMaxUpwindAngle**: Determines the tightest possible angle a rider can sail relative to the true wind


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Upwind Angle Calculation** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is my maximum upwind angle with a 15 m/s wind, 0.8 kite efficiency, 12 m/s board speed, and 1.0 skill?"

**🤖 AI Agent:**
> Your maximum upwind angle is 42.5 degrees with a VMG of 8.8 m/s.

---

**👤 You:**
> "How much will a 2 m/s current and 0.5 wave drag affect my sailing?"

**🤖 AI Agent:**
> The environmental impact includes an angle degradation of 4.2 degrees and a speed reduction of 1.1 m/s.

---

**👤 You:**
> "Calculate the optimal heading for 10 m/s wind and 10 m/s board speed with 0.85 efficiency and 1.1 skill."

**🤖 AI Agent:**
> The optimal angle is 38.2 degrees, resulting in a peak VMG of 7.6 m/s.


## ❓ FAQ

**Q: How do I use this to plan my route?**
You can use `getMaxUpwindAngle` to determine your minimum angle and then use `calculateVmgOptimization` to find the heading that provides the best progress toward your destination.

**Q: Does this account for water current?**
Yes, the `getMaxUpwindAngle` tool allows you to input `currentSpeed` to see how the water movement affects your achievable upwind angle.

**Q: Can I evaluate my skill level?**
Yes, you can input a `riderSkill` multiplier to see how technical proficiency impacts your VMG and tack efficiency.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/upwind-angle-calculation](https://vinkius.com/ai-agent-connect/upwind-angle-calculation)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Upwind Angle Calculation** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `upwind-angle-calculation` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Upwind Angle Calculation** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "upwind-angle-calculation": {
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
