# PokéAPI MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/pokeapi)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/pokeapi-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/pokeapi-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [data-management](../categories/data-management.md)

Access Pokémon data, stats, abilities, types, and evolution chains via AI.

## Description
Connect **PokéAPI**, the definitive Pokémon database, to any AI agent and explore comprehensive data on all 1000+ Pokémon species, moves, abilities, types, items, and evolution chains through natural language.

### What you can do

- **Pokémon Lookup** — Get detailed stats, types, abilities, height, weight, and sprite images for any Pokémon
- **Species Data** — Access capture rates, egg groups, growth rates, habitats, and flavor text from every game version
- **Type Effectiveness** — Check damage relations for all 18 types to plan battle strategies
- **Move Database** — Search moves by power, accuracy, PP, and effects with full metadata
- **Evolution Chains** — View complete family trees with all evolution conditions and triggers
- **Item Catalog** — Browse held items, Poké Balls, and berries with effects and costs
- **Regional Data** — Explore generations, regions, and Pokédex variants

### How it works

1. Subscribe to this server
2. No API key required — PokéAPI is free and open
3. Start exploring Pokémon data from Claude, Cursor, or any MCP-compatible client


## Available Tools
- **get_ability**: Get detailed ability information
- **get_berry**: Get detailed berry information
- **get_evolution_chain**: ).

Get evolution chain details
- **get_generation**: Get generation details
- **get_item**: Get detailed item information
- **get_move**: Get detailed move information
- **get_pokedex**: Get detailed Pokédex information
- **get_pokemon**: ), types, abilities, height, weight, and sprite images. Accepts either the Pokémon ID or name.

Get detailed Pokémon information
- **get_region**: Get region details
- **get_pokemon_species**: Get Pokémon species information
- **get_type**: Get type effectiveness and Pokémon
- **list_abilities**: Each ability grants a passive effect to the Pokémon that has it.

List all Pokémon abilities
- **list_berries**: Berries are held items with various effects when consumed.

List all berries
- **list_generations**: List all Pokémon generations
- **list_items**: List all held items
- **list_moves**: List all Pokémon moves
- **list_pokedexes**: ) with their associated regions and Pokémon entries.

List all Pokédexes
- **list_pokemon**: Use limit and offset to browse through the full catalog of 1000+ Pokémon.

List all Pokémon names with pagination
- **list_regions**: ) with their associated locations, Pokédexes, and version groups.

List all Pokémon regions
- **list_types**: ). There are 18 types in total.

List all Pokémon types


## 💬 Prompt Examples

Here are some examples of how you can interact with the **PokéAPI** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Show me everything about Pikachu."

**🤖 AI Agent:**
> Pikachu (#025) is an Electric-type Pokémon. Height: 0.4m, Weight: 6.0kg. Base stats: HP 35, Attack 55, Defense 40, Sp. Atk 50, Sp. Def 50, Speed 90. Abilities: Static (Lightning Rod is hidden). It evolves from Pichu and into Raichu.

---

**👤 You:**
> "What types are strong against Fire?"

**🤖 AI Agent:**
> Fire-type Pokémon are weak to Water, Ground, and Rock types (take 2x damage). They resist Fire, Grass, Ice, Bug, Steel, and Fairy (take 0.5x damage). Fire moves are super effective against Grass, Ice, Bug, and Steel.

---

**👤 You:**
> "What's the evolution chain for Eevee?"

**🤖 AI Agent:**
> Eevee has 8 possible evolutions! Vaporeon (Water Stone), Jolteon (Thunder Stone), Flareon (Fire Stone), Espeon (high friendship during day), Umbreon (high friendship at night), Leafeon (near Moss Rock), Glaceon (near Ice Rock), and Sylveon (high affection with Fairy-type move).


## Installation & Usage

To install and use the **PokéAPI** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/pokeapi](https://vinkius.com/mcp/pokeapi)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
