# Dinner Party Quantity Planner MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/dinner-party-quantity-planner)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [logistics](../categories/logistics.md)

Calculate precise food, drink, ice, and supply quantities for any event.

## Description
Plan your event logistics with precision. This MCP server provides tools to calculate exact requirements for food, beverages, ice, and disposable supplies. Use `calculate_food_requirements` to determine food weights or counts, `calculate_beverage_requirements` to estimate drink volumes based on event duration, `calculate_ice_needs` for chilling requirements, and `calculate_supply_requirements` for plates and cutlery.


## Available Tools (4)
- **calculate_food_requirements**: Determine the total weight or unit count of food needed for the menu
- **calculate_beverage_requirements**: Estimate the volume of various drinks needed based on time
- **calculate_ice_needs**: Calculate the weight of ice needed for chilling and serving
- **calculate_supply_requirements**: Determine the count of disposable plates, cutlery, and napkins


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Dinner Party Quantity Planner** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "How much food do I need for 10 guests with 2 appetizers (50g each) and 1 main course (250g each)?"

**🤖 AI Agent:**
> You will need 500g of appetizers and 2500g of the main course.

---

**👤 You:**
> "How much wine should I get for 20 guests for a 4-hour party if they drink 0.5 liters per hour?"

**🤖 AI Agent:**
> You will need 40 liters of wine.

---

**👤 You:**
> "How many plates and napkins do I need for 15 guests having a 3-course meal?"

**🤖 AI Agent:**
> You will need 45 plates and 45 napkins.


## ❓ FAQ

**Q: How does the tool handle leftovers?**
You can specify a `leftoverBufferPercentage` in the `calculate_food_requirements` tool to add a surplus to your total food quantities.

**Q: Can I calculate ice needs for chilling drinks?**
Yes, by using `calculate_ice_needs` and setting the `isChillingRequired` parameter to true, the tool adjusts the ice weight for chilling.

**Q: How are beverage amounts calculated?**
The `calculate_beverage_requirements` tool calculates volume based on the number of guests, the total duration of the event, and the specific consumption rate per hour for each drink type.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/dinner-party-quantity-planner](https://vinkius.com/en/ai-agent-connect/dinner-party-quantity-planner)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Dinner Party Quantity Planner** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `dinner-party-quantity-planner` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Dinner Party Quantity Planner** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "dinner-party-quantity-planner": {
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
