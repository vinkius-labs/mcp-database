# Bulb Energy Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/bulb-energy-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [utilities](../categories/utilities.md)

Calculate energy consumption, costs, and efficiency for light bulbs.

## Description
This MCP server provides tools to calculate electrical energy consumption for light bulbs. Use `get_bulb_energy_consumption` to find total kWh used, `get_energy_cost_estimate` to calculate monetary costs based on local rates, `get_bulb_efficiency_tier` to classify efficiency, and `compare_bulb_usage` to see the difference between two bulbs.


## Available Tools (4)
- **compare_bulb_usage**: Compares the energy consumption of two different bulbs over the same period
- **get_bulb_efficiency_tier**: Classifies a bulb into an efficiency category based on its wattage relative to standard usage profiles
- **get_bulb_energy_consumption**: Calculates the total energy consumed by a single bulb over a specific timeframe
- **get_energy_cost_estimate**: Estimates the financial cost of running a bulb based on its energy usage and local electricity rates


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Bulb Energy Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "How much energy does a 60W bulb use if it is on for 10 hours?"

**🤖 AI Agent:**
> A 60W bulb used for 10 hours consumes 0.6 kWh.

---

**👤 You:**
> "What is the cost of running a 100W bulb for 24 hours at $0.15 per kWh?"

**🤖 AI Agent:**
> The estimated cost is $0.36.

---

**👤 You:**
> "Which is more efficient: a 10W bulb or a 40W bulb used for 5 hours?"

**🤖 AI Agent:**
> The 10W bulb is more efficient.


## ❓ FAQ

**Q: How do I calculate the cost of my light bulb usage?**
You can use the `get_energy_cost_estimate` tool by providing the bulb's wattage, the hours used, and your local electricity rate per kWh.

**Q: Can I compare two different bulbs?**
Yes, the `compare_bulb_usage` tool allows you to compare the energy consumption of two bulbs and identifies which one is more efficient.

**Q: What units are used for energy consumption?**
Energy consumption is calculated and returned in kilowatt-hours (kWh).


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/bulb-energy-calculator](https://vinkius.com/en/ai-agent-connect/bulb-energy-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Bulb Energy Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `bulb-energy-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Bulb Energy Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "bulb-energy-calculator": {
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
