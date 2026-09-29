# EV Charging Stop Planner MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/ev-charging-stop-planner)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [transportation](../categories/transportation.md)

Calculates optimal charging stops for electric vehicle routes.

## Description
This MCP server provides tools to plan efficient electric vehicle journeys. It calculates an ordered sequence of charging stops using `plan_charging_stops`, ensuring the vehicle always maintains its `requiredReserve`. You can also use `get_charger_details` to find pricing and power rates, `validate_connector_compatibility` to check plug types, and `calculate_stop_duration` to estimate time spent at a station.


## Available Tools (4)
- **validate_connector_compatibility**: Verifies if a specific vehicle can use a specific charger
- **calculate_stop_duration**: Determines how long a vehicle must stay at a charger to reach a target energy level
- **get_charger_details**: Retrieves specific capability and pricing information for a single charging station
- **plan_charging_stops**: Calculates an ordered sequence of charging stops for a specific journey


## 💬 Prompt Examples

Here are some examples of how you can interact with the **EV Charging Stop Planner** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Plan a trip with 50kWh initial SoC, 75kWh capacity, 10kWh reserve, and these legs: [{'distanceKm': 100, 'energyRequiredKwh': 20}, {'distanceKm': 150, 'energyRequiredKwh': 30}]. Here are the chargers: [{'chargerId': 'C1', 'connectorTypes': ['CCS'], 'maxRateKw': 50, 'pricePerKwh': 0.3}]. My connector is CCS."

**🤖 AI Agent:**
> Your optimal stop is at charger C1. You will add 20kWh of energy, which will cost $6.00, and arrive at your destination with 20kWh remaining.

---

**👤 You:**
> "How long will it take to add 30kWh if the charger provides 60kW and efficiency is 0.9?"

**🤖 AI Agent:**
> It will take approximately 33.33 minutes to complete the charge.

---

**👤 You:**
> "Is a NACS connector compatible with a charger that has ['CCS', 'CHAdeMO']?"

**🤖 AI Agent:**
> No, the NACS connector is not compatible with the available connector types.


## ❓ FAQ

**Q: How does the planner ensure I don't run out of battery?**
The `plan_charging_stops` tool uses a mandatory `requiredReserve` parameter to ensure the battery level never drops below your specified safety threshold.

**Q: Can I check if a specific charger works with my car?**
Yes, you can use the `validate_connector_compatibility` tool to compare your vehicle's connector type against the available options at a station.

**Q: Does the tool account for charging speed?**
Yes, the system considers the effective charging rate and efficiency when calculating how long you will need to stay at a stop using `calculate_stop_duration`.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/ev-charging-stop-planner](https://vinkius.com/en/ai-agent-connect/ev-charging-stop-planner)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **EV Charging Stop Planner** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `ev-charging-stop-planner` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **EV Charging Stop Planner** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "ev-charging-stop-planner": {
      "url": "https://edge.vinkius.com/[TOKEN]/mcp"
    }
  }
}
```

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius connector registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
