# Used Car Shopping Plan MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/used-car-shopping-plan)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [finance](../categories/finance.md)

Compare used cars by analyzing total cost of ownership, including repairs and running costs.

## Description
This MCP server provides a comprehensive financial engine for evaluating used vehicles. It allows AI agents to calculate the Total Cost of Ownership (TCO) by aggregating sticker price, financing interest, projected repair reserves, and cumulative running costs. Use `get_car_details` to fetch vehicle specs, `calculate_running_costs` for fuel and tax estimates, `estimate_repair_reserve` for maintenance contingency planning, and `generate_comparison_report` to compare multiple vehicles side-by-side.


## Available Tools (4)
- **estimate_repair_reserve**: Calculates the recommended contingency fund required for maintenance and repairs
- **generate_comparison_report**: Provides a holistic financial view by aggregating purchase price, financing, repairs, and running costs
- **get_car_details**: Retrieves the core specifications and pricing data for a specific vehicle
- **calculate_running_costs**: Estimates the cumulative cost of fuel, insurance, and tax over a set period


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Used Car Shopping Plan** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Compare the total cost of ownership for car IDs 'car_001' and 'car_002' over 5 years with 12,000 miles per year."

**🤖 AI Agent:**
> The total cost of ownership for car_001 is $15,400, while car_002 is $18,250 over the 5-year period.

---

**👤 You:**
> "What are the estimated running costs for car_005 if I drive 15,000 miles a year and fuel is $3.50?"

**🤖 AI Agent:**
> The estimated cumulative running costs for car_005 are $6,200 over the specified period.

---

**👤 You:**
> "How much repair reserve should I set aside for car_010 if I have a conservative risk tolerance?"

**🤖 AI Agent:**
> A recommended repair reserve of $2,500 is suggested for car_010 with a conservative risk profile.


## ❓ FAQ

**Q: How is the total cost of ownership calculated?**
The total cost is the sum of the sticker price, financing interest, the estimated repair reserve, and all cumulative running costs like fuel and insurance.

**Q: What is a repair reserve?**
A repair reserve is a contingency fund calculated based on the vehicle's age and mileage to cover unexpected maintenance.

**Q: Can I compare multiple cars at once?**
Yes, you can use the comparison tool to generate a holistic report for a list of vehicle IDs.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/used-car-shopping-plan](https://vinkius.com/en/ai-agent-connect/used-car-shopping-plan)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Used Car Shopping Plan** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `used-car-shopping-plan` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Used Car Shopping Plan** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "used-car-shopping-plan": {
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
