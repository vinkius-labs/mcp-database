# Mine Ventilation Cost Optimizer MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/mine-ventilation-cost-optimizer)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [engineering](../categories/engineering.md)

Optimize underground mine ventilation by calculating required airflow and selecting the most cost-effective fans.

## Description
This MCP server provides specialized tools for underground mine ventilation management. It allows engineers to calculate the total intake airflow needed by accounting for leakage, evaluate if specific fan models meet pressure and volume requirements using `evaluate_fan_performance`, and determine the financial impact of equipment through `calculate_operating_costs`. The core capability is the `optimize_fan_selection` tool, which identifies the most economical fan choice from a library of options based on technical needs and electricity pricing.


## Available Tools (4)
- **calculate_operating_costs**: Computes the financial impact of running a fan based on its power draw
- **evaluate_fan_performance**: Determines if a specific fan can meet the calculated air and pressure requirements
- **get_required_airflow**: Calculates the total air volume that must be supplied at the intake to meet face requirements after accounting for losses
- **optimize_fan_selection**: Identifies the most cost-effective fan from a list of available options


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Mine Ventilation Cost Optimizer** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "How much total airflow do I need if the face requirement is 500 m3/s and leakage is 15%?"

**🤖 AI Agent:**
> The total required airflow is 588.24 m3/s.

---

**👤 You:**
> "Which fan is best for 600 m3/s at 200 Pa if electricity is $0.12/kWh and it runs for 2000 hours?"

**🤖 AI Agent:**
> The optimal fan is Model-X, with a total operating cost of $1,440.00.

---

**👤 You:**
> "Calculate the cost for a 50kW fan running for 100 hours at $0.15 per kWh."

**🤖 AI Agent:**
> The total operating cost is $750.00.


## ❓ FAQ

**Q: How does the tool account for air loss in the mine?**
The `get_required_airflow` tool calculates the necessary intake volume by factoring in the expected leakage percentage to ensure the required air reaches the working face.

**Q: Can I compare different fan models?**
Yes, you can use `optimize_fan_selection` to compare multiple fan profiles and find the one that meets your technical requirements at the lowest operating cost.

**Q: What inputs are needed for cost calculation?**
To calculate costs, you need the fan's power consumption in kW, the electricity price per kWh, and the total operating hours.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/mine-ventilation-cost-optimizer](https://vinkius.com/ai-agent-connect/mine-ventilation-cost-optimizer)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Mine Ventilation Cost Optimizer** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `mine-ventilation-cost-optimizer` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Mine Ventilation Cost Optimizer** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "mine-ventilation-cost-optimizer": {
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
