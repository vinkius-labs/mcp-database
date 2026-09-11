# CO2 Emission Tracker MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/co2-emission-tracker)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [energy](../categories/energy.md)

Quantify Scope 1, 2, and 3 emissions and carbon intensity for oil and gas operations.

## Description
This MCP server provides specialized tools for quantifying carbon dioxide emissions in the oil and gas sector. It adheres to international reporting standards to calculate Scope 1, 2, and 3 emissions. Users can determine their total net carbon footprint by applying `calculate_net_carbon_footprint` to account for CO2 reinjection credits, and measure production efficiency using `calculate_emission_intensity`. The engine uses IPCC-aligned emission factors to convert fuel consumption, process venting, and flaring into precise mass units of CO2.


## Available Tools (5)
- **calculate_emission_intensity**: Calculate carbon emission intensity relative to production volume
- **calculate_scope_1_emissions**: Calculate total direct Scope 1 emissions from fuel, vents, and flaring
- **calculate_net_carbon_footprint**: Calculate total net carbon footprint after accounting for sequestration
- **calculate_scope_2_emissions**: Calculate total indirect Scope 2 emissions from purchased energy
- **calculate_scope_3_emissions**: Calculate total indirect Scope 3 emissions from value chain activities


## 💬 Prompt Examples

Here are some examples of how you can interact with the **CO2 Emission Tracker** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What are my total direct Scope 1 emissions if I used 500 units of fuel, had 50 units of process venting, and 20 units of flaring?"

**🤖 AI Agent:**
> The total direct Scope 1 emissions are 450.5 kg of CO2.

---

**👤 You:**
> "Calculate my net carbon footprint with Scope 1 of 1000, Scope 2 of 500, Scope 3 of 300, and 200 units of CO2 reinjection."

**🤖 AI Agent:**
> Your gross emissions are 1800 and your net emissions are 1600.

---

**👤 You:**
> "What is the emission intensity for a net footprint of 5000 and a production volume of 10000 barrels?"

**🤖 AI Agent:**
> The emission intensity is 0.5 units of CO2 per barrel.


## ❓ FAQ

**Q: How are Scope 1 emissions calculated?**
Scope 1 emissions are calculated by summing the emissions from fuel consumption, process venting, and flaring, each multiplied by its specific IPCC-aligned emission factor via the `calculate_scope_1_emissions` tool.

**Q: Can I account for CO2 sequestration?**
Yes. You can use `calculate_net_carbon_footprint` and provide the `reinjectionVolume` to subtract sequestered CO2 from your gross emissions.

**Q: What is emission intensity?**
Emission intensity is the ratio of total net emissions to the total production volume. You can calculate this using the `calculate_emission_intensity` tool.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/co2-emission-tracker](https://vinkius.com/en/ai-agent-connect/co2-emission-tracker)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **CO2 Emission Tracker** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `co2-emission-tracker` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **CO2 Emission Tracker** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "co2-emission-tracker": {
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
