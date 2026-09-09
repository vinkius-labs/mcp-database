# Ore Sorting Optimization MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/ore-sorting-optimization)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [engineering](../categories/engineering.md)

Optimize ore sorting circuit design through grade distribution analysis and capacity modeling.

## Description
This MCP server provides specialized tools for mining engineers to optimize ore sorting circuits. It allows for detailed analysis of ore quality using `analyze_ore_distribution`, determination of optimal cut-off grades via `calculate_sorting_parameters`, and physical hardware verification with `evaluate_circuit_capacity`. Additionally, it ensures logistical feasibility through `perform_mass_water_balance` to manage material and water flows accurately.


## Available Tools (4)
- **analyze_ore_distribution**: Analyze the statistical distribution of ore grades in the raw feed
- **calculate_sorting_parameters**: Calculate optimal cut-off grade and predicted recovery
- **evaluate_circuit_capacity**: Evaluate the physical capacity of the sorting circuit
- **perform_mass_water_balance**: Perform mass and water balance calculations


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Ore Sorting Optimization** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Analyze this ore grade data: [1.2, 0.5, 2.1, 0.8, 1.5]"

**🤖 AI Agent:**
> The ore distribution analysis shows a mean grade of 1.22 and a maximum grade of 2.1.

---

**👤 You:**
> "What is the capacity for a 1.5m belt moving at 2m/s with ore density of 2.5 t/m3 and 0.05m thickness?"

**🤖 AI Agent:**
> The calculated throughput capacity is 37.5 tonnes per second.

---

**👤 You:**
> "Calculate the mass yield for 1000 tonnes of input with a 0.85 mass yield."

**🤖 AI Agent:**
> The resulting product mass is 850 tonnes and the waste mass is 150 tonnes.


## ❓ FAQ

**Q: How can I determine the best cut-off grade for my sensor?**
You can use the `calculate_sorting_parameters` tool, providing your grade data, sensor accuracy, and target recovery to find the optimal threshold.

**Q: Can I check if my conveyor belt is wide enough for the ore throughput?**
Yes, the `evaluate_circuit_capacity` tool calculates throughput capacity based on belt width, speed, ore density, and material thickness.

**Q: How do I calculate the water requirements for the sorting process?**
Use the `perform_mass_water_balance` tool to calculate total water requirements and losses based on input mass and moisture content.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/ore-sorting-optimization](https://vinkius.com/ai-agent-connect/ore-sorting-optimization)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Ore Sorting Optimization** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `ore-sorting-optimization` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Ore Sorting Optimization** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "ore-sorting-optimization": {
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
