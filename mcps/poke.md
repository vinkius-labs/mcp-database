# Poké MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/poke)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [data-management](../categories/data-management.md)

Access the ultimate Pokémon encyclopedia — query berries, contest effects, and encounter methods directly from your AI agent.

## Description
Connect to the **PokéAPI** through this MCP server to explore the vast world of Pokémon data. This integration allows any AI agent to retrieve detailed information about items, mechanics, and world interactions.

### What you can do

- **Berry Research** — List all berries, check their firmness levels, and explore flavor profiles like spicy, dry, or sweet.
- **Contest Mastery** — Query contest types and effects to understand how different moves and items perform in competition.
- **Encounter Methods** — Discover the various ways Pokémon can be encountered in the wild, from walking in tall grass to fishing.
- **Data Exploration** — Access paginated lists of resources to browse the entire database systematically.

### How it works

1. Subscribe to this server
2. Initialize the connection (no complex keys required for public data)
3. Start querying Pokémon lore and mechanics from Claude, Cursor, or any MCP client

### Who is this for?

- **Game Developers** — quickly reference Pokémon mechanics and item data while coding or designing.
- **Content Creators** — verify facts about berries and contests for guides or wikis without leaving the chat interface.
- **Data Enthusiasts** — explore the structured relationships of the Pokémon world through natural language.


## Available Tools (49)
- **get_berry_firmness**: Get berry firmness details
- **get_berry_flavor**: Get berry flavor details
- **get_berry**: Get berry details
- **get_contest_effect**: Get contest effect details
- **get_contest_type**: Get contest type details
- **get_encounter_condition**: Get encounter condition details
- **get_encounter_condition_value**: Get encounter condition value details
- **get_encounter_method**: Get encounter method details
- **get_evolution_chain**: Get evolution chain details
- **get_evolution_trigger**: Get evolution trigger details
- **get_generation**: Get generation details
- **get_item_attribute**: Get item attribute details
- **get_item_category**: Get item category details
- **get_item_fling_effect**: Get item fling effect details
- **get_item_pocket**: Get item pocket details
- **get_item**: Get item details
- **get_location_area**: Get location area details
- **get_location**: Get location details
- **get_pal_park_area**: Get pal park area details
- **get_pokedex**: Get pokedex details
- **get_region**: Get region details
- **get_super_contest_effect**: Get super contest effect details
- **get_version_group**: Get version group details
- **get_version**: Get version details
- **query_graphql**: Execute a GraphQL query against PokéAPI
- **list_berries**: List berries
- **list_berry_firmnesses**: List berry firmnesses
- **list_berry_flavors**: List berry flavors
- **list_contest_effects**: List contest effects
- **list_contest_types**: List contest types
- **list_encounter_condition_values**: List encounter condition values
- **list_encounter_conditions**: List encounter conditions
- **list_encounter_methods**: List encounter methods
- **list_evolution_chains**: List evolution chains
- **list_evolution_triggers**: List evolution triggers
- **list_generations**: List generations
- **list_item_attributes**: List item attributes
- **list_item_categories**: List item categories
- **list_item_fling_effects**: List item fling effects
- **list_item_pockets**: List item pockets
- **list_items**: List items
- **list_location_areas**: List location areas
- **list_locations**: List locations
- **list_pal_park_areas**: List pal park areas
- **list_pokedexes**: List pokedexes
- **list_regions**: List regions
- **list_super_contest_effects**: List super contest effects
- **list_version_groups**: List version groups
- **list_versions**: List versions


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Poké** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List the first 10 berries available in the database."

**🤖 AI Agent:**
> I've retrieved the first 10 berries: cheri, chesto, pecha, rawst, aspear, leppa, oran, persim, lum, and nanab. Would you like details on any of these?

---

**👤 You:**
> "What are the effects of the contest type 'cool'?"

**🤖 AI Agent:**
> The 'cool' contest type (ID: 1) is associated with specific move appeals. In contests, using 'cool' moves will yield higher points if the audience is looking for that style. Would you like to see the list of contest effects?

---

**👤 You:**
> "Show me the different encounter methods available."

**🤖 AI Agent:**
> I found several encounter methods, including 'walk' (walking in tall grass), 'old-rod' (fishing), 'surf' (moving on water), and 'headbutt' (shaking trees). Which one would you like to explore further?


## ❓ FAQ

**Q: How can I find the specific details of a berry by its name?**
Use the `get_berry` tool and provide the name (e.g., 'cheri'). The agent will return its growth time, max harvest, size, and smoothness.

**Q: Can I list all the different ways a Pokémon can be encountered?**
Yes, use the `list_encounter_methods` tool. It provides a paginated list of all methods like 'walk', 'old-rod', or 'surf' used in the games.

**Q: Is it possible to check the effects of Pokémon Contests?**
Absolutely. You can use `list_contest_effects` to see available effects or `get_contest_effect` with a specific ID to see the detailed appeal and jam metadata.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/poke](https://vinkius.com/mcp/poke)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Poké** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `poke` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Poké** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "poke": {
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
