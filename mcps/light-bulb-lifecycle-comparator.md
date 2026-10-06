# Light Bulb Lifecycle Comparator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/light-bulb-lifecycle-comparator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [finance](../categories/finance.md)

Evaluate the total cost of ownership and energy efficiency for different lighting technologies.

## Description
This MCP server provides a suite of tools to calculate the total cost of ownership (TCO) for various light bulbs. By analyzing purchase price, wattage, rated lifespan, and electricity costs, users can determine the most economical lighting solutions. Use `calculate_bulb_metrics` to find the projected cost of a single bulb type, `compare_bulb_profiles` to rank multiple options, `get_energy_efficiency_rating` to assess lumen-per-watt efficacy, and `simulate_replacement_impact` to see how lifespan variations affect long-term expenses.


## Available Tools (4)
- **calculate_bulb_metrics**: Calculates the technical and financial performance metrics for a single bulb type
- **compare_bulb_profiles**: Compares two or more different bulb configurations to determine the most cost-effective option
- **get_energy_efficiency_rating**: Determines a qualitative efficiency score for a bulb based on its power consumption
- **simulate_replacement_impact**: Evaluates how sensitive the total cost is to changes in the bulb's rated lifespan


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Light Bulb Lifecycle Comparator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Calculate the total cost for an LED bulb that costs $5, uses 10 watts, lasts 15,000 hours, is used 5 hours a day, with electricity at $0.15/kWh and a $0.50 disposal fee over 365 days."

**🤖 AI Agent:**
> The total projected cost for this LED bulb over 365 days is $6.12.

---

**👤 You:**
> "Which is cheaper: a 60W incandescent bulb at $1 or a 10W LED bulb at $5, both used 8 hours a day for a year with electricity at $0.20/kWh?"

**🤖 AI Agent:**
> The 10W LED bulb is the best option with a total cost of $10.56, compared to the incandescent bulb which costs $35.52.

---

**👤 You:**
> "What is the efficiency category for a bulb that produces 800 lumens using 9 watts?"

**🤖 AI Agent:**
> The bulb has an efficacy of 88.89 lumens per watt and falls into the High efficiency category.


## ❓ FAQ

**Q: How does the tool calculate the total cost?**
The tool sums the initial purchase price, the cumulative electricity cost based on wattage and runtime, and the disposal costs for all bulbs required over the evaluation period.

**Q: Can I compare multiple bulb types at once?**
Yes, you can use `compare_bulb_profiles` to provide multiple bulb configurations and receive a ranked list from most to least cost-effective.

**Q: What factors affect the energy efficiency rating?**
The efficiency rating is determined by the ratio of brightness (lumens) to power consumption (watts) using the `get_energy_efficiency_rating` tool.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/light-bulb-lifecycle-comparator](https://vinkius.com/en/ai-agent-connect/light-bulb-lifecycle-comparator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Light Bulb Lifecycle Comparator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `light-bulb-lifecycle-comparator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Light Bulb Lifecycle Comparator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "light-bulb-lifecycle-comparator": {
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
