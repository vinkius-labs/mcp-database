# BigOven MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/bigoven)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Access over a million recipes via BigOven — search dishes, read reviews, and explore collections directly from any AI agent.

## Description
Connect your **BigOven** account to any AI agent and bring the power of over a million recipes into your workspace through natural conversation.

### What you can do

- **Recipe Discovery** — Search for recipes by title, keyword, or specific ingredients.
- **Deep Dives** — Retrieve full recipe details including ingredients, instructions, and nutritional info.
- **Community Feedback** — Read user reviews and ratings to find the best version of a dish.
- **Curated Collections** — Explore seasonal and thematic recipe collections for inspiration.
- **Media Access** — Retrieve photos and visual guides for recipes to aid in meal planning.

### How it works

1. Subscribe to this server
2. Enter your BigOven API Key
3. Start exploring culinary ideas from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Food Bloggers & Writers** — quickly research ingredients and recipe variations without leaving the editor.
- **Meal Planners** — find recipes based on specific leftover ingredients using natural language.
- **Health & Fitness Coaches** — retrieve nutritional data and recipe ideas to share with clients.


## Available Tools (8)
- **get_recipe_reviews**: Get reviews for a specific recipe
- **get_recipe**: Get full details of a specific recipe
- **list_categories**: List valid recipe categories for filtering
- **list_collections**: List seasonal or curated recipe collections
- **search_by_ingredient**: Search recipes by ingredient keywords
- **search_recipes**: Search recipes by title or keyword
- **get_collection**: Get details and recipes of a specific collection
- **get_recipe_photos**: Retrieve photos for a specific recipe


## 💬 Prompt Examples

Here are some examples of how you can interact with the **BigOven** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Find a good recipe for Lasagna."

**🤖 AI Agent:**
> I found a few highly-rated options. The top result is 'Classic Homemade Lasagna' (ID: 14523) with a 4.8/5 star rating. Would you like the full ingredients list?

---

**👤 You:**
> "Search for recipes using salmon and sweet potato."

**🤖 AI Agent:**
> Searching by ingredients... I found 'Roasted Salmon with Sweet Potato' (ID: 8821) and 'Sweet Potato Salmon Cakes' (ID: 9912). Which one sounds better?

---

**👤 You:**
> "Get the reviews for recipe 14523."

**🤖 AI Agent:**
> Retrieving reviews... Users love this recipe! Common comments mention that adding extra garlic makes the sauce much better, and baking it covered for the first 30 minutes prevents drying.


## ❓ FAQ

**Q: Can I search for recipes based on ingredients I have in my fridge?**
Yes! Use the `search_by_ingredient` tool and provide the ingredients you have (e.g., 'chicken, broccoli'). The agent will return recipes you can make.

**Q: How do I get the step-by-step instructions for a recipe?**
First, find the Recipe ID using the search tools. Then, ask the agent to `get_recipe` with that ID. It will retrieve the full ingredient list and step-by-step instructions.

**Q: Does the integration allow me to add recipes to a grocery list?**
Currently, the toolset is focused on public discovery and searching (Read-Only). Managing personal grocery lists requires user-specific OAuth which is managed directly on the BigOven app.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/bigoven](https://vinkius.com/mcp/bigoven)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **BigOven** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `bigoven` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **BigOven** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "bigoven": {
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
