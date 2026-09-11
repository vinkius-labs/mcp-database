# ESP Sizing & Configuration MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/esp-sizing-configuration)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [engineering](../categories/engineering.md)

Calculates optimal electric submersible pump (ESP) configurations, including pump stages, motor size, and electrical systems.

## Description
This MCP server provides specialized engineering tools for sizing electric submersible pump (ESP) systems. It uses Nodal Analysis to find the equilibrium between reservoir delivery and system requirements via `get_operating_point`. Once the operating point is established, `calculate_pump_configuration` determines the necessary pump stages and models, accounting for viscosity derating and gas handling. The `select_electrical_system` tool selects the appropriate motor, cable, and VFD requirements based on depth and load. Finally, `validate_system_feasibility` ensures the entire configuration meets wellbore geometry and safety constraints.


## Available Tools (4)
- **get_operating_point**: Determines the equilibrium state where the reservoir delivery meets the system lifting requirements
- **calculate_pump_configuration**: Determines the physical hardware requirements for the pump unit
- **select_electrical_system**: Determines the motor, cable, and surface control requirements
- **validate_system_feasibility**: Checks the entire configuration against safety and operational constraints


## 💬 Prompt Examples

Here are some examples of how you can interact with the **ESP Sizing & Configuration** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Find the operating point for a well with an inflow performance of 'IPR_001' and a system head curve of 'SHC_99'."

**🤖 AI Agent:**
> The equilibrium production rate is 1,250 barrels per day with a total dynamic head of 4,500 feet.

---

**👤 You:**
> "Calculate the pump configuration for a target flow rate of 2000 bpd, 5000 ft head, 50 cP viscosity, and 5% gas."

**🤖 AI Agent:**
> The required configuration is 142 stages of the High-Efficiency Model X, with an efficiency derating factor of 0.88.

---

**👤 You:**
> "Select the electrical system for a 250 HP motor at 8,000 ft depth with a fluid density of 0.85 spgr."

**🤖 AI Agent:**
> The recommended setup is a 450V motor with #4 AWG heavy-duty cable, and a VFD is required for startup torque management.


## ❓ FAQ

**Q: How does the tool handle high-viscosity fluids?**
The `calculate_pump_configuration` tool applies a viscosity derating factor to the pump performance curves to ensure the selected hardware can handle the increased resistance.

**Q: Can I validate if my pump fits in the wellbore?**
Yes, use the `validate_system_feasibility` tool. It checks the pump diameter and electrical system against the provided wellbore geometry and constraints.

**Q: What information is needed to find the operating point?**
You need to provide the inflow performance description and the system head curve description to the `get_operating_point` tool.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/esp-sizing-configuration](https://vinkius.com/en/ai-agent-connect/esp-sizing-configuration)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **ESP Sizing & Configuration** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `esp-sizing-configuration` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **ESP Sizing & Configuration** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "esp-sizing-configuration": {
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
