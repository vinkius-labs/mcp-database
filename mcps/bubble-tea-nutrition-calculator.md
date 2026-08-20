# Bubble Tea Nutrition Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/bubble-tea-nutrition-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [nutrition](../categories/nutrition.md)

Calculate calories, sugar, and caffeine for customized bubble tea drinks.

## Description
This MCP server provides precise nutritional estimation for bubble tea customizations. Use `calculate_drink_nutrition` to get a full profile including calories, sugar, and caffeine based on drink type, size, sugar level, ice preference, and toppings. It also includes `get_topping_nutrition` for individual ingredient lookups and `validate_customization_params` to ensure your order parameters are valid.


## Available Tools (3)
- **get_topping_nutrition**: Retrieves the calorie and sugar information for a specific topping
- **validate_customization_params**: Checks if a combination of parameters is valid before performing heavy calculations
- **calculate_drink_nutrition**: Calculates the full nutritional profile of a customized bubble tea order


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Bubble Tea Nutrition Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "How many calories and how much sugar are in a 500ml milk tea with 70% sugar, no ice, and boba?"

**🤖 AI Agent:**
> A 500ml milk tea with 70% sugar, no ice, and boba contains 485.5 calories and 52.3 grams of sugar. Note: This drink exceeds the 50g sugar limit.

---

**👤 You:**
> "What is the caffeine content of a 400ml fruit tea with normal ice?"

**🤖 AI Agent:**
> A 400ml fruit tea with normal ice contains approximately 45mg of caffeine.

---

**👤 You:**
> "Check if my customization is valid: cheese_tea, 30% sugar, and less_ice."

**🤖 AI Agent:**
> The customization parameters are valid.


## ❓ FAQ

**Q: How does ice level affect the nutrition calculation?**
If you select `no_ice`, the liquid volume increases by 15% to fill the cup, which proportionally increases the base calories and sugar content.

**Q: Will I get a warning if my drink is too sweet?**
Yes, the `calculate_drink_nutrition` tool triggers a high sugar warning if the total sugar exceeds 50 grams.

**Q: Can I check the calories of a specific topping?**
Yes, you can use the `get_topping_nutrition` tool to retrieve the specific calorie and sugar values for any available topping.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/bubble-tea-nutrition-calculator](https://vinkius.com/ai-agent-connect/bubble-tea-nutrition-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Bubble Tea Nutrition Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `bubble-tea-nutrition-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Bubble Tea Nutrition Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "bubble-tea-nutrition-calculator": {
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
