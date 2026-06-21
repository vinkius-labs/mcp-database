# Nookipedia MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/nookipedia)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [databases](../categories/databases.md)

Access the ultimate Animal Crossing encyclopedia — query villager data, New Horizons items, bugs, fish, and recipes directly from any AI agent.

## Description
Connect to the **Nookipedia API** and bring the entire world of Animal Crossing to your AI agent. Whether you are tracking your museum progress or looking for the perfect gift for a villager, this server provides comprehensive data across the entire series.

### What you can do

- **Villager Database** — Search for villagers by name, species, personality, or game appearance to find their birthdays, catchphrases, and styles.
- **New Horizons Encyclopedia** — Fetch real-time data for bugs, fish, sea creatures, and fossils, including availability and pricing.
- **Item Catalog** — Browse thousands of furniture items, clothing, interior wallpapers, and tools with full metadata.
- **DIY Recipes & Events** — Access crafting requirements for recipes and stay updated on in-game events and seasonal celebrations.
- **Collectibles** — Track photos, posters, and the elusive gyroids to complete your island collection.

### How it works

1. Subscribe to this server
2. Enter your Nookipedia API Key
3. Start exploring the Animal Crossing universe from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Island Designers** — quickly check furniture variations and themes without leaving your planning tools
- **Completionists** — verify museum donation details and seasonal availability for critters
- **Developers & Fans** — build tools or simply chat about your favorite villagers with a knowledgeable AI assistant


## Available Tools
- **get_nh_art**: Retrieve New Horizons artworks
- **get_nh_bugs**: Retrieve New Horizons bugs
- **get_nh_clothing**: Retrieve New Horizons clothing
- **get_nh_events**: Retrieve New Horizons events and dates
- **get_nh_fish**: Retrieve New Horizons fish
- **get_nh_fossils**: Retrieve New Horizons fossils
- **get_nh_furniture**: Retrieve New Horizons furniture
- **get_nh_gyroids**: Retrieve New Horizons gyroids
- **get_nh_interior**: Retrieve New Horizons interior items
- **get_nh_misc**: Retrieve New Horizons miscellaneous items
- **get_nh_photos**: Retrieve New Horizons photos and posters
- **get_nh_recipes**: Retrieve New Horizons recipes
- **get_nh_sea_creatures**: Retrieve New Horizons sea creatures
- **get_nh_tools**: Retrieve New Horizons tools
- **get_villagers**: Can be filtered by name, species, personality, or game.

Retrieve information about villagers across the entire series


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Nookipedia** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Tell me everything about the villager named Raymond."

**🤖 AI Agent:**
> I've found Raymond! He is a Smug cat villager who first appeared in New Horizons. His birthday is October 1st, and his initial catchphrase is 'crisp'. Would you like to know his preferred clothing styles or his home interior?

---

**👤 You:**
> "What fish can I catch in New Horizons?"

**🤖 AI Agent:**
> I've retrieved the fish catalog for New Horizons. There are 80 different fish in total, ranging from the common Sea Bass to the rare Coelacanth. I can filter these by location (river, pond, sea) or by their selling price. What are you looking for?

---

**👤 You:**
> "List all the DIY recipes available in the game."

**🤖 AI Agent:**
> Fetching DIY recipes... I've found a wide variety of recipes including furniture, tools, and seasonal items. For example, the 'Acoustic Guitar' requires 8 softwood and 3 iron nuggets. Would you like to see recipes for a specific category?


## ❓ FAQ

**Q: Can I search for villagers based on their personality or species?**
Yes! The `get_villagers` tool allows you to filter by name, species (e.g., 'Cat'), and personality (e.g., 'Lazy') to find exactly who you are looking for.

**Q: Does this server provide information on how to craft items in New Horizons?**
Absolutely. Use the `get_nh_recipes` tool to fetch a list of DIY recipes, which includes the materials required for crafting each item.

**Q: Can I check which bugs or fish are available right now?**
Yes. By using `get_nh_bugs` or `get_nh_fish`, your AI agent can retrieve the full encyclopedia data, including the months and times of day each creature appears.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/nookipedia](https://vinkius.com/mcp/nookipedia)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Nookipedia** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `nookipedia` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Nookipedia** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "nookipedia": {
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
