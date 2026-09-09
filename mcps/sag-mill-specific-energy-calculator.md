# SAG Mill Specific Energy Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/sag-mill-specific-energy-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [engineering](../categories/engineering.md)

Estimates energy consumption, power draw, and throughput for SAG mills.

## Description
This MCP server provides specialized engineering tools for Semi-Autogenous Grinding (SAG) mill analysis. It allows AI agents to calculate specific energy requirements using `calculate_specific_energy`, predict mill performance with `predict_mill_performance`, evaluate the impact of pebble crushing via `evaluate_pebble_circuit`, and analyze capacity sensitivity through `simulate_sizing_impact`. It is designed to bridge the gap between ore characteristics and mill performance predictions.


## Available Tools (4)
- **calculate_specific_energy**: Determines the theoretical energy required per tonne to achieve a specific product size
- **evaluate_pebble_circuit**: Adjusts the throughput and energy efficiency based on the presence of a pebble crushing circuit
- **predict_mill_performance**: Estimates the total power draw and the expected throughput for a given mill configuration
- **simulate_sizing_impact**: Analyzes how changes in the target product size affect the entire circuit's capacity


## 💬 Prompt Examples

Here are some examples of how you can interact with the **SAG Mill Specific Energy Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Calculate the specific energy for an ore with competency 1.5, BWI of 14, and a target size of 200 microns."

**🤖 AI Agent:**
> The calculated specific energy is 8.45 kWh/t with an energy per size ratio of 0.12.

---

**👤 You:**
> "Predict the performance of a mill with 5m diameter, 10m length, 8.5 kWh/t specific energy, and 5000 kW available power."

**🤖 AI Agent:**
> The predicted throughput is 588.24 t/h with an estimated power draw of 5000 kW.

---

**👤 You:**
> "What is the impact of a 0.3 pebble recycle ratio and 0.8 crushing efficiency on a base throughput of 500 t/h?"

**🤖 AI Agent:**
> The adjusted throughput is 565.0 t/h with a total circuit energy of 4237.5 kWh/t.


## ❓ FAQ

**Q: How do I calculate the energy needed for a specific ore?**
You can use the `calculate_specific_energy` tool by providing the ore competency, Bond Work Index, and the target product size.

**Q: Can I account for pebble crushing in my throughput predictions?**
Yes, the `evaluate_pebble_circuit` tool allows you to adjust throughput and energy efficiency based on pebble recycle ratios and crushing efficiency.

**Q: How does mill size affect my power draw?**
The `predict_mill_performance` tool uses the mill diameter and length to estimate the total power draw and expected throughput.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/sag-mill-specific-energy-calculator](https://vinkius.com/ai-agent-connect/sag-mill-specific-energy-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **SAG Mill Specific Energy Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `sag-mill-specific-energy-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **SAG Mill Specific Energy Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "sag-mill-specific-energy-calculator": {
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
