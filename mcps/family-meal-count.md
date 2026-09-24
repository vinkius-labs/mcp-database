# Family Meal Count MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/family-meal-count)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Calculate total meals for groups and durations.

## Description
This MCP server provides tools to calculate meal requirements for groups. Use `get_daily_meal_requirement` to find daily totals, `calculate_total_period_meals` for long-term planning, and `get_meal_budget_per_person` to see individual consumption. It also includes `validate_meal_planning_inputs` to ensure your planning parameters are valid.


## Available Tools (4)
- **calculate_total_period_meals**: Answers how many meals are needed for a specific number of days
- **get_daily_meal_requirement**: Answers how many meals the entire group eats in a single day
- **get_meal_budget_per_person**: Answers how many total meals a single person will consume over a period
- **validate_meal_planning_inputs**: Answers whether a set of meal planning parameters is mathematically valid for a schedule


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Family Meal Count** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "How many meals does a group of 4 people eat in one day if they eat 3 times a day?"

**🤖 AI Agent:**
> The group eats 12 meals in one day.

---

**👤 You:**
> "Calculate total meals for 2 people eating 2 meals a day for 10 days."

**🤖 AI Agent:**
> The total number of meals needed is 40.

---

**👤 You:**
> "How many meals will one person eat over 5 days if they eat 4 times a day?"

**🤖 AI Agent:**
> One person will eat 20 meals over 5 days.


## ❓ FAQ

**Q: How do I calculate meals for a whole week?**
You can use the `calculate_total_period_meals` tool by providing the number of people, meals per day, and setting the duration to 7 days.

**Q: Can I validate my planning numbers?**
Yes, use `validate_meal_planning_inputs` to check if your people count, meals per day, and duration are valid positive integers.

**Q: How many meals does one person eat in 30 days if they eat 3 times a day?**
That person will consume 90 meals in total.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/family-meal-count](https://vinkius.com/en/ai-agent-connect/family-meal-count)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Family Meal Count** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `family-meal-count` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Family Meal Count** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "family-meal-count": {
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
