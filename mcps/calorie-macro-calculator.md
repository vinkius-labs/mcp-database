# Calorie & Macro Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/calorie-macro-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [health](../categories/health.md)

Calculate daily caloric needs and macronutrient split based on physiological metrics and activity levels.

## Description
This MCP server provides a precise nutrition engine to determine your daily energy requirements. Using the Mifflin-St Jeor equation, you can use `calculate_bmr` to find your Basal Metabolic Rate. From there, `calculate_tdee` adjusts for activity levels and dietary goals like cutting or bulking. The `distribute_macronutrients` tool calculates specific protein, carbohydrate, and fat gram targets based on diet types such as keto, balanced, or athlete. Finally, `generate_meal_breakdown` partitions these macros into a structured per-meal plan to help you stay on track with your nutrition.


## Available Tools (4)
- **calculate_bmr**: Requires weight, height, age, and biological sex.

Calculate Basal Metabolic Rate (BMR)
- **distribute_macronutrients**: Distribute calories into macronutrients
- **generate_meal_breakdown**: Partition daily macros into meals
- **calculate_tdee**: Calculate Total Daily Energy Expenditure (TDEE)


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Calorie & Macro Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Calculate my BMR for a 30 year old male, 85kg, 180cm."

**🤖 AI Agent:**
> Your Basal Metabolic Rate (BMR) is 1849 kcal/day.

---

**👤 You:**
> "I have a TDEE of 2500 kcal. How many grams of protein, carbs, and fats do I need for a keto diet on a training day?"

**🤖 AI Agent:**
> For a keto diet at 2500 kcal, you need 156g of protein, 31g of carbohydrates, and 194g of fats.

---

**👤 You:**
> "Split 200g protein, 300g carbs, and 70g fat into 4 meals."

**🤖 AI Agent:**
> Meal 1: 50g Protein, 75g Carbs, 17.5g Fat (Total: 585 kcal). Meal 2: 50g Protein, 75g Carbs, 17.5g Fat (Total: 585 kcal). Meal 3: 50g Protein, 75g Carbs, 17.5g Fat (Total: 585 kcal). Meal 4: 50g Protein, 75g Carbs, 17.5g Fat (Total: 585 kcal).


## ❓ FAQ

**Q: How is my BMR calculated?**
The `calculate_bmr` tool uses the Mifflin-St Jeor Equation, which considers your weight, height, age, and biological sex for high accuracy.

**Q: Can I adjust my macros for different diets?**
Yes, using `distribute_macronutrients`, you can choose between keto, balanced, or athlete diet types to get specific gram targets.

**Q: Does it account for training days?**
Yes, the `distribute_macronutrients` tool allows you to specify if it is a training day, which adjusts your carbohydrate targets accordingly.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/calorie-macro-calculator](https://vinkius.com/mcp/calorie-macro-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Calorie & Macro Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `calorie-macro-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Calorie & Macro Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "calorie-macro-calculator": {
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
