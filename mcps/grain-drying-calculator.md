# Grain Drying Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/grain-drying-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [agriculture](../categories/agriculture.md)

Calculate grain drying time, energy needs, and mass shrinkage.

## Description
This MCP server provides precise thermodynamic calculations for agricultural grain drying. It uses thin-layer drying models to estimate how long it takes to reach a target moisture level using `estimate_drying_time`. Users can also determine energy costs with `calculate_energy_requirements`, verify if drying is physically possible with `verify_drying_feasibility`, and calculate mass loss using `calculate_mass_and_shrinkage`.


## Available Tools (4)
- **calculate_energy_requirements**: Estimates the total energy cost in kWh for the drying process
- **calculate_mass_and_shrinkage**: Calculates the reduction in grain mass and the resulting shrinkage percentage
- **estimate_drying_time**: Calculates how long it will take to reach the target moisture level
- **verify_drying_feasibility**: Checks if the specified air conditions are capable of reaching the target moisture


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Grain Drying Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "How long will it take to dry 10 tons of Corn from 25% to 15% moisture at 40°C, 50% humidity, and 2 m3/min airflow?"

**🤖 AI Agent:**
> It will take approximately 14.5 hours to reach the target moisture, resulting in a final mass of 8.75 tons.

---

**👤 You:**
> "Is it possible to dry Wheat to 12% moisture if the air is at 30°C and 80% humidity?"

**🤖 AI Agent:**
> No, the target moisture of 12% is below the Equilibrium Moisture Content for these conditions.

---

**👤 You:**
> "What is the energy cost to dry grain for 10 hours at 45°C with an airflow of 5 m3/min?"

**🤖 AI Agent:**
> The estimated energy consumption for this operation is 125.4 kWh.


## ❓ FAQ

**Q: How accurate are the drying time estimates?**
Estimates are based on thin-layer drying equations and specific grain constants for Corn, Wheat, and Soybeans.

**Q: Can I check if my target moisture is achievable?**
Yes, use the `verify_drying_feasibility` tool to check if the air conditions allow reaching your target moisture based on the Equilibrium Moisture Content.

**Q: Does this account for grain shrinkage?**
Yes, the `calculate_mass_and_shrinkage` tool calculates the reduction in mass and the resulting shrinkage percentage.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/grain-drying-calculator](https://vinkius.com/ai-agent-connect/grain-drying-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Grain Drying Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `grain-drying-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Grain Drying Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "grain-drying-calculator": {
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
