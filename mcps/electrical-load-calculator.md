# Electrical Load Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/electrical-load-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [construction](../categories/construction.md)

Calculate electrical load per room/circuit, including lighting, receptacles, and appliances for panel sizing.

## Description
The Electrical Load Calculator MCP server provides specialized tools for electrical engineers and professionals to determine circuit requirements and panel capacity. Use `get_lighting_load` to calculate wattage based on room type and area, `calculate_receptacle_load` to estimate VA loads for outlets, `lookup_appliance_impact` to find running and peak power for appliances, and `evaluate_circuit_safety` to check if a circuit exceeds the 80% breaker capacity rule. It also suggests appropriate wire gauge and breaker sizes based on NEC standards.


## Available Tools (4)
- **lookup_appliance_impact**: Retrieves the power requirements for specific fixed appliances
- **evaluate_circuit_safety**: Checks if a circuit is safe for use and recommends hardware
- **calculate_receptacle_load**: Estimates the total VA load for a group of wall outlets
- **get_lighting_load**: g., Kitchen, Bedroom).

Calculates the electrical demand for lighting based on room dimensions and type


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Electrical Load Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Calculate the lighting load for a 200 sq ft Kitchen."

**🤖 AI Agent:**
> The total lighting wattage for a 200 sq ft Kitchen is 400 Watts (based on 2.0 W/sq ft density).

---

**👤 You:**
> "How much VA load should I assume for 10 wall outlets?"

**🤖 AI Agent:**
> The total estimated load for 10 receptacles is 1800 VA.

---

**👤 You:**
> "Check if a 15A breaker at 120V is safe for a 1400W load."

**🤖 AI Agent:**
> The circuit is overloaded. The current draw is 11.67A, which exceeds the 80% safety threshold of 12A (for a 15A breaker).


## ❓ FAQ

**Q: How does the calculator handle lighting loads?**
It uses `get_lighting_load` to apply a power density constant (Watts per Sq Ft) based on the specific room type provided.

**Q: What is the 80% rule used for?**
The `evaluate_circuit_safety` tool checks if the total load exceeds 80% of the breaker's rated capacity to prevent nuisance tripping and handle continuous loads.

**Q: Does it account for appliance startup surges?**
Yes, `lookup_appliance_impact` provides both running watts and peak starting watts to ensure your calculations account for inrush current.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/electrical-load-calculator](https://vinkius.com/mcp/electrical-load-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Electrical Load Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `electrical-load-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Electrical Load Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "electrical-load-calculator": {
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
