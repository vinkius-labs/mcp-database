# Nutritionix MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/nutritionix)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [data-analytics](../categories/data-analytics.md)

Analyze food nutrition from natural language using the industry-leading NLP engine — type any meal description and get instant, precise calorie and macro data.

## Description
The **Nutritionix MCP Server** gives your AI agent access to the industry's most advanced natural language food analysis engine.

### Core Capabilities

- **NLP Food Analysis** — Type anything like "3 slices of pizza and a diet coke" and get instant, precise nutritional breakdown per item.
- **Comprehensive Macros** — Returns calories, protein, fat, carbs, fiber, sugar, sodium, and cholesterol per serving.
- **Instant Search** — Search the Nutritionix database of common and branded foods including restaurant chains.
- **Restaurant Coverage** — Extensive menu item data from national and regional restaurant chains.

Requires app_id and app_key from Nutritionix. The gold standard for NLP food tracking used by major fitness and health apps.


## Available Tools (2)
- **analyze_food_nutrition**: g. "3 slices of pizza and a coke", "1 cup of brown rice", "grilled salmon 200g") and get instant, precise nutritional breakdown including calories, protein, fat, carbs, fiber, sugar, sodium, and cholesterol. The most advanced NLP food parsing engine available.

Analyze nutritional content of any food using natural language — powered by Nutritionix NLP
- **search_nutritionix_foods**: Returns both generic foods and brand-specific items with calorie data.

Search Nutritionix for common and branded food items


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Nutritionix** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Analyze the nutrition of 2 eggs, 1 toast with butter, and a glass of orange juice."

**🤖 AI Agent:**
> Here's your breakfast breakdown:
- 2 large eggs: 144 kcal, 12g protein, 10g fat
- 1 piece of toast with butter: 166 kcal, 3g protein, 6g fat, 24g carbs
- 1 glass OJ (240ml): 112 kcal, 2g protein, 26g carbs

Total: 422 kcal, 17g protein, 16g fat, 50g carbs.

---

**👤 You:**
> "Calculate the macros for 1 cup of oatmeal with a sliced banana and a tablespoon of peanut butter."

**🤖 AI Agent:**
> Breakdown:
- 1 cup cooked oatmeal: 166 kcal, 6g protein, 28g carbs, 4g fiber
- 1 medium banana: 105 kcal, 1.3g protein, 27g carbs
- 1 tbsp peanut butter: 94 kcal, 4g protein, 8g fat
Total: 365 kcal, 11g protein, 63g carbs, 10g fat.

---

**👤 You:**
> "How many calories in a Starbucks Grande Caramel Macchiato with almond milk?"

**🤖 AI Agent:**
> A Starbucks Grande (16 oz) Caramel Macchiato made with almond milk contains approximately 190 calories, 4g of protein, 5g of fat, and 27g of carbohydrates (including 25g of sugar).


## ❓ FAQ

**Q: How accurate is the NLP food analysis?**
Nutritionix's NLP engine is used by major fitness and health apps globally. It can parse complex meal descriptions including quantities, cooking methods, and brand names with high accuracy, backed by a verified database of 1M+ food items.

**Q: Can it recognize branded foods or restaurant items?**
Yes, Nutritionix excels at this. If you type '1 Big Mac and a medium fries from McDonald's', it will correctly map these to specific branded items in its database.

**Q: Does it track micronutrients?**
Yes, in addition to macros (proteins, fats, carbs), it returns data on dietary fiber, sugars, sodium, cholesterol, and potassium for an incredibly comprehensive nutritional profile.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/nutritionix](https://vinkius.com/mcp/nutritionix)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Nutritionix** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `nutritionix` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Nutritionix** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "nutritionix": {
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
