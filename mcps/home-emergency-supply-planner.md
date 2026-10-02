# Home Emergency Supply Planner MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/home-emergency-supply-planner)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [logistics](../categories/logistics.md)

Calculate essential household supplies, identify inventory gaps, and manage expiration schedules.

## Description
This MCP server provides a complete toolkit for household preparedness. It allows AI agents to calculate the exact quantities of supplies needed for any duration, identify missing items in your current inventory, estimate the cost to reach full preparedness, and generate rotation schedules to prevent item expiration. Use `get_supply_requirements` to plan your needs, `calculate_inventory_gap` to see what is missing, `estimate_preparedness_cost` to budget for supplies, and `get_rotation_schedule` to manage your stock.


## Available Tools (4)
- **calculate_inventory_gap**: Identifies which supplies are missing or insufficient to meet the requirements for a given plan
- **estimate_preparedness_cost**: Provides a financial projection of what it will cost to reach full preparedness
- **get_rotation_schedule**: Generates a list of upcoming dates when supplies should be inspected or replaced to prevent expiration
- **get_supply_requirements**: Determines the total quantity of every required supply type needed for a specific duration and household size


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Home Emergency Supply Planner** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "How many supplies do I need for a family of 4 for 14 days?"

**🤖 AI Agent:**
> For a family of 4 for 14 days, you will need 56 liters of water and 56 units of canned food.

---

**👤 You:**
> "I have 10 liters of water and 5 cans of food. What am I missing for a 3-day plan for 2 people?"

**🤖 AI Agent:**
> You are missing 2 liters of water and 1 can of food to meet the requirements for a 3-day plan for 2 people.

---

**👤 You:**
> "What is my next maintenance window for my current supplies?"

**🤖 AI Agent:**
> Your next maintenance window is October 12, 2025, when your canned goods are scheduled to expire.


## ❓ FAQ

**Q: How do I know how many supplies I need?**
You can use the `get_supply_requirements` tool by providing the number of days you want to be prepared for and the number of people in your household.

**Q: Can I estimate the cost of my emergency kit?**
Yes, the `estimate_preparedness_cost` tool calculates the projected expenditure needed to fill your supply gaps based on current market averages.

**Q: How do I manage expiring food or water?**
The `get_rotation_schedule` tool generates a list of upcoming dates when your supplies should be inspected or replaced.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/home-emergency-supply-planner](https://vinkius.com/en/ai-agent-connect/home-emergency-supply-planner)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Home Emergency Supply Planner** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `home-emergency-supply-planner` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Home Emergency Supply Planner** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "home-emergency-supply-planner": {
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
