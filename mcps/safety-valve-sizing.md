# Safety Valve Sizing MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/safety-valve-sizing)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [engineering](../categories/engineering.md)

Calculate SSSV dimensions, flow coefficients, and pressure drops.

## Description
This MCP server provides specialized engineering tools for sizing Subsurface Safety Valves (SSSV). It allows engineers to determine the required `calculate_valve_id` to accommodate specific flow rates, calculate the `calculate_flow_coefficient` for existing valves, and predict energy loss using `calculate_pressure_drop`. It also includes `validate_well_safety_margin` to ensure operating conditions respect erosion velocity and pressure limits.


## Available Tools (4)
- **calculate_flow_coefficient**: Calculates the valve's flow coefficient based on existing physical parameters
- **calculate_pressure_drop**: Predicts the energy loss (pressure reduction) as fluid passes through a valve of a known size
- **calculate_valve_id**: You can optionally provide an erosion velocity limit.

Determines the required internal diameter of the SSSV to accommodate a specific flow rate without exceeding safety limits
- **validate_well_safety_margin**: Checks if the current valve configuration meets safety requirements regarding erosion and pressure limits


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Safety Valve Sizing** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is the required valve ID for a liquid flow of 500 units at 2000 psi upstream?"

**🤖 AI Agent:**
> The required minimum internal diameter is 2.45 inches with an expected velocity of 12.3 ft/s.

---

**👤 You:**
> "Calculate the pressure drop for a 3-inch valve with a flow rate of 1000 and upstream pressure of 3000."

**🤖 AI Agent:**
> The predicted pressure drop is 150 psi, resulting in a downstream pressure of 2850 psi.

---

**👤 You:**
> "Is my current valve configuration safe for a flow rate of 800 and an erosion limit of 50?"

**🤖 AI Agent:**
> Yes, the configuration is safe with a safety margin of 15.2.


## ❓ FAQ

**Q: How do I determine the correct valve size?**
You can use the `calculate_valve_id` tool by providing the flow rate, fluid type, and upstream pressure.

**Q: Can I check for erosion risks?**
Yes, the `validate_well_safety_margin` tool checks if the fluid velocity stays below the specified erosion velocity limit.

**Q: Does it support gas flow calculations?**
Yes, all tools support both gas and liquid flow types, accounting for gas compressibility where necessary.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/safety-valve-sizing](https://vinkius.com/en/ai-agent-connect/safety-valve-sizing)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Safety Valve Sizing** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `safety-valve-sizing` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Safety Valve Sizing** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "safety-valve-sizing": {
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
