# Gas PVT Properties Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/gas-pvt-properties-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [science](../categories/science.md)

Calculate real gas properties like Z-factor, density, and viscosity.

## Description
This MCP server provides high-precision thermodynamic calculations for natural gas. It allows AI agents to determine critical reservoir parameters including the Z-factor, gas density, viscosity, and the gas formation volume factor. By accounting for specific gas compositions and impurities like CO2 and H2S, the tools provide accurate physical modeling for fluid flow and reservoir engineering.


## Available Tools (5)
- **get_gas_compressibility**: Determines the isothermal compressibility of the gas
- **get_gas_density**: Determines the mass per unit volume of the gas at specific reservoir conditions
- **get_gas_formation_volume_factor**: Calculates the ratio of gas volume at standard conditions to volume at reservoir conditions
- **get_gas_viscosity**: Calculates the dynamic viscosity of the gas
- **get_z_factor**: Calculates the compressibility factor (Z) to determine how much the gas deviates from ideal behavior


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Gas PVT Properties Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is the Z-factor for a gas with specific gravity 0.65 at 3000 psi and 150 F?"

**🤖 AI Agent:**
> The calculated Z-factor for the gas at 3000 psi and 150 F is 0.842.

---

**👤 You:**
> "Calculate the gas density for a methane-rich gas (CH4: 0.9, CO2: 0.1) at 2000 psi and 100 F."

**🤖 AI Agent:**
> The gas density at 2000 psi and 100 F is 0.062 lb/ft³.

---

**👤 You:**
> "Find the gas formation volume factor (BoG) at 4000 psi and 200 F, given standard conditions are 14.7 psi and 60 F."

**🤖 AI Agent:**
> The gas formation volume factor (BoG) is 0.00155 res bbl/scf.


## ❓ FAQ

**Q: How do I calculate the Z-factor?**
You can use the `get_z_factor` tool by providing the gas pressure, temperature, and either the specific gravity or a JSON string of the gas composition.

**Q: Does this tool account for impurities?**
Yes, by providing a composition mapping that includes components like CO2 or H2S, the `get_gas_density` and `get_gas_viscosity` tools will factor these impurities into the results.

**Q: What units should I use for pressure?**
The tools support both psi and bar for pressure inputs.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/gas-pvt-properties-calculator](https://vinkius.com/ai-agent-connect/gas-pvt-properties-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Gas PVT Properties Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `gas-pvt-properties-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Gas PVT Properties Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "gas-pvt-properties-calculator": {
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
