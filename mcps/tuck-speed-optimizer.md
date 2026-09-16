# Tuck Speed Optimizer MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/tuck-speed-optimizer)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [sports](../categories/sports.md)

Optimize rider aerodynamics using precise tuck angle modeling.

## Description
This MCP server provides advanced aerodynamic modeling to help riders find their most efficient body position. By analyzing rider height, chest width, wind speed, and slope, the server uses `calculate_optimal_tuck` to determine the best torso angle for minimizing drag. It also includes tools like `analyze_aerodynamic_impact` to evaluate speed changes and `evaluate_flexibility_constraint` to ensure the suggested position is physically sustainable. Perfect for cyclists and aerodynamic enthusiasts looking to maximize speed through better positioning.


## Available Tools (4)
- **analyze_aerodynamic_impact**: Evaluates how much speed is lost or gained due to specific environmental changes
- **evaluate_flexibility_constraint**: Checks if a proposed tuck position is physically sustainable for a given rider profile
- **get_drag_reduction_profile**: Provides a summary of drag reduction potential across different wind speeds for a specific rider
- **calculate_optimal_tuck**: Determines the best body position to minimize drag based on physical and environmental constraints


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Tuck Speed Optimizer** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is the best tuck angle for a rider who is 180cm tall, has a 45cm chest width, facing a 10m/s wind on a 2 degree slope with a flexibility score of 0.7?"

**🤖 AI Agent:**
> The optimal tuck angle for your profile is 24 degrees, which will provide an estimated drag reduction of 12% and a speed gain of 0.45 m/s.

---

**👤 You:**
> "Is a 15 degree tuck angle sustainable for someone with a flexibility score of 0.3?"

**🤖 AI Agent:**
> No, a 15 degree angle is not feasible for your flexibility level. It would result in an Extreme strain level.

---

**👤 You:**
> "How much speed will I gain if I improve my tuck from a neutral position?"

**🤖 AI Agent:**
> Based on your dimensions and current wind speed, moving to the optimal tuck will increase your velocity by 0.32 m/s.


## ❓ FAQ

**Q: How does the tool account for my physical limits?**
The `calculate_optimal_tuck` tool uses your flexibility score to ensure the recommended angle is physically achievable. You can also use `evaluate_flexibility_constraint` to verify if a specific angle is sustainable.

**Q: Can I use this to prepare for high wind conditions?**
Yes. You can use `get_drag_reduction_profile` to see how drag reduction changes across different wind speeds, accounting for factors like clothing flapping.

**Q: Does the slope of the road affect the results?**
Yes, the `calculate_optimal_tuck` tool takes the slope angle into account to provide a more accurate model of effective velocity and drag.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/tuck-speed-optimizer](https://vinkius.com/en/ai-agent-connect/tuck-speed-optimizer)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Tuck Speed Optimizer** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `tuck-speed-optimizer` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Tuck Speed Optimizer** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "tuck-speed-optimizer": {
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
