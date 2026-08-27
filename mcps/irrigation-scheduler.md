# Irrigation Scheduler MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/irrigation-scheduler)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [agriculture](../categories/agriculture.md)

Calculate precise irrigation needs using the FAO-56 Penman-Monteith model.

## Description
This MCP server provides precise agricultural water management by implementing the FAO-56 Penman-Monteith evapotranspiration model. It allows AI agents to calculate atmospheric water demand via `calculate_et_reference`, determine specific crop requirements with `calculate_crop_demand`, and produce actionable plans using `generate_irrigation_schedule`. You can also monitor plant health by using `check_soil_moisture_status` to identify potential water stress risks based on soil capacity and daily demand.


## Available Tools (4)
- **calculate_crop_demand**: Calculates the specific water requirement for a given crop type and growth stage
- **calculate_et_reference**: Determines the atmospheric water demand (ETo) based on meteorological data
- **check_soil_moisture_status**: Evaluates if a specific soil moisture level is sufficient to sustain the crop until the next scheduled event
- **generate_irrigation_schedule**: Produces the final actionable irrigation plan including depth, timing, and volume


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Irrigation Scheduler** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Calculate the reference evapotranspiration for 25°C, 50% humidity, 2 m/s wind speed, and 15 MJ/m2 solar radiation."

**🤖 AI Agent:**
> The calculated Reference Evapotranspiration (ETo) is 4.2 mm/day.

---

**👤 You:**
> "What is the crop water demand if the ETo is 5 mm/day and the crop coefficient is 0.8?"

**🤖 AI Agent:**
> The total crop evapotranspiration (ETc) is 4.0 mm/day.

---

**👤 You:**
> "Generate an irrigation schedule for a crop needing 5 mm/day, with 2 mm of effective rainfall, 30 mm soil capacity, and 80% efficiency."

**🤖 AI Agent:**
> The required irrigation depth is 4.38 mm, with a suggested frequency of 6 days between irrigations, totaling 26.25 mm³ per unit area.


## ❓ FAQ

**Q: How does this tool calculate water needs?**
It uses the FAO-56 Penman-Monteith method, which balances atmospheric demand (evapotranspiration) against soil water availability and effective rainfall.

**Q: Can I check if my crops are at risk of water stress?**
Yes, by using the `check_soil_moisture_status` tool, you can determine if current soil moisture levels are sufficient to sustain the crop until the next irrigation event.

**Q: What inputs are required for the irrigation schedule?**
To generate a schedule, you need the daily crop water demand (ETc), effective rainfall, soil water holding capacity, and the irrigation system efficiency.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/irrigation-scheduler](https://vinkius.com/ai-agent-connect/irrigation-scheduler)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Irrigation Scheduler** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `irrigation-scheduler` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Irrigation Scheduler** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "irrigation-scheduler": {
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
