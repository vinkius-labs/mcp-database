# API Ninjas Nutrition MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/api-ninjas-nutrition)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [data-analytics](../categories/data-analytics.md)

Fast, NLP-powered food nutrition analysis — type any food description and get instant calorie, protein, fat, carb, fiber, and sugar data.

## Description
The **API Ninjas Nutrition MCP Server** provides fast, lightweight nutritional analysis using natural language processing. Successor to the popular CalorieNinjas API.

### Core Capabilities

- **NLP Food Analysis** — Type any food in plain English (e.g. "1 lb brisket", "200g salmon", "3 eggs") and get instant nutrient breakdown.
- **Comprehensive Data** — Returns calories, protein, total fat, saturated fat, carbs, fiber, sugar, sodium, and cholesterol.
- **Recipe Search** — Find recipes by keyword with serving information.
- **Per-Serving Data** — All nutrition data is returned per serving size in grams.

Free API key with rate limits. Simple X-Api-Key header authentication.


## Available Tools
- **ninja_analyze_nutrition**: g. "1 lb brisket", "200g salmon", "3 eggs and 2 slices of toast") and get instant nutritional data: calories, protein, fat, carbs, fiber, sugar, sodium, and cholesterol. Fast NLP-powered analysis.

Analyze nutritional content of any food using natural language
- **ninja_search_recipes**: Returns recipe titles and serving information.

Search for recipes by name or keyword


## 💬 Prompt Examples

Here are some examples of how you can interact with the **API Ninjas Nutrition** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "How many calories in 200g of grilled salmon?"

**🤖 AI Agent:**
> 200g of grilled salmon contains approximately 412 calories, 40g protein, 27g fat (4.4g saturated), 0g carbs, and 0g fiber. It's also a rich source of omega-3 fatty acids. Cholesterol: 126mg, Sodium: 98mg.


## ❓ FAQ

**Q: How does it compare to Nutritionix?**
API Ninjas Nutrition is simpler and faster for basic lookups. It's the spiritual successor to CalorieNinjas. Use Nutritionix for branded/restaurant data and more advanced NLP, or API Ninjas for quick, lightweight analysis.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/api-ninjas-nutrition](https://vinkius.com/mcp/api-ninjas-nutrition)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **API Ninjas Nutrition** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `api-ninjas-nutrition` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **API Ninjas Nutrition** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "api-ninjas-nutrition": {
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
