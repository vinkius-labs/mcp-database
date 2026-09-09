# Roaster Circuit Design MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/roaster-circuit-design)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [engineering](../categories/engineering.md)

Engineering tool for designing roasting circuits for refractory ores.

## Description
This MCP server provides specialized engineering calculations for designing roasting circuits used to treat refractory ores. It allows users to determine vessel dimensions using `calculate_roaster_dimensions`, manage gas flow with `calculate_gas_handling_requirements`, design environmental mitigation via `design_off_gas_treatment`, and monitor thermal stability with `analyze_temperature_profile`.


## Available Tools (4)
- **analyze_temperature_profile**: Evaluates if the thermal energy released by oxidation remains within safe and effective operating limits
- **calculate_gas_handling_requirements**: Determines the volumetric flow rates and velocity required for gas transport
- **calculate_roaster_dimensions**: Determines the physical size and capacity of the roasting vessel
- **design_off_gas_treatment**: Sizes the equipment needed to capture sulfur and meet environmental standards


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Roaster Circuit Design** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Calculate the vessel dimensions for 50 tons of ore per hour with 5% sulfur and 2% carbon and a 4-hour residence time."

**🤖 AI Agent:**
> The required vessel diameter is 4.5 meters, the height is 12.0 meters, with a total volume of 190.85 cubic meters and a heating zone length of 15.5 meters.

---

**👤 You:**
> "What are the gas handling requirements for 100 tons/hr throughput at 850 degrees Celsius with 10% sulfur?"

**🤖 AI Agent:**
> The volumetric flow rate is 12,450 m3/h with a gas velocity of 15.2 m/s and a pressure drop of 250 Pa.

---

**👤 You:**
> "Design an off-gas treatment system for a flow rate of 5000 m3/h with 2% sulfur concentration and a 99% capture target."

**🤖 AI Agent:**
> The scrubber capacity is 5200 m3/h, the reagent consumption rate is 45 kg/h, and the expected emission level is 0.0002%.


## ❓ FAQ

**Q: How do I calculate the size of the roasting vessel?**
You can use the `calculate_roaster_dimensions` tool by providing the ore throughput, sulfur and carbon content, and the required residence time.

**Q: Can this tool help with environmental compliance?**
Yes, the `design_off_gas_treatment` tool helps size equipment to capture sulfur and meet regulatory standards.

**Q: How is thermal stability monitored?**
The `analyze_temperature_profile` tool evaluates peak temperatures and thermal stability based on the exothermic heat from oxidation.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/roaster-circuit-design](https://vinkius.com/ai-agent-connect/roaster-circuit-design)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Roaster Circuit Design** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `roaster-circuit-design` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Roaster Circuit Design** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "roaster-circuit-design": {
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
