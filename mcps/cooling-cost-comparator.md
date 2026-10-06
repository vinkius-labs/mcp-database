# Cooling Cost Comparator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/cooling-cost-comparator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [finance](../categories/finance.md)

Compare the financial impact of using fans versus air conditioning.

## Description
This MCP server provides tools to evaluate the total cost of ownership for different cooling methods. Use `get_fan_scenario` and `get_ac_scenario` to calculate electricity costs and TCO for specific devices, or use `compare_cooling_costs` to find the most economical option between a fan and an AC unit. You can also use `get_energy_efficiency_ratio` to see the power consumption difference.


## Available Tools (4)
- **compare_cooling_costs**: Performs the comparative analysis between a fan scenario and an AC scenario
- **get_ac_scenario**: Retrieves the specific configuration and cost data for a defined air conditioning setup
- **get_energy_efficiency_ratio**: Calculates the ratio of energy consumption between the two devices
- **get_fan_scenario**: Retrieves the specific configuration and cost data for a defined fan setup


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Cooling Cost Comparator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Compare a 50W fan costing $30 with a 1000W AC costing $400. Electricity is $0.15 per kWh. Both run for 500 hours."

**🤖 AI Agent:**
> The fan is the cheaper option, saving you $375.00 compared to the air conditioner.

---

**👤 You:**
> "What is the electricity cost for a 60W fan running for 1000 hours at $0.20 per kWh?"

**🤖 AI Agent:**
> The total electricity cost for the fan is $12.00.

---

**👤 You:**
> "How much more power does a 1500W AC use compared to a 40W fan?"

**🤖 AI Agent:**
> The air conditioning unit consumes 37.5 times more power than the fan.


## ❓ FAQ

**Q: How does the tool calculate the total cost?**
The tool calculates the Total Cost of Ownership (TCO) by summing the purchase cost, the total maintenance cost, and the electricity cost derived from wattage and runtime.

**Q: Can I compare different electricity prices?**
Yes, you can provide any electricity price per kWh to see how it affects the total cost of your cooling options.

**Q: What is the difference between a fan and an AC in terms of power?**
You can use `get_energy_efficiency_ratio` to find exactly how many times more power an AC unit consumes compared to a fan.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/cooling-cost-comparator](https://vinkius.com/en/ai-agent-connect/cooling-cost-comparator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Cooling Cost Comparator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `cooling-cost-comparator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Cooling Cost Comparator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "cooling-cost-comparator": {
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
