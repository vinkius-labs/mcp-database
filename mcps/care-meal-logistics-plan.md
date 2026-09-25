# Care Meal Logistics Plan MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/care-meal-logistics-plan)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Automated coordination for meal delivery, shopping, and storage logistics.

## Description
This MCP server automates the complex logistics of meal management. It connects AI agents to tools that generate cohesive meal delivery schedules using `plan_meal_schedule`, create detailed shopping lists with `generate_shopping_assignments`, organize food storage with `create_storage_checklist`, and establish user feedback loops via `setup_feedback_loop`. It ensures dietary restrictions, budget constraints, and storage capacities are strictly respected.


## Available Tools (4)
- **create_storage_checklist**: Creates a spatial plan to ensure all food fits in available storage
- **generate_shopping_assignments**: Breaks down required food items into specific shopping tasks
- **plan_meal_schedule**: Generates a cohesive timeline for meal arrival and consumption
- **setup_feedback_loop**: Establishes the mechanism for users to report issues with the plan


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Care Meal Logistics Plan** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Create a meal schedule for Italian food with home delivery, assuming a helper is available between 10 AM and 2 PM."

**🤖 AI Agent:**
> 10:00 AM: Meal Delivery (Assigned to Helper A)
12:30 PM: Meal Service (Assigned to Helper A)

---

**👤 You:**
> "Generate a shopping list for a Mediterranean meal plan with a budget of $50 and no peanuts."

**🤖 AI Agent:**
> 1. Greek Salad ($12.00, Produce)
2. Chicken Breast ($15.00, Meat)
3. Feta Cheese ($8.00, Dairy)
4. Olives ($6.00, Pantry)
5. Cucumber ($4.00, Produce)

---

**👤 You:**
> "Check if these items will fit in my small fridge: milk, eggs, yogurt, and butter."

**🤖 AI Agent:**
> Milk: Fridge (Fits)
Eggs: Fridge (Fits)
Yogurt: Fridge (Fits)
Butter: Fridge (Fits)


## ❓ FAQ

**Q: How does the tool handle dietary restrictions?**
The `generate_shopping_assignments` tool filters all items against the provided dietary restrictions to ensure no prohibited ingredients are included in the shopping list.

**Q: Can I schedule deliveries if no one is home?**
No. The `plan_meal_schedule` tool requires helper availability. If a requested delivery window does not align with when a helper is present, the tool will return an error.

**Q: How do I know if my food will fit in my fridge?**
You can use `create_storage_checklist` by providing your available storage capacity. The tool will then provide a checklist indicating if items fit or if space is tight.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/care-meal-logistics-plan](https://vinkius.com/en/ai-agent-connect/care-meal-logistics-plan)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Care Meal Logistics Plan** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `care-meal-logistics-plan` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Care Meal Logistics Plan** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "care-meal-logistics-plan": {
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
