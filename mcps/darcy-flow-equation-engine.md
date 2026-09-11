# Darcy Flow Equation Engine MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/darcy-flow-equation-engine)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [engineering](../categories/engineering.md)

Calculate fluid flow rates, velocities, and pressure profiles in porous media using Darcy's Law.

## Description
This MCP server provides specialized computational tools for analyzing fluid movement through porous structures. It implements Darcy's Law to determine flow characteristics across different geometries and regimes. Use `calculate_linear_flow` for uniform channels, `calculate_radial_flow` for cylindrical patterns like wellbores, and `compare_flow_regimes` to evaluate the impact of steady-state versus pseudo-steady state conditions. You can also use `get_pressure_profile` to pinpoint specific pressure values at any given distance or radius.


## Available Tools (4)
- **calculate_radial_flow**: g., around a wellbore) using Darcy's law.

Calculates flow rate and pressure characteristics for fluid moving in a circular or cylindrical pattern
- **compare_flow_regimes**: Compares flow rate between steady-state and pseudo-steady state conditions
- **get_pressure_profile**: Calculates the specific pressure value at a specific point along a flow path
- **calculate_linear_flow**: Calculates flow rate, velocity, and pressure profile for fluid moving through a uniform channel


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Darcy Flow Equation Engine** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Calculate the flow rate for a linear flow with permeability 1e-12, area 0.01, pressure gradient 500, and viscosity 0.001 over a distance of 2 meters."

**🤖 AI Agent:**
> The calculated flow rate is 5.0 m³/s with a velocity of 500 m/s.

---

**👤 You:**
> "What is the flow rate for radial flow with permeability 1e-12, inner radius 0.1, outer radius 0.5, pressure difference 1000, and viscosity 0.001?"

**🤖 AI Agent:**
> The radial flow rate is 125.66 m³/s.

---

**👤 You:**
> "Compare steady-state and pseudo-steady state flow for a linear system with permeability 1e-12, area 0.01, pressure gradient 500, and viscosity 0.001."

**🤖 AI Agent:**
> The steady-state flow rate is 5.0 m³/s, while the pseudo-steady state flow rate is 4.8 m³/s, representing a 4% difference.


## ❓ FAQ

**Q: What geometries are supported?**
The engine supports both linear flow through uniform channels and radial flow through cylindrical patterns.

**Q: Can I compare steady-state and pseudo-steady state conditions?**
Yes, you can use the `compare_flow_regimes` tool to see the percentage difference in flow rates between these two states.

**Q: How do I find the pressure at a specific distance?**
Use the `get_pressure_profile` tool by providing the geometry, physical constants, and the specific target point.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/darcy-flow-equation-engine](https://vinkius.com/en/ai-agent-connect/darcy-flow-equation-engine)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Darcy Flow Equation Engine** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `darcy-flow-equation-engine` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Darcy Flow Equation Engine** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "darcy-flow-equation-engine": {
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
