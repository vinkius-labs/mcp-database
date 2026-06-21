# USDA FoodData Central MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/usda-fooddata-central)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [industry-titans](../categories/industry-titans.md)

Access the gold standard in nutrition data — 300,000+ foods with scientific-grade nutrient profiles from the U.S. Department of Agriculture.

## Description
The **USDA FoodData Central MCP Server** provides access to the most authoritative nutrition database in the world. Maintained by the U.S. Department of Agriculture, it covers foundation foods, branded products, and survey data.

### Core Capabilities

- **Food Search** — Find any food by name and get instant nutritional breakdown.
- **Detailed Profiles** — Complete macro and micronutrient data including all vitamins, minerals, amino acids, and fatty acids.
- **Multiple Data Types** — Foundation (research-grade), SR Legacy (historical), Branded (commercial products), and Survey (consumption patterns).

Free API key required (instant registration). The definitive source for nutrition research, dietary analysis, and health applications.


## Available Tools
- **get_usda_food_details**: Get detailed nutritional information for a specific food by its USDA FDC ID
- **search_usda_foods**: S. Department of Agriculture food database containing 300,000+ foods. Returns calories, protein, fat, carbs, fiber, and sugar per serving. Covers foundation foods, branded products, and survey data.

Search the USDA FoodData Central database for foods and their nutritional profiles


## 💬 Prompt Examples

Here are some examples of how you can interact with the **USDA FoodData Central** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "How many calories are in 100g of chicken breast?"

**🤖 AI Agent:**
> According to USDA data, 100g of raw chicken breast contains approximately 165 kcal, 31g protein, 3.6g fat, and 0g carbohydrates. It's an excellent source of lean protein with minimal fat content.

---

**👤 You:**
> "Find a list of foods with the highest vitamin D content per 100g."

**🤖 AI Agent:**
> Accessing USDA database for Vitamin D (Nutrient ID: 328)...
Top sources per 100g:
1. Cod liver oil — 250 µg
2. Salmon (sockeye, cooked) — 16.7 µg
3. Mushrooms (exposed to UV) — 10.7 µg
4. Mackerel (Atlantic, cooked) — 16.1 µg

---

**👤 You:**
> "Look up the exact fat profile (saturated, monounsaturated, polyunsaturated) of an avocado."

**🤖 AI Agent:**
> Parsing profile for 'Avocados, raw' (FDC ID: 171705). Per 100g:
- Total Fat: 14.7g
  - Saturated: 2.13g
  - Monounsaturated: 9.8g (primarily oleic acid)
  - Polyunsaturated: 1.82g


## ❓ FAQ

**Q: How do I get a USDA API key?**
Register for a free API key at fdc.nal.usda.gov/api-key-signup.html. Approval is instant — no wait time required.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/usda-fooddata-central](https://vinkius.com/mcp/usda-fooddata-central)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **USDA FoodData Central** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `usda-fooddata-central` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **USDA FoodData Central** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "usda-fooddata-central": {
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
