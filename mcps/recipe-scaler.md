# Recipe Scaler MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/recipe-scaler)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Precisely scale recipe ingredients while maintaining culinary proportions and practical measurements.

## Description
The Recipe Scaler MCP connects your AI agent to a precision ingredient scaling engine. It ensures that when you change the number of servings in a recipe, the proportions remain perfect and the measurements stay practical for real-world cooking. Using `scale_ingredients`, you can adjust quantities based on serving size changes. The engine uses `resolve_measurement_precision` to determine appropriate rounding increments for different units (like volume or mass) and `format_culinary_units` to convert complex decimals into human-readable kitchen measurements like '1 tbsp + 1 tsp' instead of '1.37 tbsp'. This prevents unusable measurements and maintains the integrity of your culinary creations.


## Available Tools (3)
- **format_culinary_units**: Converts raw decimal quantities into human-readable, practical strings
- **resolve_measurement_precision**: Determines the appropriate rounding increment for a specific unit
- **scale_ingredients**: Scales a recipe based on serving size changes


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Recipe Scaler** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Scale this recipe for 10 people: 2 servings, ingredients: [{name: 'flour', quantity: 500, unit: 'g'}, {name: 'sugar', quantity: 1, unit: 'cup'}]"

**🤖 AI Agent:**
> Scaled ingredients for 10 servings: [{name: 'flour', quantity: 2500, unit: 'g'}, {name: 'sugar', quantity: 5, unit: 'cup'}]

---

**👤 You:**
> "How much sugar do I need if I scale a recipe from 2 to 3 servings, where the original amount was 1.5 tablespoons?"

**🤖 AI Agent:**
> You will need 2.25 tablespoons of sugar.

---

**👤 You:**
> "Convert 0.75 tablespoons to a more practical measurement."

**🤖 AI Agent:**
> 0.75 tablespoons is equivalent to 2.25 teaspoons.


## ❓ FAQ

**Q: How does the scaling engine maintain recipe integrity?**
The engine calculates a precise scaling ratio by dividing target servings by original servings. It then applies this ratio uniformly to every ingredient in the `ingredientsList` via the `scale_ingredients` tool, ensuring flavor and texture profiles remain unchanged.

**Q: Will I get unusable decimal measurements?**
No. The engine uses `format_culinary_units` to convert raw decimals into practical, human-readable strings. It breaks down complex quantities into standard kitchen units (e.g., converting parts of a tablespoon into teaspoons) based on the precision determined by `resolve_measurement_precision`.

**Q: Does it support both Metric and US Imperial systems?**
Yes. The engine is designed to respect both the US Imperial (ounces, pounds, tablespoons) and Metric (grams, kilograms, milliliters) standards, adjusting its precision logic accordingly.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/recipe-scaler](https://vinkius.com/mcp/recipe-scaler)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Recipe Scaler** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `recipe-scaler` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Recipe Scaler** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "recipe-scaler": {
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
