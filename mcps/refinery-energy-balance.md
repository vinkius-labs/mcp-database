# Refinery Energy Balance MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/refinery-energy-balance)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [optimization](../categories/optimization.md)

Audit and optimize refinery energy consumption and efficiency.

## Description
This MCP server provides specialized calculation engines to audit refinery energy consumption, efficiency, and fuel utilization. It connects AI agents to core energy balance methodologies, allowing for precise calculation of energy intensity, fuel equivalents, and cogeneration performance. Use `get_energy_intensity` to measure efficiency per barrel, `calculate_fuel_equivalent` to standardize energy carriers, `evaluate_cogeneration_performance` to assess CHP systems, and `identify_optimization_targets` to find cost-reduction opportunities.


## Available Tools (4)
- **evaluate_cogeneration_performance**: Evaluate the efficiency of the combined heat and power (CHP) system
- **get_energy_intensity**: Calculate energy intensity per unit of production
- **identify_optimization_targets**: Identify significant opportunities to reduce energy costs and improve efficiency
- **calculate_fuel_equivalent**: Calculate total energy consumption expressed in a single standardized fuel unit


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Refinery Energy Balance** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is the energy intensity if we consumed 500,000 GJ for 100,000 barrels?"

**🤖 AI Agent:**
> The energy intensity is 5.0 GJ per barrel.

---

**👤 You:**
> "Calculate the fuel equivalent for 100 units of fuel, 50 units of electricity (factor 0.34), and 20 units of steam (factor 0.75)."

**🤖 AI Agent:**
> The total fuel equivalent is 132.0 units.

---

**👤 You:**
> "Is our cogeneration system performing well if we input 1000 units of fuel and produce 650 units of total energy (electricity + steam)?"

**🤖 AI Agent:**
> Yes, the cogeneration efficiency is 65%, which is considered high performing.


## ❓ FAQ

**Q: How can I measure the efficiency of my refinery?**
You can use the `get_energy_intensity` tool to calculate the energy consumed per unit of production, such as energy per barrel of crude.

**Q: Can I standardize different energy sources into one unit?**
Yes, the `calculate_fuel_equivalent` tool converts electricity and steam into a single standardized fuel unit using provided conversion factors.

**Q: How do I find areas to reduce energy costs?**
The `identify_optimization_targets` tool analyzes current intensity and cogeneration efficiency to flag priority areas for improvement.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/refinery-energy-balance](https://vinkius.com/en/ai-agent-connect/refinery-energy-balance)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Refinery Energy Balance** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `refinery-energy-balance` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Refinery Energy Balance** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "refinery-energy-balance": {
      "url": "https://edge.vinkius.com/[TOKEN]/mcp"
    }
  }
}
```

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius connector registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
