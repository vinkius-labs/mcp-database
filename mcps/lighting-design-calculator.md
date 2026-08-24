# Lighting Design Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/lighting-design-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [design](../categories/design.md)

Deterministic lighting design tool for calculating illuminance, spacing, and energy usage.

## Description
A professional-grade tool for lighting designers to calculate precise lighting requirements. Use `get_design_validation` to verify if a setup meets target lux levels for offices, kitchens, or living rooms. You can also use `get_room_index_data` to determine the Coefficient of Utilization (CU) based on room geometry and surface reflectances, or `calculate_energy_profile` to estimate annual energy consumption and total wattage.


## Available Tools (3)
- **calculate_energy_profile**: Calculates the electrical impact of the lighting design
- **get_design_validation**: Validates if a proposed lighting setup meets the target illuminance requirements for a specific room type
- **get_room_index_data**: Provides the calculated Room Index and Coefficient of Utilization (CU) for a specific room geometry and surface set


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Lighting Design Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Validate a lighting setup for a 5x5x3 meter office with 4 fixtures of 3000 lumens each and 70% ceiling reflectance."

**🤖 AI Agent:**
> The calculated average illuminance is 540 lux, which meets the 500 lux requirement for an office.

---

**👤 You:**
> "Calculate the annual energy consumption for 10 LED fixtures, each using 15 watts, running for 2500 hours per year."

**🤖 AI Agent:**
> The total wattage is 150W and the annual energy consumption is 375 kWh.

---

**👤 You:**
> "What is the room index for a room that is 6 meters long, 4 meters wide, and 3 meters high?"

**🤖 AI Agent:**
> The calculated Room Index for these dimensions is 1.25.


## ❓ FAQ

**Q: How do I verify if my office lighting is sufficient?**
You can use the `get_design_validation` tool by providing the room dimensions, task type (office), fixture flux, and surface reflectances to see if the average illuminance meets the 500 lux requirement.

**Q: Can I calculate the energy cost of my lighting setup?**
Yes, use the `calculate_energy_profile` tool with the number of fixtures, wattage per fixture, and annual operating hours to get the total wattage and annual kWh.

**Q: What determines the Coefficient of Utilization (CU)?**
The CU is determined by the room's geometry and the reflectances of the surfaces. You can find these values using the `get_room_index_data` tool.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/lighting-design-calculator](https://vinkius.com/ai-agent-connect/lighting-design-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Lighting Design Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `lighting-design-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Lighting Design Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "lighting-design-calculator": {
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
