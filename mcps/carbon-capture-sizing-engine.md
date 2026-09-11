# Carbon Capture Sizing Engine MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/carbon-capture-sizing-engine)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [engineering](../categories/engineering.md)

Technical sizing engine for CO2 removal system dimensions, energy, and costs.

## Description
This MCP server provides technical sizing for carbon capture systems. It calculates physical vessel dimensions using `get_system_dimensions`, determines chemical needs via `calculate_solvent_requirements`, estimates power and heat needs with `estimate_energy_demand`, and provides economic analysis through `calculate_capture_economics`. It is designed for engineers designing amine-based or other CO2 removal technologies.


## Available Tools (4)
- **calculate_capture_economics**: Provides the cost analysis for the carbon capture operation
- **calculate_solvent_requirements**: Calculates the amount of chemical solvent needed to process the gas stream
- **estimate_energy_demand**: Calculates the thermal and electrical energy needed to operate the system
- **get_system_dimensions**: Determines the physical size of the capture equipment


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Carbon Capture Sizing Engine** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What are the dimensions for a system capturing 90% of CO2 from a gas stream with a flow rate of 50 m3/s and a 15% CO2 concentration?"

**🤖 AI Agent:**
> The absorber diameter is 3.5 meters with a height of 12.0 meters, and the stripper diameter is 2.8 meters with a height of 10.5 meters.

---

**👤 You:**
> "How much energy will be required for a capture system with a circulation rate of 150 kg/s?"

**🤖 AI Agent:**
> The system requires 450 MW of thermal energy and 25 MW of electrical energy for operation.

---

**👤 You:**
> "What is the estimated cost per tonne of CO2 if the capital expenditure is 500 million dollars?"

**🤖 AI Agent:**
> The estimated cost is 65 dollars per tonne of CO2 captured.


## ❓ FAQ

**Q: What can I calculate with this server?**
You can determine the physical size of absorbers and strippers, the required solvent circulation rate, the total energy demand, and the economic cost per tonne of CO2 captured.

**Q: How do I determine the equipment size?**
Use the `get_system_dimensions` tool by providing the flue gas composition, the gas flow rate, and your target CO2 capture fraction.

**Q: Does this support different solvent types?**
Yes, you can specify different solvents like MEA, DEA, or PZ when using `calculate_solvent_requirements` to get accurate circulation rates.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/carbon-capture-sizing-engine](https://vinkius.com/en/ai-agent-connect/carbon-capture-sizing-engine)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Carbon Capture Sizing Engine** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `carbon-capture-sizing-engine` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Carbon Capture Sizing Engine** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "carbon-capture-sizing-engine": {
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
