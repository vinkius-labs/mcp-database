# Well Inflow Performance Relationship (IPR) Engine MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/well-inflow-performance-relationship-ipr-engine)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [engineering](../categories/engineering.md)

Calculate oil well inflow performance, AOF, and optimal production rates using Vogel and Fetkovich models.

## Description
This MCP server provides specialized engineering calculations for modeling the Inflow Performance Relationship (IPR) of oil wells. It allows AI agents to determine potential flow rates based on reservoir pressure, bubble point pressure, and productivity index. Using tools like `calculate_ipr_parameters` and `get_maximum_flow_capacity`, agents can identify if a well is in a single-phase or two-phase regime and calculate the Absolute Open Flow (AOF). The engine also includes `optimize_producing_rate` to find the best production balance and `analyze_gas_drive_impact` to evaluate how gas liberation affects flow performance.


## Available Tools (4)
- **get_maximum_flow_capacity**: Calculates the theoretical maximum flow rate (AOF)
- **calculate_ipr_parameters**: Determines the core inflow performance metrics for a well
- **analyze_gas_drive_impact**: Evaluates how solution gas drive affects the inflow performance as pressure declines
- **optimize_producing_rate**: Identifies the optimal flow rate to balance production against pressure drawdown constraints


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Well Inflow Performance Relationship (IPR) Engine** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Calculate the IPR parameters for a well with 3000 psi reservoir pressure, 2500 psi bubble point, 1.5 PI, and 2000 psi flowing bottomhole pressure."

**🤖 AI Agent:**
> The current flow rate is 1500 STB/d and the well is operating in a Two-Phase regime.

---

**👤 You:**
> "What is the maximum flow capacity for a reservoir with 4000 psi pressure, 3000 psi bubble point, and 2.0 PI?"

**🤖 AI Agent:**
> The Absolute Open Flow (AOF) for this well is 8000 STB/d.

---

**👤 You:**
> "Find the optimal rate for a well with 3500 psi reservoir pressure, 2800 psi bubble point, 1.2 PI, and a minimum allowed pressure of 2200 psi."

**🤖 AI Agent:**
> The optimal rate is 1560 STB/d at a bottomhole pressure of 2200 psi, with a safety margin of 600 psi before two-phase flow begins.


## ❓ FAQ

**Q: How does the tool handle two-phase flow?**
When the flowing bottomhole pressure drops below the bubble point pressure, the `calculate_ipr_parameters` tool automatically switches to Vogel's model to account for gas evolution.

**Q: What is Absolute Open Flow (AOF)?**
AOF is the theoretical maximum flow rate achievable if the bottomhole pressure were reduced to zero. You can find this using `get_maximum_flow_capacity`.

**Q: Can I optimize my production rate?**
Yes, the `optimize_producing_rate` tool identifies the highest achievable rate without letting the bottomhole pressure drop below your specified minimum safety threshold.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/well-inflow-performance-relationship-ipr-engine](https://vinkius.com/ai-agent-connect/well-inflow-performance-relationship-ipr-engine)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Well Inflow Performance Relationship (IPR) Engine** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `well-inflow-performance-relationship-ipr-engine` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Well Inflow Performance Relationship (IPR) Engine** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "well-inflow-performance-relationship-ipr-engine": {
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
