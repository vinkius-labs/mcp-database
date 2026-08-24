# Fruit Portion Sizing Engine MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/fruit-portion-sizing-engine)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [health](../categories/health.md)

Calculate exact fruit portions to hit a 15g carbohydrate target.

## Description
This MCP server provides precise tools for diabetic portion control by calculating the exact mass and volume of fruit needed to reach a standardized 15g carbohydrate target. Using the `calculate_portion_size` tool, users can determine the specific grams, volume equivalent, sugar content, and fiber content for various fruits. You can also use `get_fruit_nutritional_profile` to see density data or `list_supported_fruits` to see available options. It is designed to help manage blood glucose levels through accurate carbohydrate counting.


## Available Tools (3)
- **calculate_portion_size**: Determines the precise weight and nutritional breakdown of a fruit to reach exactly 15g of carbohydrates
- **list_supported_fruits**: Provides a list of all fruits currently supported by the engine
- **get_fruit_nutritional_profile**: Retrieves the baseline nutritional density (carbs, sugar, fiber) for a specific fruit type


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Fruit Portion Sizing Engine** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "How many grams of strawberries do I need for 15g of carbs?"

**🤖 AI Agent:**
> To reach 15g of carbohydrates, you need 150g of strawberries, which is approximately 1 cup.

---

**👤 You:**
> "What is the portion size for an apple to get 15g of carbs?"

**🤖 AI Agent:**
> You need 115g of apple, which is equivalent to one small apple.

---

**👤 You:**
> "How much watermelon should I eat for a 15g carb serving?"

**🤖 AI Agent:**
> You should eat 210g of watermelon to hit the 15g carbohydrate target.


## ❓ FAQ

**Q: What is the carbohydrate target for these calculations?**
The engine is hardcoded to target exactly 15 grams of carbohydrates, which is the standard serving size used in carbohydrate counting.

**Q: How can I see which fruits are available?**
You can use the `list_supported_fruits` tool to get a complete list of all fruit types currently supported by the engine.

**Q: Does this tool provide volume measurements?**
Yes, the `calculate_portion_size` tool provides a `volumeEquivalent` (such as '1 cup' or '1/2 medium banana') to make measuring easier in a kitchen setting.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/fruit-portion-sizing-engine](https://vinkius.com/ai-agent-connect/fruit-portion-sizing-engine)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Fruit Portion Sizing Engine** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `fruit-portion-sizing-engine` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Fruit Portion Sizing Engine** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "fruit-portion-sizing-engine": {
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
