# Viscosity Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/viscosity-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [science](../categories/science.md)

Compute viscosity, relative viscosity, and activation energy for pure liquids and solutions.

## Description
This MCP server provides specialized computational tools for fluid dynamics analysis. It allows AI agents to determine the viscosity of pure liquids using `calculate_pure_liquid_viscosity`, predict suspension viscosity via the Einstein model with `calculate_dilute_suspension_viscosity`, and model electrolyte solutions using the Jones-Dole method with `calculate_electrolyte_solution_viscosity`. Additionally, it can determine the activation energy for flow using `analyze_viscosity_temperature_sensitivity`.


## Available Tools (4)
- **analyze_viscosity_temperature_sensitivity**: Calculates the activation energy required for flow based on viscosity measurements at two different temperatures
- **calculate_dilute_suspension_viscosity**: Predicts the viscosity of a dilute suspension based on particle volume fraction
- **calculate_electrolyte_solution_viscosity**: Calculates the viscosity of a solution containing ions (electrolytes) using concentration data
- **calculate_pure_liquid_viscosity**: Determines the viscosity of a single pure liquid at a specific temperature


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Viscosity Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is the viscosity of water at 298.15 Kelvin?"

**🤖 AI Agent:**
> The viscosity of water at 298.15 K is approximately 0.89 mPa·s.

---

**👤 You:**
> "Calculate the viscosity of a dilute suspension with a solvent viscosity of 1.0 mPa·s and a volume fraction of 0.05 at 300 K."

**🤖 AI Agent:**
> The absolute viscosity of the suspension is 1.05 mPa·s, with a relative viscosity of 1.05.

---

**👤 You:**
> "Find the activation energy if viscosity is 1.0 mPa·s at 300 K and 0.5 mPa·s at 350 K."

**🤖 AI Agent:**
> The calculated activation energy for flow is approximately 15.3 kJ/mol.


## ❓ FAQ

**Q: What models are used for viscosity calculations?**
The server uses the Einstein model for dilute suspensions and the Jones-Dole model for electrolyte solutions.

**Q: Can I calculate activation energy?**
Yes, you can use `analyze_viscosity_temperature_sensitivity` to find the activation energy required for flow based on two temperature measurements.

**Q: What units are used for temperature?**
All temperature inputs must be provided in Kelvin.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/viscosity-calculator](https://vinkius.com/ai-agent-connect/viscosity-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Viscosity Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `viscosity-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Viscosity Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "viscosity-calculator": {
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
