# Dewatering Flow Rate Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/dewatering-flow-rate-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [construction](../categories/construction.md)

Calculate hydraulic requirements, well configurations, and pump needs for groundwater dewatering.

## Description
This MCP server provides essential geotechnical tools for managing groundwater during excavation. It allows AI agents to calculate the total water volume to be removed using `calculate_flow_rate`, determine the physical layout of wells with `calculate_well_configuration`, and specify mechanical equipment needs via `calculate_pump_requirements`. It also includes `evaluate_boundary_impact` to adjust flow rates based on environmental constraints like nearby rivers.


## Available Tools (4)
- **calculate_pump_requirements**: Determines the mechanical pump equipment necessary to move the calculated flow
- **calculate_well_configuration**: Determines the number of wells needed and how far apart they should be placed
- **evaluate_boundary_impact**: Adjusts the expected flow rate based on environmental constraints like nearby water bodies
- **calculate_flow_rate**: Determines the total volume of water that must be removed per minute to achieve the target drawdown


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Dewatering Flow Rate Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Calculate the flow rate for an excavation 50m long, 30m wide, with a groundwater level of 10m, a required drawdown of 5m, permeability of 0.0001 m/s, and a radius of influence of 100m."

**🤖 AI Agent:**
> The calculated total flow rate is 1,250 L/min, with a theoretical drawdown of 5.0m and a total water volume removed of 450 cubic meters.

---

**👤 You:**
> "I need to know how many wells to install for a flow rate of 500 L/min if each well has a capacity of 150 L/min and the excavation perimeter is 200m."

**🤖 AI Agent:**
> You will need 4 wells, which will be spaced 50 meters apart along the perimeter, providing a redundancy factor of 1.2.

---

**👤 You:**
> "How many pumps are required for a flow of 1000 L/min if each pump handles 400 L/min and I want a 20% safety margin?"

**🤖 AI Agent:**
> You will need 3 pumps, providing a total capacity of 1200 L/min with a 83.3% utilization rate.


## ❓ FAQ

**Q: How do I calculate the total water flow needed?**
Use the `calculate_flow_rate` tool by providing the excavation dimensions, soil permeability, and required drawdown.

**Q: Can I account for nearby rivers in my calculations?**
Yes, use the `evaluate_boundary_impact` tool to adjust your flow rate if the excavation is near a constant-head boundary.

**Q: How many pumps will I need for my site?**
You can determine the exact number of pumps required by using the `calculate_pump_requirements` tool with your calculated flow rate and pump capacity.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/dewatering-flow-rate-calculator](https://vinkius.com/ai-agent-connect/dewatering-flow-rate-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Dewatering Flow Rate Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `dewatering-flow-rate-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Dewatering Flow Rate Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "dewatering-flow-rate-calculator": {
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
