# Kick Tolerance Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/kick-tolerance-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [engineering](../categories/engineering.md)

Calculate critical well control safety limits including MAASP and maximum influx volume.

## Description
This MCP server provides essential well control calculations to maintain the drilling window. It allows AI agents to determine the Maximum Allowable Annular Surface Pressure (MAASP) using `calculate_maasp`, calculate the maximum safe influx volume with `calculate_kick_tolerance_volume`, and determine surface pressure limits via `calculate_max_surface_pressure`. It also provides wellbore geometry analysis through `get_wellbore_capacity` to ensure formation integrity is maintained during kick management.


## Available Tools (4)
- **calculate_kick_tolerance_volume**: Calculates the maximum volume of an influx that can be tolerated before the shoe fractures
- **calculate_maasp**: Determines the maximum safe pressure that can be applied to the annulus
- **calculate_max_surface_pressure**: Calculates the maximum pressure allowed at the surface during a kick
- **get_wellbore_capacity**: Provides the volume capacity of the wellbore based on geometry


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Kick Tolerance Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is the MAASP for a shoe depth of 2000m, fracture gradient of 1.5 psi/ft, pore pressure of 1.0 psi/ft, and mud weight of 1.2 psi/ft?"

**🤖 AI Agent:**
> The Maximum Allowable Annular Surface Pressure (MAASP) is 600 psi.

---

**👤 You:**
> "Calculate the maximum influx volume if the shoe depth is 2500m, fracture gradient is 1.6, pore pressure is 1.1, mud weight is 1.3, influx density is 0.1, and annular capacity is 0.05."

**🤖 AI Agent:**
> The maximum tolerated influx volume is 125 cubic units.

---

**👤 You:**
> "What is the maximum surface pressure for a gas kick at 500m depth if the MAASP is 800 psi?"

**🤖 AI Agent:**
> The maximum surface pressure allowed is 750 psi.


## ❓ FAQ

**Q: What is MAASP?**
MAASP is the Maximum Allowable Annular Surface Pressure, which is the maximum pressure that can be applied to the annulus before the formation at the casing shoe fractures.

**Q: How does the tool handle gas vs water influx?**
The `calculate_max_surface_pressure` tool accounts for the different physical behaviors of gas expansion versus water incompressibility to provide accurate surface pressure limits.

**Q: Can I calculate wellbore volumes?**
Yes, you can use `get_wellbore_capacity` to calculate both the annular volume and the drill pipe volume based on the provided diameters and total depth.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/kick-tolerance-calculator](https://vinkius.com/en/ai-agent-connect/kick-tolerance-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Kick Tolerance Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `kick-tolerance-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Kick Tolerance Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "kick-tolerance-calculator": {
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
