# Centrifugal Concentrator Design Tool MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/centrifugal-concentrator-design-tool)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [engineering](../categories/engineering.md)

Design centrifugal concentrator circuits by calculating unit capacity, circuit configuration, and fluidization parameters.

## Description
This MCP server provides specialized engineering tools for designing centrifugal concentrator circuits, such as Falcon or Knelson units. It allows AI agents to calculate the processing capacity of individual units using `calculate_unit_capacity`, determine the total number of units required via `design_circuit_configuration`, optimize water flow and pressure with `optimize_fluidization_parameters`, and predict operational timing using `estimate_operational_cycle`. It is designed to bridge mineral processing requirements with automated circuit design.


## Available Tools (4)
- **calculate_unit_capacity**: Determines the processing capacity of a single concentrator unit based on particle and grade requirements
- **design_circuit_configuration**: You can optionally provide a redundancy factor.

Determines the total number of concentrator units and the total system footprint required for a specific throughput
- **estimate_operational_cycle**: Predicts the timing of the concentration cycle and the frequency of concentrate reclamation
- **optimize_fluidization_parameters**: Calculates the required fluidization water flow and pressure to maintain an active bed for a given particle size


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Centrifugal Concentrator Design Tool** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Calculate the capacity for a unit with 2% feed grade, 75 micron particles, and 85% target recovery at 60G."

**🤖 AI Agent:**
> The unit capacity is 12.5 TPH with a recommended G-force of 60G and a theoretical recovery of 85%.

---

**👤 You:**
> "How many units do I need for a 100 TPH feed if each unit handles 25 TPH?"

**🤖 AI Agent:**
> You will need 4 units to process a 100 TPH feed rate.

---

**👤 You:**
> "What are the fluidization requirements for 50 micron particles at 80G and 90% concentrate grade?"

**🤖 AI Agent:**
> The required water flow rate is 45 Lpm with a fluidization pressure of 1.2 Bar, resulting in a bed stability index of 0.85.


## ❓ FAQ

**Q: How do I determine the number of units needed for my plant?**
You can use the `design_circuit_configuration` tool. Provide the total feed rate and the capacity of a single unit to get the required number of units and the estimated footprint.

**Q: Can I optimize fluidization for specific particle sizes?**
Yes, the `optimize_fluidization_parameters` tool calculates the necessary water flow rate and pressure based on the target particle size and G-force.

**Q: How is the unit capacity calculated?**
The `calculate_unit_capacity` tool determines capacity by evaluating the feed grade, particle size, target recovery, and the applied G-force.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/centrifugal-concentrator-design-tool](https://vinkius.com/en/ai-agent-connect/centrifugal-concentrator-design-tool)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Centrifugal Concentrator Design Tool** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `centrifugal-concentrator-design-tool` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Centrifugal Concentrator Design Tool** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "centrifugal-concentrator-design-tool": {
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
