# Travel Budget Planner MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/travel-budget-planner)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Calculate daily spending limits and trip costs.

## Description
This MCP server provides tools to manage trip finances. Use `get_daily_allowance` to find your daily spending limit, `get_allowance_with_buffer` to reserve emergency funds, `get_extended_trip_cost` to plan total budget needs, and `get_trip_cost_breakdown` to see how funds are distributed across categories.


## Available Tools (4)
- **get_daily_allowance**: Calculates the basic daily spending limit
- **get_extended_trip_cost**: Determines how much total budget is required for a specific daily spending target
- **get_allowance_with_buffer**: Calculates a daily spending limit while reserving a specific amount for emergencies
- **get_trip_cost_breakdown**: Provides a detailed view of how a budget is distributed across different expense categories


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Travel Budget Planner** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "I have a budget of 1500 USD for a 10-day trip. How much can I spend each day?"

**🤖 AI Agent:**
> You can spend 150 USD per day.

---

**👤 You:**
> "I want to spend 50 USD a day for 7 days. How much total budget do I need if I want a 10% buffer?"

**🤖 AI Agent:**
> You will need a total budget of 385 USD.

---

**👤 You:**
> "If I have 1000 USD, how much goes to food if it's 40% of my budget?"

**🤖 AI Agent:**
> 400 USD will be allocated to food.


## ❓ FAQ

**Q: How do I calculate my daily spending limit?**
You can use the `get_daily_allowance` tool by providing your total budget and the number of days for your trip.

**Q: Can I set aside money for emergencies?**
Yes, the `get_allowance_with_buffer` tool allows you to reserve a specific amount for unexpected costs before calculating your daily limit.

**Q: How can I see a breakdown of my expenses?**
Use the `get_trip_cost_breakdown` tool to distribute your total budget across different categories like food, transport, or lodging.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/travel-budget-planner](https://vinkius.com/en/ai-agent-connect/travel-budget-planner)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Travel Budget Planner** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `travel-budget-planner` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Travel Budget Planner** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "travel-budget-planner": {
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
