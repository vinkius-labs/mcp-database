# Hops Drying Energy Optimizer MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/hops-drying-energy-optimizer)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [agriculture](../categories/agriculture.md)

Optimize hop drying for energy efficiency and alpha acid retention.

## Description
This MCP server provides precise optimization for the hop drying process. It uses a thin-layer drying model to calculate the ideal temperature profiles and airflow requirements needed to reach target moisture levels. Users can use `get_drying_profile` to generate optimal drying sequences, `calculate_energy_metrics` to determine energy consumption and costs, `estimate_quality_retention` to predict alpha acid preservation, and `simulate_drying_efficiency` to compare different dryer architectures like belt, kiln, or whole-plant systems.


## Available Tools (4)
- **get_drying_profile**: Generates the optimal sequence of temperatures and airflows to reach the target moisture
- **estimate_quality_retention**: Predicts the percentage of alpha acids preserved after the drying process
- **calculate_energy_metrics**: Calculates the total energy required and the efficiency of the process
- **simulate_drying_efficiency**: Compares different drying scenarios for the same batch of hops


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Hops Drying Energy Optimizer** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Generate a drying profile for 500kg of hops with 80% initial moisture and a target of 9%."

**🤖 AI Agent:**
> The optimal drying profile for 500kg of hops requires a starting temperature of 55°C, gradually decreasing to 40°C as moisture reaches 9%, with a constant airflow rate of 120 m³/h.

---

**👤 You:**
> "What is the estimated energy cost for drying 1000kg of hops from 75% to 10% moisture using a belt dryer?"

**🤖 AI Agent:**
> The total energy consumption for this batch is 4,500,000 kJ, resulting in a drying cost of $12.50 per kg of dried hops.

---

**👤 You:**
> "Compare the efficiency of a kiln dryer versus a belt dryer for 200kg of hops."

**🤖 AI Agent:**
> The belt dryer offers a lower drying cost of $0.15/kg with 94% alpha acid retention, while the kiln dryer has a higher cost of $0.22/kg but provides 96% alpha acid retention.


## ❓ FAQ

**Q: How does this tool help with alpha acid retention?**
By using `estimate_quality_retention`, the tool predicts how much alpha acid is preserved based on the specific temperature profile used, helping to prevent thermal degradation.

**Q: Can I compare different types of dryers?**
Yes, the `simulate_drying_efficiency` tool allows you to compare the cost and quality outcomes of different dryer types, such as belt, kiln, or whole-plant dryers.

**Q: What inputs are required for the drying profile?**
To use `get_drying_profile`, you need to provide the initial moisture content, the target moisture, the total mass of hops in kilograms, and the type of dryer being used.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/hops-drying-energy-optimizer](https://vinkius.com/ai-agent-connect/hops-drying-energy-optimizer)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Hops Drying Energy Optimizer** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `hops-drying-energy-optimizer` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Hops Drying Energy Optimizer** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "hops-drying-energy-optimizer": {
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
