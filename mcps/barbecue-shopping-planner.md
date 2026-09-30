# Barbecue Shopping Planner MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/barbecue-shopping-planner)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [logistics](../categories/logistics.md)

A logistics engine that generates precise shopping lists for food, drinks, ice, fuel, and serving ware.

## Description
This MCP server acts as a complete logistics engine for hosting barbecues. It transforms guest demographics and menu choices into an itemized shopping list. Use `generate_master_shopping_list` to get a unified list of food, beverages, and hardware, or use specific tools like `calculate_food_quantities` and `calculate_beverage_and_ice_needs` for granular planning. It accounts for meat-eaters, vegetarians, children, weather conditions, and cooking methods to ensure you have exactly what you need.


## Available Tools (4)
- **calculate_beverage_and_ice_needs**: Calculates the total liquid volume required and the amount of ice needed to keep drinks cold
- **calculate_food_quantities**: Determines the exact amount of meat, vegetarian main courses, and side dishes needed based on guest demographics
- **calculate_supplies_and_hardware**: Determines the amount of fuel needed for cooking and the count of disposable serving ware
- **generate_master_shopping_list**: Aggregates all calculated requirements into a single, unified list for the user


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Barbecue Shopping Planner** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "I'm hosting a barbecue for 10 meat-eaters, 2 vegetarians, and 3 children. We want burgers and corn on the cob. It's going to be hot weather, we'll use charcoal, and we need a full list including drinks and supplies."

**🤖 AI Agent:**
> Here is your complete shopping list: 
- Food: 3.5kg Burgers, 1.2kg Corn on the cob, 1.5kg Vegetarian patties.
- Beverages: 15 Liters of Soda, 10kg of Ice.
- Hardware: 2kg Charcoal, 15 Plates, 15 Sets of Cutlery, 20 Napkins.

---

**👤 You:**
> "How much ice do I need for 20 people drinking soda for 4 hours in hot weather?"

**🤖 AI Agent:**
> You will need 12kg of ice (approximately 3 bags) to keep the drinks cold for 4 hours in hot weather.

---

**👤 You:**
> "Calculate the food needed for 5 meat-eaters and 5 vegetarians with a menu of hot dogs and veggie skewers."

**🤖 AI Agent:**
> You will need 1.8kg of Hot dogs and 1.2kg of Veggie skewers.


## ❓ FAQ

**Q: How does the tool calculate food amounts?**
The engine uses guest demographics--meat-eaters, vegetarians, and children--to scale portions and applies a safety buffer to ensure you don't run out of food.

**Q: Can I get a single list for everything?**
Yes, by using the `generate_master_shopping_list` tool, you receive a single, categorized list covering food, drinks, ice, fuel, and disposable supplies.

**Q: Does it account for hot weather?**
Yes, the `calculate_beverage_and_ice_needs` tool includes a parameter for hot weather, which increases the recommended ice and liquid volume.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/barbecue-shopping-planner](https://vinkius.com/en/ai-agent-connect/barbecue-shopping-planner)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Barbecue Shopping Planner** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `barbecue-shopping-planner` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Barbecue Shopping Planner** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "barbecue-shopping-planner": {
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
