# Birthday Party Planner MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/birthday-party-planner)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [lifestyle](../categories/lifestyle.md)

Plan complete party logistics including timelines, shopping lists, and staffing.

## Description
This MCP server provides a complete suite of tools to organize birthday celebrations. Use `plan_party_logistics` to generate a full itinerary, shopping list, and cost breakdown. You can also use `calculate_food_requirements` to determine specific food quantities based on guest ages, `estimate_staffing_needs` to ensure proper supervision, and `verify_budget_feasibility` to keep your spending on track.


## Available Tools (4)
- **calculate_food_requirements**: Determines specific food and supply quantities based on guest profiles
- **estimate_staffing_needs**: Calculates how many supervisors are needed based on the age of the guests
- **verify_budget_feasibility**: Checks if a specific set of costs fits within the user's budget
- **plan_party_logistics**: Generates a comprehensive party plan including timeline, shopping list, staffing, and cost breakdown


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Birthday Party Planner** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Plan a party for 10 guests. Ages are 5, 6, 5, 7, 8, 4, 5, 6, 7, 5. Budget is 500. Food portion is 2. Activity is 60 minutes. Venue is open for 4 hours. Vendors: Cake at 50, DJ at 150."

**🤖 AI Agent:**
> Here is your party plan: Timeline: 0:00 Arrival, 0:30 Activity starts, 1:30 Activity ends, 2:00 Departure. Shopping List: 20 food units. Staffing: 3 supervisors needed. Total Cost: 200.

---

**👤 You:**
> "How much food do I need for 5 guests aged 25, 30, 28, 35, and 40 if the baseline portion is 3?"

**🤖 AI Agent:**
> You will need 15 total food units.

---

**👤 You:**
> "Is a budget of 100 enough for a 50 dollar cake and 60 dollar entertainer?"

**🤖 AI Agent:**
> No, the total cost of 110 exceeds your budget of 100.


## ❓ FAQ

**Q: How do I plan a full party with one command?**
You can use the `plan_party_logistics` tool, which takes your guest count, ages, budget, and vendor costs to produce a complete timeline and shopping list.

**Q: Can I check if my party is within budget?**
Yes, the `verify_budget_feasibility` tool allows you to compare your total estimated costs against your available funds.

**Q: How is staffing calculated?**
The `estimate_staffing_needs` tool calculates the required number of supervisors based on the age distribution of your guests.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/birthday-party-planner](https://vinkius.com/en/ai-agent-connect/birthday-party-planner)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Birthday Party Planner** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `birthday-party-planner` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Birthday Party Planner** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "birthday-party-planner": {
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
