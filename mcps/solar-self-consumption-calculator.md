# Solar Self-Consumption Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/solar-self-consumption-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [mathematics](../categories/mathematics.md)

Analyze solar energy flows, battery dynamics, and economic impact.

## Description
This MCP server provides tools to model residential solar and battery systems. Use `calculate_hourly_energy_flow` to determine how solar generation, household load, and battery state interact in any given hour. You can also use `calculate_daily_economics` to find net costs or credits, `analyze_self_consumption_efficiency` to evaluate system utilization, and `simulate_battery_cycling` to project battery state over time.


## Available Tools (4)
- **analyze_self_consumption_efficiency**: Evaluates how effectively the system is utilizing its solar generation
- **calculate_daily_economics**: Determines the total financial cost or savings for a single day based on energy flows
- **calculate_hourly_energy_flow**: Calculates the specific energy movements (consumption, storage, export, import) for a single hour
- **simulate_battery_cycling**: Projects the state of the battery over a series of hourly flows


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Solar Self-Consumption Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Calculate the energy flow for an hour with 5000Wh generation, 2000Wh load, 1000Wh current battery charge, and 5000Wh capacity."

**🤖 AI Agent:**
> In this hour, 2000Wh is consumed by the load, 3000Wh is used to charge the battery (bringing it to 4000Wh), and 0Wh is exported.

---

**👤 You:**
> "What are the economics if I imported 1000Wh at 0.15/Wh and exported 500Wh at 0.08/Wh?"

**🤖 AI Agent:**
> The total import cost is 150.00, the total export credit is 40.00, resulting in a net cost of 110.00.

---

**👤 You:**
> "How efficient is a system that produced 10000Wh, used 7000Wh, and exported 2000Wh?"

**🤖 AI Agent:**
> The self-consumption ratio is 0.7 and the wasted energy ratio is 0.2.


## ❓ FAQ

**Q: How do I calculate my daily savings?**
Use the `calculate_daily_economics` tool by providing the total energy imported from the grid, total energy exported to the grid, and the respective import and export rates.

**Q: Can I simulate battery usage over a full day?**
Yes, the `simulate_battery_cycling` tool allows you to project battery state by providing an array of hourly generation and load data.

**Q: What determines if energy is exported to the grid?**
Energy is exported when solar generation exceeds both the household load and the current charging capacity of the battery.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/solar-self-consumption-calculator](https://vinkius.com/en/ai-agent-connect/solar-self-consumption-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Solar Self-Consumption Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `solar-self-consumption-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Solar Self-Consumption Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "solar-self-consumption-calculator": {
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
