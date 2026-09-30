# Home Dinner Host Plan MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/home-dinner-host-plan)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Complete management for hosting dinner parties, from menu design to cleanup.

## Description
This MCP server provides a complete suite of tools to manage every phase of hosting a dinner party. Use `plan_dinner_menu` to design a menu that respects dietary restrictions, `generate_shopping_list` to consolidate ingredients, `create_execution_timeline` to work backward from serving time, and `verify_hosting_resources` to ensure you have enough plates and cutlery for your guests.


## Available Tools (4)
- **create_execution_timeline**: Generate a step-by-step schedule for the host
- **plan_dinner_menu**: Design a menu based on guest requirements and desired course structure
- **generate_shopping_list**: Create a consolidated list of items to purchase
- **verify_hosting_resources**: Ensure the host has sufficient physical items for the guest count


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Home Dinner Host Plan** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Plan a 3-course dinner for 6 guests, including an appetizer, main, and dessert, with no gluten."

**🤖 AI Agent:**
> I have designed a gluten-free menu for 6 guests consisting of Caprese Salad, Roasted Chicken with Vegetables, and Fruit Sorbet.

---

**👤 You:**
> "Create a timeline for my dinner menu (ID: menu_123) to be served at 7:00 PM tonight."

**🤖 AI Agent:**
> To serve at 7:00 PM, you should begin preparation at 4:30 PM, start cooking the main course at 5:45 PM, and set the table at 6:30 PM.

---

**👤 You:**
> "Generate a shopping list for menu ID menu_456, but I already have salt, pepper, and olive oil."

**🤖 AI Agent:**
> Your shopping list includes 500g of pasta, 200g of parmesan cheese, and 500g of ground beef. Salt, pepper, and olive oil are already in your pantry.


## ❓ FAQ

**Q: How do I plan a menu for guests with allergies?**
You can use the `plan_dinner_menu` tool by providing the specific dietary restrictions in the input array to ensure all selected recipes are safe.

**Q: Can I account for items I already have in my kitchen?**
Yes, when using `generate_shopping_list`, you can provide your pantry inventory to reduce the items you need to purchase.

**Q: How do I know if I have enough plates for my guests?**
Use the `verify_hosting_resources` tool with your guest count and current inventory to confirm you have sufficient tableware.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/home-dinner-host-plan](https://vinkius.com/en/ai-agent-connect/home-dinner-host-plan)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Home Dinner Host Plan** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `home-dinner-host-plan` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Home Dinner Host Plan** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "home-dinner-host-plan": {
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
