# Thermal Mass Estimator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/thermal-mass-estimator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [construction](../categories/construction.md)

Calculate thermal lag, amplitude damping, and U-value for wall structures based on material properties.

## Description
This MCP server provides specialized tools to quantify the thermal performance of building envelopes. Use `get_material_properties` to retrieve conductivity, density, and specific heat for materials like brick or concrete. Use `calculate_u_value` to determine thermal transmittance based on wall thickness. You can also use `estimate_thermal_behavior` to project how much temperature fluctuations are reduced (damping) and the time delay (lag) of heat moving through a structure.


## Available Tools (3)
- **calculate_u_value**: Calculates the thermal transmittance (U-value) for a single layer of material
- **estimate_thermal_behavior**: Estimates the thermal lag and amplitude damping factor for a wall layer
- **get_material_properties**: Retrieves the fundamental thermal properties for a specific building material


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Thermal Mass Estimator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What are the thermal properties of concrete?"

**🤖 AI Agent:**
> The `get_material_properties` tool shows that concrete has a specific conductivity, density, and specific heat capacity.

---

**👤 You:**
> "Calculate the U-value for a 0.2m brick wall."

**🤖 AI Agent:**
> Using `calculate_u_value` with thickness 0.2 and material 'brick', the tool returns the calculated thermal transmittance.

---

**👤 You:**
> "Estimate the thermal behavior of a 0.1m wood layer."

**🤖 AI Agent:**
> The `estimate_thermal_behavior` tool provides the estimated thermal lag in hours and the damping factor for this thickness.


## ❓ FAQ

**Q: What materials are supported?**
The server currently supports brick, concrete, wood, and drywall.

**Q: How is the U-value calculated?**
The U-value is calculated as the ratio of the material's thermal conductivity to its thickness in meters.

**Q: What does thermal lag represent?**
Thermal lag represents the time interval between peak external temperature and peak internal temperature.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/thermal-mass-estimator](https://vinkius.com/mcp/thermal-mass-estimator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Thermal Mass Estimator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `thermal-mass-estimator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Thermal Mass Estimator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "thermal-mass-estimator": {
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
