# Groundwater Recharge Estimator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/groundwater-recharge-estimator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [environmental-science](../categories/environmental-science.md)

Estimates groundwater recharge and well yield impacts using water balance and mass balance methods.

## Description
This MCP server provides specialized tools for hydrological modeling. It allows AI agents to calculate groundwater recharge using the `calculate_water_balance` method or the `calculate_chloride_mass_balance` approach. Users can also predict how changes in water levels affect local resources with `estimate_well_yield_impact` and refine estimates based on environmental factors using `analyze_soil_vegetation_interaction`.


## Available Tools (4)
- **analyze_soil_vegetation_interaction**: Modifies recharge expectations based on specific soil types and plant characteristics
- **calculate_chloride_mass_balance**: Estimates recharge using chloride concentration ratios
- **calculate_water_balance**: Estimates recharge based on the volumetric water balance approach
- **estimate_well_yield_impact**: Predicts how changes in recharge will affect water availability for extraction


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Groundwater Recharge Estimator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Calculate the annual recharge if precipitation is 1200mm, ET is 500mm, soil capacity is 300mm, and rooting depth is 500mm."

**🤖 AI Agent:**
> The estimated annual recharge is 700 mm, with a recharge coefficient of 58.33%.

---

**👤 You:**
> "What is the impact on well yield if current recharge is 500mm and projected recharge drops to 400mm with an extraction rate of 1000 cubic meters?"

**🤖 AI Agent:**
> The projected yield change is a 20% decrease, and the water availability status is declining.

---

**👤 You:**
> "Estimate recharge using chloride mass balance with 5 mg/L in rain, 0.5 mg/L in groundwater, and 1000mm precipitation."

**🤖 AI Agent:**
> The estimated annual recharge is 100 mm, representing a 10% recharge coefficient.


## ❓ FAQ

**Q: What methods are used for recharge estimation?**
The server uses the volumetric water balance method via `calculate_water_balance` and the chloride mass balance method via `calculate_chloride_mass_balance`.

**Q: Can I predict the impact on my local well?**
Yes, you can use `estimate_well_yield_impact` to see how changes in annual recharge will affect the volume of water available for extraction.

**Q: How do soil and plants affect the results?**
The `analyze_soil_vegetation_interaction` tool adjusts recharge estimates by accounting for soil texture and the density of vegetation.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/groundwater-recharge-estimator](https://vinkius.com/ai-agent-connect/groundwater-recharge-estimator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Groundwater Recharge Estimator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `groundwater-recharge-estimator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Groundwater Recharge Estimator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "groundwater-recharge-estimator": {
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
