# Edamam MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/edamam)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [artificial-intelligence](../categories/artificial-intelligence.md)

Analyze nutrition from natural language, search recipes with dietary filters, and access a comprehensive food database with Edamam's AI-powered platform.

## Description
The **Edamam MCP Server** brings advanced nutritional intelligence to your AI agent. Edamam's unique NLP engine can parse any food description in natural language and return instant, precise nutritional analysis.

### Core Capabilities

- **Natural Language Nutrition** — Type "1 cup brown rice and 200g chicken breast" and get instant calorie, protein, fat, carb, and fiber breakdown. No structured input needed.
- **Recipe Search** — Search recipes with advanced filters for cuisine, diet, and health labels (gluten-free, vegan, keto, peanut-free, etc.).
- **Dietary Intelligence** — Built-in support for 40+ health and diet labels including allergen-free variants.

Free developer tier available. Requires app_id and app_key from the Edamam developer portal. The most advanced nutrition analysis engine available.


## Available Tools (2)
- **analyze_nutrition**: g. "1 cup brown rice", "200g chicken breast", "1 large avocado") and get instant calorie, protein, fat, carb, and fiber breakdown. Powered by Edamam's NLP nutrition engine.

Analyze the nutritional content of any food or ingredient using natural language
- **search_edamam_recipes**: Supports filtering by cuisine type (American, Asian, Chinese, French, Indian, Italian, Japanese, Mediterranean, Mexican), diet (balanced, high-fiber, high-protein, low-carb, low-fat, low-sodium), and health labels (alcohol-free, dairy-free, gluten-free, keto-friendly, peanut-free, vegan, vegetarian).

Search the Edamam recipe database with advanced dietary and health filters


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Edamam** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "How many calories in 2 eggs and a slice of avocado toast?"

**🤖 AI Agent:**
> I've analyzed your meal: 2 large eggs and 1 slice of avocado toast contains approximately 420 calories, 24g protein, 28g fat, 20g carbs, and 5g fiber. The eggs contribute most of the protein while the avocado provides healthy monounsaturated fats.

---

**👤 You:**
> "Find 3 gluten-free dinner recipes with chicken."

**🤖 AI Agent:**
> I found several gluten-free chicken dinner recipes. Here are the top 3: 1. Lemon Herb Roast Chicken, 2. Gluten-Free Chicken Piccata, 3. One-Pan Chicken and Veggies. Shall I fetch the full ingredients for one of them?

---

**👤 You:**
> "Analyze the nutrition for a peanut butter sandwich."

**🤖 AI Agent:**
> Here is the nutritional breakdown for 1 peanut butter sandwich (2 slices of wheat bread and 2 tbsp peanut butter): approximately 330 calories, 12g of protein, 17g of fat, and 34g of carbohydrates.


## ❓ FAQ

**Q: How does the natural language nutrition analysis work?**
Simply type any food description — like '2 eggs and 1 slice of toast with butter' — and Edamam's NLP engine will parse the text, identify each ingredient, and return precise calorie and nutrient data. No need for structured inputs or food IDs.

**Q: Does the API offer filters for vegan or paleo diets?**
Yes, the recipe tool provides extensive dietary and health label filters including 'vegan', 'paleo', 'keto-friendly', 'gluten-free', and many more.

**Q: Are both API endpoints completely free?**
Yes, Edamam offers a Developer tier that is free of charge for both the Recipe Search API and the Nutrition Analysis API with certain monthly limits.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/edamam](https://vinkius.com/mcp/edamam)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Edamam** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `edamam` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Edamam** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "edamam": {
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
