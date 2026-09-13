# Tank Heating System Design MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/tank-heating-system-design)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [engineering](../categories/engineering.md)

Engineering tool for heavy oil tank heating and heat duty calculations.

## Description
This MCP server provides specialized engineering tools for designing heating systems for heavy oil storage tanks. It allows users to calculate the total heat duty required to reach target temperatures, select the most efficient heater type (such as internal coils or external heating), and estimate steam consumption based on latent heat. Additionally, it includes a validation tool to ensure that the heating parameters successfully reach the required viscosity target for fluid mobility.


## Available Tools (4)
- **calculate_steam_consumption**: Estimates the amount of steam needed to satisfy the calculated heat duty
- **get_heat_duty**: Calculates the total thermal energy required to heat the oil and compensate for heat losses
- **select_heater_type**: Determines the most appropriate heating configuration based on tank geometry and oil properties
- **validate_viscosity_target**: Verifies if the proposed heating parameters will achieve the necessary fluid mobility


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Tank Heating System Design** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is the total heat duty for 500 cubic meters of oil with a density of 950 kg/m3, moving from 20C to 60C, with a specific heat of 2000 J/kgK and a loss coefficient of 5?"

**🤖 AI Agent:**
> The total heat duty is 40,000,000 J and the net heat duty is 40,005,000 J.

---

**👤 You:**
> "Which heater is best for a tank 10m wide and 15m high with an oil viscosity of 500 cP at target temperature?"

**🤖 AI Agent:**
> The recommended heater type is internal coils with a suitability score of 0.85.

---

**👤 You:**
> "Will a temperature of 50C be enough to reach a target viscosity of 100 cP if the current viscosity is 500 cP?"

**🤖 AI Agent:**
> Yes, the target viscosity is met.


## ❓ FAQ

**Q: How do I calculate the energy needed for my tank?**
You can use the `get_heat_duty` tool by providing the oil density, volume, temperatures, and heat loss coefficient.

**Q: Can this tool help me choose between coils and external heating?**
Yes, the `select_heater_type` tool analyzes tank dimensions and oil viscosity to recommend the best configuration.

**Q: How is steam usage estimated?**
The `calculate_steam_consumption` tool estimates steam mass flow and total usage based on the required heat duty and steam latent heat.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/tank-heating-system-design](https://vinkius.com/en/ai-agent-connect/tank-heating-system-design)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Tank Heating System Design** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `tank-heating-system-design` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Tank Heating System Design** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "tank-heating-system-design": {
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
