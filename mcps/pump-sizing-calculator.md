# Pump Sizing Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/pump-sizing-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [engineering](../categories/engineering.md)

Professional engineering tool for pump sizing, power calculation, and cavitation safety analysis.

## Description
This MCP server provides essential engineering tools for fluid transport system design. It allows AI agents to calculate the exact operating point where a pump meets system resistance using `pump_calculate_operating_point`. Engineers can determine electrical and mechanical requirements via `pump_calculate_power_requirements`, evaluate safety against cavitation using `pump_check_cavitation_risk`, and predict performance changes under different hardware configurations with `pump_apply_affinity_laws`.


## Available Tools (4)
- **pump_apply_affinity_laws**: Predict how changing the pump hardware (impeller size) or speed will impact performance
- **pump_calculate_operating_point**: Determine the specific operating conditions where the pump performance meets the system resistance
- **pump_calculate_power_requirements**: Determine the electrical and mechanical power needed to drive the pump at a specific operating point
- **pump_check_cavitation_risk**: Evaluate if the current system configuration will cause cavitation damage


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Pump Sizing Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Calculate the power required for a pump with 50 m3/h flow, 30m head, fluid density of 1000 kg/m3, and 75% efficiency."

**🤖 AI Agent:**
> The required power is 4.31 kW (5.78 HP) with a shaft torque of 145.2 Nm.

---

**👤 You:**
> "Is it safe to run a pump with 5m NPSH available and 4.5m NPSH required, assuming a 0.5m safety margin?"

**🤖 AI Agent:**
> No, the system is not safe. The available margin is 0.5m, which does not exceed the required safety margin.

---

**👤 You:**
> "If I increase the impeller diameter by 10%, what happens to the flow and head?"

**🤖 AI Agent:**
> With a diameter ratio of 1.1, the predicted flow increases by 10% and the head increases by 21%.


## ❓ FAQ

**Q: How do I find the operating point of my pump?**
You can use the `pump_calculate_operating_point` tool by providing the target flow rate and the JSON-formatted system and pump curves.

**Q: Can this tool help prevent pump damage?**
Yes, the `pump_check_cavitation_risk` tool evaluates the margin between available and required NPSH to ensure the system operates safely without cavitation.

**Q: How do I calculate the power needed for a specific flow?**
Use the `pump_calculate_power_requirements` tool with the operating flow, head, fluid density, and pump efficiency to get brake horsepower and kilowatts.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/pump-sizing-calculator](https://vinkius.com/ai-agent-connect/pump-sizing-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Pump Sizing Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `pump-sizing-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Pump Sizing Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "pump-sizing-calculator": {
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
