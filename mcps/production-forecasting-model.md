# Production Forecasting Model MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/production-forecasting-model)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [engineering](../categories/engineering.md)

Predict oil and gas production rates using reservoir data and decline curve analysis.

## Description
This MCP server provides specialized engineering tools for oil and gas reservoir management. It allows AI agents to calculate projected production profiles using `forecast_production_profile`, determine the profitability window with `calculate_economic_limit`, and adjust forecasts for physical equipment limits using `apply_facility_constraints`. It also enables sensitivity analysis through `evaluate_well_density_impact` to understand how well spacing affects recovery.


## Available Tools (4)
- **calculate_economic_limit**: Determines when the field will cease to be profitable
- **evaluate_well_density_impact**: Analyzes how changing the number of wells affects the peak production and total recovery
- **forecast_production_profile**: Calculates the projected production rates over a specified time horizon
- **apply_facility_constraints**: Adjusts a theoretical production forecast to account for physical equipment limitations


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Production Forecasting Model** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Forecast production for a reservoir with porosity 0.2, permeability 50, and initial pressure 3000 psi using a water drive for 24 months with 5 wells."

**🤖 AI Agent:**
> The projected monthly production rates for the 24-month period show a peak rate of 1,200 barrels per day, with a total cumulative production of 18,450 barrels.

---

**👤 You:**
> "What is the economic life if my production profile shows 500 barrels per day and my operating cost is $20 per barrel while the market price is $60 per barrel?"

**🤖 AI Agent:**
> The field will remain profitable for 48 months, with an estimated abandonment date of December 2028.

---

**👤 You:**
> "Adjust a production rate of [100, 150, 200, 150] for a facility with a maximum capacity of 120."

**🤖 AI Agent:**
> The constrained production rates are [100, 120, 120, 120].


## ❓ FAQ

**Q: How do I forecast future production?**
You can use the `forecast_production_profile` tool by providing reservoir characteristics, the number of wells, the drive mechanism, and the desired time horizon.

**Q: Can I account for facility limitations?**
Yes, the `apply_facility_constraints` tool allows you to cap theoretical production rates based on the maximum capacity of your equipment.

**Q: How is the economic life of a field determined?**
The `calculate_economic_limit` tool determines the end of profitability by comparing the production profile against operating costs and market prices.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/production-forecasting-model](https://vinkius.com/en/ai-agent-connect/production-forecasting-model)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Production Forecasting Model** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `production-forecasting-model` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Production Forecasting Model** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "production-forecasting-model": {
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
