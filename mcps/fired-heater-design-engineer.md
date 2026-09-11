# Fired Heater Design Engineer MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/fired-heater-design-engineer)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [engineering](../categories/engineering.md)

Professional engineering tool for sizing radiant sections, tube coils, and calculating fuel efficiency for industrial fired heaters.

## Description
This MCP server provides specialized engineering calculations for industrial fired heater design. It allows AI agents to perform complex thermal modeling, including sizing the radiant section using `get_radiant_section_sizing`, designing tube coil configurations with `get_tube_coil_design`, predicting stack exit temperatures via `get_stack_temperature_and_losses`, and estimating fuel requirements through `get_fuel_consumption`. It is designed to handle heating duty, fluid properties, and fuel composition to ensure accurate equipment sizing and efficiency targets.


## Available Tools (4)
- **get_fuel_consumption**: Estimates the total mass or volume of fuel required to meet the heating demand
- **get_radiant_section_sizing**: Determines the physical dimensions required for the radiant section to achieve the necessary heat transfer
- **get_stack_temperature_and_losses**: Predicts the temperature of the flue gas exiting the stack and calculates energy lost to the environment
- **get_tube_coil_design**: Calculates the physical configuration and number of tubes needed for the heating coils


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Fired Heater Design Engineer** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Calculate the radiant section size for a heating duty of 50 MW with a specific fluid and fuel profile."

**🤖 AI Agent:**
> The required radiant section volume is 1250 m³, with a tube surface area of 450 m² and an estimated height of 12 meters.

---

**👤 You:**
> "What will be the stack temperature if I use a 15% excess air ratio?"

**🤖 AI Agent:**
> The predicted stack exit temperature is 185°C with a flue gas volume flow of 4500 m³/h.

---

**👤 You:**
> "Estimate the fuel consumption for a 25 MW duty at 85% efficiency."

**🤖 AI Agent:**
> The estimated fuel mass flow rate is 420 kg/h based on the provided fuel composition.


## ❓ FAQ

**Q: What can I calculate with this tool?**
You can calculate radiant section dimensions, tube coil geometry, stack exit temperatures, heat losses, and total fuel consumption.

**Q: How do I provide fluid properties?**
Fluid properties should be provided as a JSON string containing heatCapacity, density, and viscosity.

**Q: Does this tool account for efficiency targets?**
Yes, the efficiency target is a required input for sizing and fuel consumption calculations to ensure the design meets specific performance goals.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/fired-heater-design-engineer](https://vinkius.com/en/ai-agent-connect/fired-heater-design-engineer)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Fired Heater Design Engineer** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `fired-heater-design-engineer` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Fired Heater Design Engineer** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "fired-heater-design-engineer": {
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
