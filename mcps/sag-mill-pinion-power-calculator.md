# SAG Mill Pinion Power Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/sag-mill-pinion-power-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [engineering](../categories/engineering.md)

Calculate mechanical and electrical power requirements for SAG mill pinions.

## Description
This MCP server provides specialized engineering tools to calculate the power requirements for Semi-Autogenous Grinding (SAG) mill pinions. It allows AI agents to determine the mechanical `calculate_pinion_power` needed based on mill geometry and ore characteristics, calculate the total electrical `calculate_motor_power` required, and assess `calculate_power_utilization` relative to motor capacity. Additionally, it can `analyze_slurry_impact` to understand how changes in slurry density affect power draw.


## Available Tools (4)
- **analyze_slurry_impact**: Evaluates how the density of the slurry affects the overall power requirements
- **calculate_motor_power**: Determines the total electrical motor power required to drive the pinion
- **calculate_pinion_power**: Determines the mechanical power required at the pinion to rotate the mill under specific loading conditions
- **calculate_power_utilization**: Measures how effectively the installed motor is being used relative to its rated capacity


## 💬 Prompt Examples

Here are some examples of how you can interact with the **SAG Mill Pinion Power Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Calculate the pinion power for a mill with 5m diameter, 15m length, 75% critical speed, 25% charge level, 2.5 ore density, and a standard liner profile."

**🤖 AI Agent:**
> The calculated pinion power is 1250.5 kW with a total charge mass of 450 metric tons.

---

**👤 You:**
> "What is the motor power required if the pinion power is 1000 kW, transmission efficiency is 0.95, and motor efficiency is 0.98?"

**🤖 AI Agent:**
> The total electrical motor power required is 1097.46 kW.

---

**👤 You:**
> "How much motor capacity is being used if the motor power is 800 kW and the rated capacity is 1000 kW?"

**🤖 AI Agent:**
> The motor is currently at 80% utilization.


## ❓ FAQ

**Q: What inputs are needed for pinion power calculation?**
You need the mill diameter, length, rotational speed (as % of critical speed), charge level, ore density, and the liner profile type.

**Q: How does slurry density affect power?**
Changes in slurry density alter the total mass being moved, which directly impacts the required pinion power.

**Q: Can I calculate motor efficiency losses?**
Yes, by using the motor power tool, you can account for both transmission and motor efficiency to find the total electrical demand.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/sag-mill-pinion-power-calculator](https://vinkius.com/ai-agent-connect/sag-mill-pinion-power-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **SAG Mill Pinion Power Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `sag-mill-pinion-power-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **SAG Mill Pinion Power Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "sag-mill-pinion-power-calculator": {
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
