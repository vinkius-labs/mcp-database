# Punk MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/punk)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [developer-tools](../categories/developer-tools.md)

Explore the BrewDog beer catalog — search by ingredients, food pairings, and technical specs like ABV or IBU.

## Description
Access the complete **BrewDog** beer library through the Punk API. This MCP server allows your AI agent to act as a digital sommelier or brewing consultant.

### What you can do

- **Advanced Search** — Filter the catalog by ABV (alcohol by volume), IBU (bitterness), or EBC (color) using precise ranges.
- **Ingredient Analysis** — Search for beers containing specific hops, malts, or yeast strains to understand flavor profiles.
- **Food Pairing** — Get instant recommendations for beers that complement specific dishes or cuisines.
- **Detailed Specs** — Retrieve full recipes, brewing tips, and technical measurements for any beer in the database.
- **Random Discovery** — Let the agent suggest a surprise brew from the extensive collection.

### How it works

1. Subscribe to this server
2. Enter 'OPEN' in the token field (this is a public API)
3. Start exploring recipes and pairings from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Homebrewers** — quickly look up hop profiles and malt bills without leaving your research notes
- **Foodies & Chefs** — find the perfect craft beer to pair with your latest recipe
- **App Developers** — test beer-related data structures and API responses in a conversational environment


## Available Tools
- **get_beer**: Get a single beer by ID
- **list_beers**: Supports pagination and filtering by ABV, IBU, EBC, ingredients, and food pairings.

List beers from the BrewDog catalog
- **get_random_beer**: Get a random beer


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Punk** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List some beers that go well with spicy curry."

**🤖 AI Agent:**
> I've searched the BrewDog catalog for you. Based on your request for spicy curry, I recommend 'Punk IPA' (ID: 192) and 'Jack Hammer' (ID: 37). Both have the bitterness and hop profile to balance the heat. Would you like the full details for one of these?

---

**👤 You:**
> "Show me the details for beer with ID 192."

**🤖 AI Agent:**
> Fetching details for ID 192... This is 'Punk IPA', a Post Modern Classic with 5.6% ABV. It features Chinook, Ahtanum, and Nelson Sauvin hops. It pairs perfectly with spicy meat pizza or burger. Would you like the brewing method details?

---

**👤 You:**
> "Give me a random beer recommendation with an ABV higher than 6%."

**🤖 AI Agent:**
> I'll find a strong random brew for you... I've selected 'Hardcore IPA' (ID: 15). It has a powerful 9.2% ABV and 125 IBU. It's an explicit imperial ale with a massive hop hit. Does this sound like what you're looking for?


## ❓ FAQ

**Q: How can I find beers that pair well with a specific food like 'steak'?**
You can use the `list_beers` tool and provide the `food` parameter with your dish name. The agent will return a list of beers from the BrewDog catalog specifically recommended for that pairing.

**Q: Can I filter beers by their alcohol percentage (ABV)?**
Yes! Use the `list_beers` tool with `abv_gt` (greater than) or `abv_lt` (less than) parameters to find beers within your preferred strength range.

**Q: How do I get the full recipe and details for a specific beer ID?**
Use the `get_beer` tool and provide the unique integer `id`. The agent will retrieve the complete profile, including ingredients, brewing methods, and technical specifications.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/punk](https://vinkius.com/mcp/punk)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Punk** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `punk` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Punk** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "punk": {
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
