# Wellbore Pressure Drop Model MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/wellbore-pressure-drop-model)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [engineering](../categories/engineering.md)

Calculates multiphase pressure profiles and flow regimes in wellbores.

## Description
This MCP server provides specialized engineering tools to simulate fluid production in wellbores. It accounts for multiphase flow dynamics, phase slip, and varying inclination angles. Using established correlations like Hagedorn-Brown and Beggs-Brill, it calculates the complete pressure profile, bottomhole pressure, and wellhead pressure. You can also use `analyze_flow_regime` to identify specific flow patterns like slug or annular flow at any depth.


## Available Tools (4)
- **calculate_pressure_profile**: Generates a complete map of pressure changes at specific depth intervals along the entire wellbore
- **analyze_flow_regime**: Identifies the specific pattern of fluid movement (e.g., slug flow) at a given point in the well
- **get_bottomhole_pressure**: Determines the pressure at the very bottom of the well
- **get_wellhead_pressure**: Calculates the surface pressure based on a known bottomhole pressure and the resistance encountered during ascent


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Wellbore Pressure Drop Model** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Calculate the pressure profile for a vertical well with a flow rate of 500 m3/day, density of 800 kg/m3, viscosity of 0.001 Pa·s, diameter of 0.15m, depth of 2000m, and a temperature gradient of 0.03 C/m using Hagedorn-Brown."

**🤖 AI Agent:**
> The calculated pressure profile shows a starting bottomhole pressure of 16.5 MPa and a wellhead pressure of 12.2 MPa at the surface.

---

**👤 You:**
> "What is the flow regime at 500m depth for this well?"

**🤖 AI Agent:**
> At a depth of 500m, the flow regime is identified as slug flow with a slip velocity of 1.2 m/s.

---

**👤 You:**
> "Find the bottomhole pressure if the wellhead pressure is 5 MPa and the profile is provided."

**🤖 AI Agent:**
> The bottomhole pressure at the maximum depth is 14.8 MPa.


## ❓ FAQ

**Q: Which flow correlations are supported?**
The model supports Hagedorn-Brown, Beggs-Brill, and Duns-Ros correlations.

**Q: Can I determine the flow pattern at a specific depth?**
Yes, you can use the `analyze_flow_regime` tool to identify the flow regime and slip velocity at any given depth.

**Q: How does inclination affect the results?**
The inclination angle is a critical input for `calculate_pressure_profile` as it determines the hydrostatic component of the pressure drop.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/wellbore-pressure-drop-model](https://vinkius.com/ai-agent-connect/wellbore-pressure-drop-model)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Wellbore Pressure Drop Model** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `wellbore-pressure-drop-model` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Wellbore Pressure Drop Model** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "wellbore-pressure-drop-model": {
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
