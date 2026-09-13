# Horizontal Well IPR Analyzer MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/horizontal-well-ipr-analyzer)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [oil-and-gas](../categories/oil-and-gas.md)

Generates Inflow Performance Relationship (IPR) curves and performance metrics for horizontal wells.

## Description
This MCP server provides specialized tools for modeling the inflow performance of horizontal wells. It calculates the Inflow Performance Relationship (IPR) curve, determines the Absolute Open Flow (AOF), and identifies the optimal drawdown to maximize production efficiency. The tools account for reservoir anisotropy, two-phase flow impacts, and solution gas drive to provide accurate performance metrics for horizontal wellbore configurations.


## Available Tools (4)
- **calculate_aof**: Determines the theoretical maximum flow rate (AOF) for the well
- **analyze_two_phase_impact**: Evaluates how the presence of gas affects the inflow performance
- **calculate_ipr_curve**: Generates a set of flow rate data points across a range of bottomhole pressures to model the IPR curve
- **calculate_optimal_drawdown**: Identifies the ideal pressure drop to maximize production efficiency


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Horizontal Well IPR Analyzer** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Generate an IPR curve for a well with 3000 psi reservoir pressure, 2500 psi bottomhole pressure, 1000 ft length, 50 mD permeability, 0.5 anisotropy, and fluid properties including viscosity and GOR."

**🤖 AI Agent:**
> The calculated IPR curve shows a flow rate of 1250 STB/d at a bottomhole pressure of 2500 psi.

---

**👤 You:**
> "What is the absolute open flow for a well with 4000 psi reservoir pressure, 1500 ft length, 100 mD permeability, and 0.4 anisotropy?"

**🤖 AI Agent:**
> The Absolute Open Flow (AOF) for this well is 4500 STB/d.

---

**👤 You:**
> "Find the optimal drawdown for a reservoir at 3500 psi with 800 ft horizontal length and 40 mD permeability."

**🤖 AI Agent:**
> The optimal drawdown is 850 psi, which yields an expected flow rate of 1800 STB/d.


## ❓ FAQ

**Q: How do I model the IPR curve for my horizontal well?**
You can use the `calculate_ipr_curve` tool by providing the reservoir pressure, target bottomhole pressure, horizontal length, permeability, anisotropy ratio, and fluid properties.

**Q: Can I calculate the maximum possible flow rate?**
Yes, the `calculate_aof` tool determines the Absolute Open Flow rate by extrapolating the IPR curve to zero bottomhole pressure.

**Q: How does gas presence affect my results?**
The `analyze_two_phase_impact` tool evaluates how the transition to two-phase flow reduces the productivity index due to gas liberation.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/horizontal-well-ipr-analyzer](https://vinkius.com/en/ai-agent-connect/horizontal-well-ipr-analyzer)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Horizontal Well IPR Analyzer** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `horizontal-well-ipr-analyzer` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Horizontal Well IPR Analyzer** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "horizontal-well-ipr-analyzer": {
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
