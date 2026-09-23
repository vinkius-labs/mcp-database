# Fan Cost Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/fan-cost-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [finance](../categories/finance.md)

Calculate the electrical cost of running electric fans.

## Description
This MCP server provides tools to estimate the electrical expenses of operating electric fans. You can use `calculate_fan_running_cost` to find the cost for a specific period, `compare_fan_efficiency` to see which fan is cheaper, `estimate_annual_impact` for yearly projections, and `get_usage_thresholds` to stay within a specific budget.


## Available Tools (4)
- **calculate_fan_running_cost**: Calculates the cost of running a fan for a specific duration
- **compare_fan_efficiency**: Compares the cost-effectiveness of two fans
- **estimate_annual_impact**: Estimates the projected yearly cost of a fan
- **get_usage_thresholds**: Calculates maximum usage hours to stay within a budget


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Fan Cost Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "How much will it cost to run a 50W fan for 8 hours a day for 30 days if electricity is $0.15 per kWh?"

**🤖 AI Agent:**
> It will cost $1.80 to run that fan for 30 days.

---

**👤 You:**
> "Which is cheaper: a 40W fan or a 60W fan, if used 10 hours a day for 7 days at $0.20 per kWh?"

**🤖 AI Agent:**
> The 40W fan is cheaper, costing $0.56 compared to $0.84 for the 60W fan.

---

**👤 You:**
> "What is the annual cost for a 100W fan used 12 hours a day at $0.12 per kWh?"

**🤖 AI Agent:**
> The projected annual cost is $31.54.


## ❓ FAQ

**Q: How do I calculate the cost for a specific duration?**
Use the `calculate_fan_running_cost` tool by providing the fan's wattage, daily usage hours, total days, and your electricity rate.

**Q: Can I compare two different fans?**
Yes, the `compare_fan_efficiency` tool allows you to compare the operating costs of two fans to see which one is more cost-effective.

**Q: How can I stay within my monthly budget?**
You can use `get_usage_thresholds` to determine the maximum number of hours you can run a fan without exceeding your budget.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/fan-cost-calculator](https://vinkius.com/en/ai-agent-connect/fan-cost-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Fan Cost Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `fan-cost-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Fan Cost Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "fan-cost-calculator": {
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
