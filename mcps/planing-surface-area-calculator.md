# Planing Surface Area Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/planing-surface-area-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [hydrodynamics](../categories/hydrodynamics.md)

Calculate hydrodynamic planing metrics, stability, and rocker impact for boards.

## Description
This MCP server provides hydrodynamic analysis for boards riding on water surfaces. It allows AI agents to calculate critical metrics like wetted length and planing area using `get_planing_metrics`. Users can evaluate stability with `get_stability_assessment`, analyze how tail curvature affects performance via `get_rocker_impact_analysis`, and determine efficiency tiers using `get_lift_efficiency_ratio`.


## Available Tools (4)
- **get_stability_assessment**: Evaluates how stable the board is likely to be based on the calculated planing area and speed
- **get_lift_efficiency_ratio**: Determines the efficiency of the board by comparing lift produced to the total surface area
- **get_planing_metrics**: Calculates the primary hydrodynamic characteristics of the board under current riding conditions
- **get_rocker_impact_analysis**: Specifically analyzes how changes in the tail rocker affect the planing surface area


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Planing Surface Area Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is the planing area for a 7ft board, 20in wide, moving at 15 knots with a 3 degree angle of attack?"

**🤖 AI Agent:**
> The calculated planing area for your board is 425.5 square inches.

---

**👤 You:**
> "Is my board stable at 25 knots with a wetted length of 4ft and width of 22in?"

**🤖 AI Agent:**
> No, at 25 knots with that wetted length, the stability score is low, indicating a high risk of instability.

---

**👤 You:**
> "How much will increasing my rocker from 0.1 to 0.2 reduce my planing area at 12 knots?"

**🤖 AI Agent:**
> Increasing the rocker to 0.2 will reduce the planing area by approximately 12%.


## ❓ FAQ

**Q: How do I calculate the planing area?**
You can use the `get_planing_metrics` tool by providing the board length, width, speed, and angle of attack.

**Q: Can I analyze the effect of tail rocker?**
Yes, the `get_rocker_impact_analysis` tool specifically calculates how changes in rocker affect the planing surface area.

**Q: How is stability determined?**
Stability is assessed using `get_stability_assessment`, which evaluates the relationship between wetted length, speed, and board width.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/planing-surface-area-calculator](https://vinkius.com/en/ai-agent-connect/planing-surface-area-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Planing Surface Area Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `planing-surface-area-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Planing Surface Area Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "planing-surface-area-calculator": {
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
