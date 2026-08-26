# Pasture Growth Rate Model MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/pasture-growth-rate-model)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [agriculture](../categories/agriculture.md)

Simulate pasture biomass accumulation and grazing capacity based on environmental drivers.

## Description
This MCP server provides tools to model pasture growth by accounting for temperature, soil moisture, solar radiation, and nitrogen application. It allows for calculating daily growth rates, simulating seasonal biomass accumulation curves, predicting livestock grazing capacity, and estimating surplus hay production for different grass types like cool-season and warm-season species. Use `calculate_daily_growth` to find immediate biomass production or `predict_grazing_capacity` to plan livestock stocking rates.


## Available Tools (4)
- **calculate_hay_surplus**: Estimates the amount of biomass available for hay production after grazing needs are satisfied
- **calculate_daily_growth**: Determines the specific biomass accumulation for a single day based on current environmental conditions
- **predict_grazing_capacity**: Determines how many livestock can be sustained by the pasture's annual production
- **simulate_seasonal_growth**: Projects the growth pattern over a specific period to visualize biomass accumulation trends


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Pasture Growth Rate Model** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is the daily growth rate for a cool-season pasture with 25% soil moisture, 20 degrees Celsius, and 15 units of solar radiation?"

**🤖 AI Agent:**
> The daily growth rate for the cool-season pasture is 12.5 kg DM/ha/day.

---

**👤 You:**
> "How many animal units can I support with 5000 kg DM/ha/year of production if each animal needs 15 kg DM/unit/day for 100 days?"

**🤖 AI Agent:**
> The pasture can support 3.33 animal units.

---

**👤 You:**
> "How much hay can I harvest if I produce 4000 kg DM/ha/year and my livestock consume 3200 kg DM/ha/year?"

**🤖 AI Agent:**
> The surplus hay production is 800 kg DM/ha.


## ❓ FAQ

**Q: What grass types are supported?**
The model supports both cool-season and warm-season grass types.

**Q: How is grazing capacity determined?**
You can use `predict_grazing_capacity` to determine how many animal units can be sustained based on annual production and daily animal demand.

**Q: Can I account for nitrogen application?**
Yes, nitrogen application is a supported input that increases the biological growth potential in the simulation.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/pasture-growth-rate-model](https://vinkius.com/ai-agent-connect/pasture-growth-rate-model)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Pasture Growth Rate Model** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `pasture-growth-rate-model` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Pasture Growth Rate Model** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "pasture-growth-rate-model": {
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
