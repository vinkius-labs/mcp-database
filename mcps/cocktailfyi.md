# CocktailFyi MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/cocktailfyi)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/cocktailfyi-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/cocktailfyi-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Explore cocktails, ingredients, and bartending techniques — get recipes and guides via AI.

## Description
Connect **CocktailFyi**, the comprehensive cocktail database, to any AI agent and explore hundreds of cocktail recipes, ingredients, bartending techniques, and educational guides through natural language.

### What you can do

- **Cocktail Recipes** — Browse 600+ cocktails with complete recipes, ingredients, measurements, and step-by-step instructions
- **Ingredient Database** — Explore spirits, mixers, garnishes, and bitters used in cocktails
- **Flavor Profiles** — View sweetness, sourness, bitterness, and strength ratings for each cocktail
- **Bartending Techniques** — Learn when to shake, stir, muddle, or build a drink
- **Educational Content** — Access guides, glossary terms, and FAQs about mixology
- **Search & Filter** — Find cocktails by name, ingredient, or category

### How it works

1. Subscribe to this server
2. No API key required — CocktailFyi is free and open
3. Start exploring cocktails from Claude, Cursor, or any MCP-compatible client


## Available Tools
- **get_cocktail**: Get detailed cocktail information
- **get_cocktails_by_category**: Get cocktails filtered by category
- **get_ingredient**: Get detailed ingredient information
- **get_cocktail_stats**: Get CocktailFyi database statistics
- **list_categories**: List cocktail categories
- **list_cocktails**: Each cocktail includes name, category, glass type, alcoholic status, difficulty, prep time, ABV, calories, flavor profile, ingredients, and instructions.

List cocktails with pagination
- **list_faqs**: List frequently asked questions about cocktails
- **list_glossary**: List cocktail glossary terms
- **list_guides**: List cocktail-making guides
- **list_ingredients**: List all cocktail ingredients
- **list_techniques**: with descriptions of when and how to use each.

List cocktail preparation techniques
- **search_cocktails**: Returns results matching the query term in cocktail names, ingredient names, or guide titles.

Search cocktails by name or ingredients


## 💬 Prompt Examples

Here are some examples of how you can interact with the **CocktailFyi** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Give me a classic Mojito recipe."

**🤖 AI Agent:**
> Here's the classic Mojito: White rum, fresh lime juice, simple syrup, fresh mint leaves, and soda water. Served in a Highball glass. Muddle mint with syrup, add lime juice and rum, top with soda water and ice. Difficulty: easy, Prep time: 3 min.

---

**👤 You:**
> "What cocktails can I make with tequila?"

**🤖 AI Agent:**
> Found 45 tequila cocktails including Margarita, Tequila Sunrise, Paloma, Tomatini, and Tequila Sour. Top picks: Margarita (easy, 5 min), Paloma (easy, 3 min), and Tequila Sunrise (medium, 5 min).

---

**👤 You:**
> "What's the difference between shaking and stirring a cocktail?"

**🤖 AI Agent:**
> Shaking is used for cocktails with citrus, dairy, or egg ingredients — it aerates and chills quickly. Stirring is for spirit-forward cocktails like Manhattans and Martinis — it gently chills without clouding or over-diluting. The technique affects texture, temperature, and dilution.


## Installation & Usage

To install and use the **CocktailFyi** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/cocktailfyi](https://vinkius.com/mcp/cocktailfyi)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
