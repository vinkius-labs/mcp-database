# School Lunch Prep Plan MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/school-lunch-prep-plan)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [logistics](../categories/logistics.md)

Generate precise lunch portions, grocery lists, and prep schedules for school lunches.

## Description
This MCP server helps families manage school lunch logistics by calculating exact portion requirements and optimized preparation workflows. Use `calculate_meal_requirements` to determine total servings and daily volume, `generate_shopping_list` to compile ingredient needs, and `create_prep_schedule` to organize tasks into time-blocked segments. It also includes `validate_dietary_safety` to check for allergens and `verify_container_fit` to ensure portions fit in lunch boxes.


## Available Tools (5)
- **calculate_meal_requirements**: Determines the total number of servings and volume requirements for a set of planned recipes
- **generate_shopping_list**: Compiles a complete list of ingredients and quantities needed to fulfill the meal plan
- **validate_dietary_safety**: Checks if the selected recipes are safe for all children based on their specific dietary exclusions
- **create_prep_schedule**: Decomposes the necessary meal preparation into logical, time-stamped blocks
- **verify_container_fit**: Ensures that the portions calculated for a recipe will actually fit into the available lunch containers


## 💬 Prompt Examples

Here are some examples of how you can interact with the **School Lunch Prep Plan** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "I need to plan lunches for 2 children for 5 school days using recipe IDs 'pasta_01' and 'salad_02'. How many servings and what volume do I need?"

**🤖 AI Agent:**
> You will need a total of 10 servings. The required volume per day is calculated based on the combined volume of the pasta and salad recipes.

---

**👤 You:**
> "Generate a shopping list for these recipes: 'taco_01, chicken_02' with a scale factor of 3."

**🤖 AI Agent:**
> The shopping list includes 3x the required ingredients for tacos and chicken, such as ground beef, taco shells, chicken breast, and seasoning.

---

**👤 You:**
> "Will a 500ml portion fit in my 450ml lunch container?"

**🤖 AI Agent:**
> No, the portion will not fit. There is an overflow volume of 50ml.


## ❓ FAQ

**Q: How do I know if my recipes are safe for my children?**
You can use the `validate_dietary_safety` tool to check if any selected recipes contain ingredients listed in your children's dietary exclusions.

**Q: Can I plan for multiple children at once?**
Yes, the `calculate_meal_requirements` tool allows you to specify the total number of children to ensure accurate portioning.

**Q: How does the prep schedule work?**
The `create_prep_schedule` tool breaks down the necessary tasks into logical blocks based on the total time you have available for preparation.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/school-lunch-prep-plan](https://vinkius.com/en/ai-agent-connect/school-lunch-prep-plan)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **School Lunch Prep Plan** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `school-lunch-prep-plan` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **School Lunch Prep Plan** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "school-lunch-prep-plan": {
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
