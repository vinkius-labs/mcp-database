# Cooling Tower Sizing Utility MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/cooling-tower-sizing-utility)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [engineering](../categories/engineering.md)

Thermodynamic sizing and water balance calculations for industrial cooling towers.

## Description
This MCP server provides professional engineering tools to design and analyze cooling tower performance. Use `calculate_tower_dimensions` to determine physical tower size and air flow requirements based on heat load and wet bulb temperature. Use `estimate_water_balance` to calculate necessary makeup water and system losses. You can also use `validate_cooling_constraints` to check if a temperature profile is physically achievable and `get_tower_efficiency_metrics` to evaluate thermal effectiveness.


## Available Tools (4)
- **estimate_water_balance**: Estimates the water balance for the cooling tower system
- **calculate_tower_dimensions**: Calculates the required dimensions and air flow for a cooling tower
- **validate_cooling_constraints**: Validates if the proposed cooling profile meets hardware constraints
- **get_tower_efficiency_metrics**: Calculates efficiency metrics for the cooling tower


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Cooling Tower Sizing Utility** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What size tower do I need for a 5000 kW heat load with a wet bulb of 25°C, an approach of 5°C, and a circulation rate of 100 kg/s?"

**🤖 AI Agent:**
> The required cooling tower has a diameter of 4.5 meters, a height of 6.2 meters, a cooling range of 15°C, and requires an air flow of 120 m³/s.

---

**👤 You:**
> "Is it possible to reach a water temperature of 28°C if the wet bulb is 26°C and my minimum approach is 2°C?"

**🤖 AI Agent:**
> No, the proposed profile is not feasible because the calculated approach is only 2°C, which does not meet the minimum required approach of 2°C when considering precision limits.

---

**👤 You:**
> "Calculate the water balance if evaporation is 0.5 kg/s and blowdown is 0.1 kg/s."

**🤖 AI Agent:**
> The total makeup water required is 0.6 kg/s, with total system losses of 0.6 kg/s.


## ❓ FAQ

**Q: How do I determine the physical size of my tower?**
You can use the `calculate_tower_dimensions` tool by providing the heat load, wet bulb temperature, approach temperature, and circulation rate.

**Q: Can I check if my cooling target is realistic?**
Yes, the `validate_cooling_constraints` tool allows you to verify if a target water temperature is feasible given the ambient wet bulb temperature and hardware limits.

**Q: How much makeup water will I need?**
Use the `estimate_water_balance` tool with your evaporation and blowdown rates to find the total required makeup water.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/cooling-tower-sizing-utility](https://vinkius.com/en/ai-agent-connect/cooling-tower-sizing-utility)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Cooling Tower Sizing Utility** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `cooling-tower-sizing-utility` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Cooling Tower Sizing Utility** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "cooling-tower-sizing-utility": {
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
