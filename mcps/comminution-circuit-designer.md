# Comminution Circuit Designer MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/comminution-circuit-designer)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [engineering](../categories/engineering.md)

Design optimal mineral processing circuits, equipment sizing, and energy requirements.

## Description
This MCP server provides specialized tools for mineral processing engineers to design comminution circuits. By analyzing ore properties with `analyze_ore_properties`, users can determine the most efficient configuration using `calculate_circuit_configuration`. The server also enables precise physical dimensioning via `size_equipment` and power demand forecasting through `estimate_energy_consumption`.


## Available Tools (4)
- **analyze_ore_properties**: Evaluates the specific characteristics and grindability of a given ore sample
- **calculate_circuit_configuration**: Determines the most efficient circuit type based on ore hardness and throughput
- **estimate_energy_consumption**: Predicts the total electrical power required to operate the designed circuit
- **size_equipment**: Calculates the physical dimensions and capacities required for the identified circuit equipment


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Comminution Circuit Designer** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Analyze an ore with a hardness index of 75 and 5% moisture."

**🤖 AI Agent:**
> The ore is categorized as Hard with a grindability factor of 0.85.

---

**👤 You:**
> "What circuit configuration is best for an ore with hardness 40 and throughput of 500 tph?"

**🤖 AI Agent:**
> An ABC circuit is the most efficient configuration for these parameters.

---

**👤 You:**
> "Calculate the equipment size for an SABC circuit with 1000 tph throughput and hardness 80."

**🤖 AI Agent:**
> The required equipment includes a SAG mill with a diameter of 8.5m and a motor power rating of 12.5 MW.


## ❓ FAQ

**Q: How do I determine the best circuit for my ore?**
First, use `analyze_ore_properties` to understand the hardness. Then, pass that hardness index to `calculate_circuit_configuration` to find the optimal setup like SABC or ABC.

**Q: Can I estimate the power needed for a SAG mill?**
Yes, after sizing your equipment with `size_equipment`, you can use `estimate_energy_consumption` to predict the total electrical power demand.

**Q: What inputs are required for ore analysis?**
The primary requirement is the `oreHardnessIndex`. You can also optionally provide the `moistureContent` for a more detailed evaluation.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/comminution-circuit-designer](https://vinkius.com/en/ai-agent-connect/comminution-circuit-designer)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Comminution Circuit Designer** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `comminution-circuit-designer` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Comminution Circuit Designer** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "comminution-circuit-designer": {
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
