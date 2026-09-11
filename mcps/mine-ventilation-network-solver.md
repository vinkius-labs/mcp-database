# Mine Ventilation Network Solver MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/mine-ventilation-network-solver)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [engineering](../categories/engineering.md)

Simulate airflows, pressures, and fan operating points in underground mine ventilation networks.

## Description
This MCP server provides a professional-grade simulation engine for underground mine ventilation. It uses the Hardy Cross method to calculate steady-state airflows and pressures across complex network topologies. Users can determine specific fan operating points, calculate airway resistance based on physical dimensions, and validate network integrity. The solver accounts for natural ventilation pressure (NVP) to ensure accurate hydraulic balancing of the entire circuit.


## Available Tools (4)
- **get_airway_resistance_profile**: Calculates the resistance of specific airways based on physical dimensions
- **calculate_fan_operating_points**: Determines the specific state (pressure and quantity) at which a fan will operate given a specific network resistance
- **solve_network_flow**: Performs the core iterative calculation to find the steady-state airflows and pressures across the entire mine network
- **validate_network_topology**: Checks the integrity of the provided mine geometry before simulation


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Mine Ventilation Network Solver** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Calculate the resistance for an airway that is 100m long, has an area of 15m2, a perimeter of 16m, and a roughness coefficient of 0.02."

**🤖 AI Agent:**
> The calculated resistance for the specified airway is 0.045.

---

**👤 You:**
> "Check if my mine network geometry is valid for simulation."

**🤖 AI Agent:**
> The network topology is valid and ready for simulation.

---

**👤 You:**
> "Find the operating point for a fan with the following curve: [{'p': 1000, 'q': 50}, {'p': 800, 'q': 70}] and a system resistance of {'r': 0.5}."

**🤖 AI Agent:**
> The fan will operate at a pressure of 850 and a quantity of 65.


## ❓ FAQ

**Q: How does the solver handle network balancing?**
The engine uses the `solve_network_flow` tool to perform iterative calculations using the Hardy Cross method, ensuring flow continuity and pressure balance.

**Q: Can I calculate resistance for specific tunnels?**
Yes, you can use `get_airway_resistance_profile` to calculate resistance based on length, area, perimeter, and roughness.

**Q: Does it support natural ventilation pressure?**
Yes, the `solve_network_flow` tool allows for an optional NVP distribution to be applied to the network.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/mine-ventilation-network-solver](https://vinkius.com/en/ai-agent-connect/mine-ventilation-network-solver)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Mine Ventilation Network Solver** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `mine-ventilation-network-solver` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Mine Ventilation Network Solver** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "mine-ventilation-network-solver": {
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
