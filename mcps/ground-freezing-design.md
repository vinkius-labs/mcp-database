# Ground Freezing Design MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/ground-freezing-design)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [construction](../categories/construction.md)

Engineering tool for calculating freeze-wall formation parameters for shaft and tunnel excavations.

## Description
This MCP server provides specialized engineering calculations for artificial ground freezing (AGF) projects. It allows AI agents to design stable ice barriers for shaft and tunnel excavations by calculating optimal pipe layouts, predicting freezing durations, determining refrigeration loads, and verifying structural stability. Use `get_freeze_pipe_layout` to determine pipe spacing, `estimate_freezing_time` to predict process duration, `calculate_refrigeration_load` for cooling requirements, and `validate_structural_stability` to ensure the ice wall can withstand hydrostatic and earth pressures.


## Available Tools (4)
- **calculate_refrigeration_load**: Determines the total cooling capacity required to maintain the ice wall against ground heat and water flow
- **estimate_freezing_time**: Predicts how long it will take for the ice wall to reach the required thickness and stability
- **get_freeze_pipe_layout**: Determines the optimal arrangement and distance between freeze pipes to ensure a continuous ice barrier
- **validate_structural_stability**: Checks if the designed ice wall can withstand the external pressures at the excavation depth


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Ground Freezing Design** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is the optimal pipe spacing for a shaft with a 5m radius, soil thermal conductivity of 2.5 W/mK, and a target wall thickness of 2m?"

**🤖 AI Agent:**
> The optimal pipe spacing for your shaft is 1.2 meters, requiring a total of 26 pipes for the perimeter.

---

**👤 You:**
> "How long will it take to form a 2m thick ice wall if the pipe spacing is 1.5m, soil latent heat is 334 kJ/kg, and groundwater velocity is 0.01 m/s?"

**🤖 AI Agent:**
> The estimated freezing time is 450 hours with a 95% confidence interval.

---

**👤 You:**
> "Calculate the refrigeration load for 30 pipes with a groundwater velocity of 0.02 m/s and a ground temperature of 10°C for a 300-hour duration."

**🤖 AI Agent:**
> The required cooling capacity is 150 kW with a peak load of 185 kW.


## ❓ FAQ

**Q: How do I determine the distance between freeze pipes?**
You can use the `get_freeze_pipe_layout` tool, providing the excavation geometry, soil thermal conductivity, and target wall thickness.

**Q: Does groundwater flow affect the design?**
Yes, groundwater velocity is a critical factor. You must use `estimate_freezing_time` and `calculate_refrigeration_load` to account for the heat introduced by moving water.

**Q: How can I verify if my ice wall is safe?**
Use the `validate_structural_stability` tool to check the safety factor against earth and hydrostatic pressures.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/ground-freezing-design](https://vinkius.com/ai-agent-connect/ground-freezing-design)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Ground Freezing Design** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `ground-freezing-design` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Ground Freezing Design** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "ground-freezing-design": {
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
