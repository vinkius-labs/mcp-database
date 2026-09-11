# Water PVT Properties MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/water-pvt-properties)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [petroleum-engineering](../categories/petroleum-engineering.md)

Calculates physical and thermodynamic properties of formation water.

## Description
This MCP server provides tools to calculate critical PVT properties of formation water. It determines the water formation volume factor, viscosity, compressibility, and gas solubility by accounting for salinity, pressure, and temperature. Use `get_water_viscosity` to find flow resistance or `get_gas_solubility_in_water` to determine gas capacity in brine.


## Available Tools (4)
- **get_gas_solubility_in_water**: Calculates the maximum amount of gas that can be dissolved in the formation water
- **get_water_viscosity**: Calculates the resistance of the formation water to flow
- **get_water_compressibility**: Determines how much the water volume changes per unit of pressure change
- **get_water_formation_volume_factor**: Determines how the volume of water changes from reservoir to standard conditions


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Water PVT Properties** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is the water viscosity at 35000 ppm salinity, 4500 psi, and 200 degrees Fahrenheit?"

**🤖 AI Agent:**
> The water viscosity is 0.324 cP.

---

**👤 You:**
> "Calculate the gas solubility for methane at 50000 ppm, 3000 psi, and 180 degrees Fahrenheit."

**🤖 AI Agent:**
> The gas solubility for methane is 0.0152 scf/cc.

---

**👤 You:**
> "Find the water formation volume factor for 40000 ppm salinity at 5000 psi and 250 degrees Fahrenheit."

**🤖 AI Agent:**
> The water formation volume factor is 1.0045.


## ❓ FAQ

**Q: What properties can be calculated?**
You can calculate the water formation volume factor, viscosity, isothermal compressibility, and gas solubility in water.

**Q: How does salinity affect the results?**
Salinity is a key input that influences density, viscosity, and the 'salting-out' effect on gas solubility.

**Q: Which AI clients are compatible?**
This server is compatible with Cursor, VS Code, Claude Desktop, Windsurf, and any MCP-compatible client via Vinkius Edge.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/water-pvt-properties](https://vinkius.com/ai-agent-connect/water-pvt-properties)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Water PVT Properties** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `water-pvt-properties` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Water PVT Properties** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "water-pvt-properties": {
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
