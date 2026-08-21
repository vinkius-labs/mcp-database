# Singapore Hawker Macro Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/singapore-hawker-macro-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [health](../categories/health.md)

Get precise nutritional data and Nutri-Grade ratings for Singaporean hawker dishes.

## Description
This MCP server provides deterministic nutritional analysis for Singaporean hawker food. It uses fixed Health Promotion Board (HPB) values to calculate calories, proteins, carbohydrates, fats, and sodium. Users can specify portion sizes and dietary modifications to see exact macro adjustments. Use `calculate_dish_macros` to get a full nutritional profile and Nutri-Grade, `get_available_dishes` to browse supported meals, or `get_modification_impacts` to see how specific changes like 'no_skin' affect your meal.


## Available Tools (3)
- **get_available_dishes**: Allows the user to see which hawker dishes are supported by the calculator
- **calculate_dish_macros**: Calculates the base and adjusted nutritional profile of a specific hawker dish
- **get_modification_impacts**: Informs the user of the specific nutritional changes associated with common modifications


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Singapore Hawker Macro Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What are the macros for a regular portion of chicken rice with no skin?"

**🤖 AI Agent:**
> A regular portion of chicken rice with no skin has 520 calories, 22g of protein, 65g of carbs, and 18g of fat, with a Nutri-Grade B.

---

**👤 You:**
> "Show me all available noodle dishes."

**🤖 AI Agent:**
> The available noodle dishes are laksa, char kway teow, and mee pok.

---

**👤 You:**
> "How much fat do I save if I ask for less oil in my dish?"

**🤖 AI Agent:**
> Requesting 'less_oil' reduces the total fat content by 5g.


## ❓ FAQ

**Q: How accurate are these nutritional values?**
The values are deterministic and based on fixed Health Promotion Board (HPB) data for standard hawker portions.

**Q: Can I adjust for specific dietary needs?**
Yes, you can use `calculate_dish_macros` with the `modifications` parameter to account for changes like 'no_skin' or 'less_oil'.

**Q: What is a Nutri-Grade?**
Nutri-Grade is a Singaporean health rating system (A to D) that assesses the nutritional profile of food based on energy, sugar, and saturated fat.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/singapore-hawker-macro-calculator](https://vinkius.com/ai-agent-connect/singapore-hawker-macro-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Singapore Hawker Macro Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `singapore-hawker-macro-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Singapore Hawker Macro Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "singapore-hawker-macro-calculator": {
      "url": "https://edge.vinkius.com/[TOKEN]/mcp"
    }
  }
}
```

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
