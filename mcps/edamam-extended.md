# Edamam MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/edamam-extended)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [scientific-research](../categories/scientific-research.md)

Search over 2.3 million recipes, analyze nutritional data, and access a database of 900,000+ food items directly from your AI agent.

## Description
Integrate **Edamam** into your AI workflows to access world-class nutrition and recipe data. Whether you are building a meal planner, a health app, or just looking for cooking inspiration, this server provides the tools to query millions of recipes and analyze ingredients with scientific precision.

### What you can do

- **Recipe Discovery** — Search a massive database of 2.3M+ recipes using keywords, dietary labels (vegan, keto), and cuisine types.
- **Nutrition Analysis** — Get detailed breakdowns of calories, fats, proteins, and micronutrients for any list of ingredients or full recipes.
- **Food Lookup** — Access data for over 900,000 foods, including raw ingredients, restaurant items, and packaged goods using names or UPC codes.
- **Dietary Filtering** — Filter results by health labels, allergens, and specific nutritional goals like high-protein or low-carb.

### How it works

1. Subscribe to this server
2. Enter your Edamam Application ID and Application Key
3. Start querying food and nutrition data from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Health & Wellness Coaches** — generate instant nutritional reports for client meal plans
- **Home Cooks & Foodies** — find recipes that match specific dietary needs or available ingredients
- **Developers** — integrate robust food data into applications without managing complex databases


## Available Tools (3)
- **search_recipes**: 3 million recipes by keywords, dietary restrictions, and other filters.

Search recipes by keywords and filters
- **analyze_nutrition**: Get nutrition facts for a recipe
- **parse_food**: Look up food in the Food Database


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Edamam** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Search for high-protein chicken recipes with an Asian cuisine type."

**🤖 AI Agent:**
> I found several high-protein Asian chicken recipes, including 'Thai Basil Chicken' and 'Ginger Soy Steamed Chicken'. Would you like the full ingredient list for one of these?

---

**👤 You:**
> "Analyze the nutrition for 100g of oats, 1 banana, and 200ml of almond milk."

**🤖 AI Agent:**
> Based on those ingredients, the total is approximately 540 calories, with 82g of carbohydrates, 12g of protein, and 14g of fat. It is also high in fiber and potassium.

---

**👤 You:**
> "Look up the nutritional data for 'Greek Yogurt' in the food database."

**🤖 AI Agent:**
> I've retrieved the data for Greek Yogurt. A standard serving contains high protein levels and active cultures. I can also provide specific brand data if you have a UPC code.


## ❓ FAQ

**Q: Can I search for recipes based on specific dietary restrictions like gluten-free or vegan?**
Yes! Use the `search_recipes` tool and specify your requirements in the `health` or `diet` parameters to filter for labels like 'vegan', 'gluten-free', or 'low-carb'.

**Q: How do I get a detailed nutritional breakdown for a list of ingredients?**
You can use the `analyze_nutrition` tool. Simply provide an array of ingredient strings (e.g., ['1 cup of flour', '2 eggs']), and the agent will return calories and nutrient levels.

**Q: Can I look up specific food items or products using their name or UPC?**
Yes, the `parse_food` tool allows you to look up data for over 900,000 foods by entering the food name or a UPC barcode string.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/edamam-extended](https://vinkius.com/mcp/edamam-extended)
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
3. Set Type to "SSE" (or "streamable HTTP"), enter `edamam-extended` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Edamam** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "edamam-extended": {
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
