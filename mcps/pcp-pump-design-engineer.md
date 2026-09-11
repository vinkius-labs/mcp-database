# PCP Pump Design Engineer MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/pcp-pump-design-engineer)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [engineering](../categories/engineering.md)

Design Progressive Cavity Pump systems by calculating rotor/stator configurations, mechanical loads, and material compatibility.

## Description
This MCP server provides specialized engineering tools for designing Progressive Cavity Pump (PCP) systems. It allows AI agents to calculate optimal rotor and stator dimensions using `calculate_pump_configuration`, determine necessary torque and speed with `estimate_mechanical_load`, verify elastomer suitability via `verify_material_compatibility`, and select appropriate surface equipment with `select_drive_head`. It is designed to handle complex variables like fluid viscosity, well depth, and sand content to ensure reliable pump performance in demanding environments.


## Available Tools (4)
- **estimate_mechanical_load**: Calculates the torque and speed necessary to drive the selected pump configuration
- **calculate_pump_configuration**: Determines the optimal rotor and stator dimensions to meet the target fluid rate
- **select_drive_head**: Identifies the appropriate surface drive unit based on the calculated mechanical loads
- **verify_material_compatibility**: Checks if the chosen elastomer can withstand the operating environment


## 💬 Prompt Examples

Here are some examples of how you can interact with the **PCP Pump Design Engineer** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "I need to design a PCP for a well that is 1500 meters deep, with a fluid viscosity of 250 cP and 2% sand content. The target rate is 50 m3/h. What configuration do I need?"

**🤖 AI Agent:**
> For a well depth of 1500m and a target rate of 50 m3/h, the optimal configuration requires a rotor diameter of 85mm and a specific stator geometry to maintain volumetric efficiency at 250 cP.

---

**👤 You:**
> "What is the total torque required for a pump with a 90mm rotor diameter at 1200m depth and 300 cP viscosity for a 40 m3/h rate?"

**🤖 AI Agent:**
> The total torque required is 450 Nm, consisting of 320 Nm of hydraulic torque and 130 Nm of friction torque, with an operating speed of 180 RPM.

---

**👤 You:**
> "Will a standard nitrile elastomer work for a fluid containing crude oil at 85 degrees Celsius with 1% sand?"

**🤖 AI Agent:**
> The nitrile elastomer is compatible with crude oil at 85 degrees Celsius, but ensure the hardness rating is sufficient for the 1% sand content to prevent extrusion.


## ❓ FAQ

**Q: How do I determine the correct pump size for my well?**
You can use the `calculate_pump_configuration` tool. Provide the well depth, fluid viscosity, sand content, and your target production rate to receive the optimal rotor and stator dimensions.

**Q: Can this tool help me select a drive head?**
Yes. After calculating the required torque and speed, use the `select_drive_head` tool to identify a surface unit that meets your mechanical requirements, including a safety factor.

**Q: How does sand content affect the design?**
Sand content is a critical input for both `calculate_pump_configuration` and `verify_material_compatibility`. High sand concentrations influence the required rotor/stator fit and the type of elastomer needed to prevent abrasive wear.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/pcp-pump-design-engineer](https://vinkius.com/en/ai-agent-connect/pcp-pump-design-engineer)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **PCP Pump Design Engineer** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `pcp-pump-design-engineer` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **PCP Pump Design Engineer** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "pcp-pump-design-engineer": {
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
