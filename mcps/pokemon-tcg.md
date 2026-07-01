# Pokemon TCG MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/pokemon-tcg)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [knowledge-management](../categories/knowledge-management.md)

Search and browse the entire Pokemon Trading Card Game database — find specific cards, explore sets, and filter by types or rarities.

## Description
Connect to the comprehensive **Pokemon TCG API** and turn your AI agent into a master collector or deck builder. Access thousands of cards across all historical and modern sets through natural conversation.

### What you can do

- **Card Discovery** — Search for specific cards using names, types, or complex queries (e.g., "name:charizard") using the `list_cards` tool
- **Set Exploration** — List all released sets and fetch detailed metadata for specific expansions with `list_sets` and `get_set`
- **Metadata Lookup** — Retrieve exhaustive lists of energy types, card subtypes, supertypes, and rarities to refine your searches
- **Deep Card Inspection** — Get high-resolution image links, market prices, and attack details for any individual card using `get_card`

### How it works

1. Subscribe to this server
2. (Optional) Enter your Pokemon TCG API Key for higher rate limits
3. Start querying card data from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Collectors** — quickly find card variations, check rarities, and browse historical sets
- **Players & Deck Builders** — search for cards with specific attacks or types to optimize your competitive play
- **Developers** — integrate real-time TCG data into your workflow or applications


## Available Tools (8)
- **list_sets**: Use the "q" parameter to search (e.g., "series:sword").

List Pokemon card sets with optional search and pagination
- **list_subtypes**: g., EX, Mega, Rapid Strike).

List all card subtypes
- **list_supertypes**: g., Pokémon, Trainer, Energy).

List all card supertypes
- **list_types**: g., Fire, Water, Grass).

List all Pokemon energy types
- **get_card**: Get details for a specific Pokemon card by ID
- **get_set**: Get details for a specific Pokemon card set by ID
- **list_cards**: Use the "q" parameter to search (e.g., "name:charizard").

List Pokemon cards with optional search and pagination
- **list_rarities**: g., Rare Holo, Uncommon).

List all card rarities


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Pokemon TCG** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Search for all Charizard cards from the 'Base' set."

**🤖 AI Agent:**
> I've found the results for Charizard in the Base set. The most famous one is ID 'base1-4', a Rare Holo Stage 2 Pokemon with 120 HP and the Fire Spin attack.

---

**👤 You:**
> "List all available Pokemon energy types."

**🤖 AI Agent:**
> The current energy types in the TCG include: Colorless, Darkness, Dragon, Fairy, Fighting, Fire, Grass, Lightning, Metal, Psychic, and Water.

---

**👤 You:**
> "Get the full details for the card with ID 'swsh1-1'."

**🤖 AI Agent:**
> Card 'swsh1-1' is Celebi V from the Sword & Shield expansion. It's a Basic Grass Pokemon with 180 HP, featuring the attacks 'Line Spray' and 'Beam Blast'.


## ❓ FAQ

**Q: Can I search for cards from a specific set like 'Base Set'?**
Yes! Use the `list_cards` tool with a query parameter like `q="set.name:base"`. You can combine this with other filters like name or type.

**Q: How do I see all the available card rarities in the game?**
Simply run the `list_rarities` tool. It will return a complete list of all rarity strings used in the database, such as 'Rare Holo', 'Uncommon', or 'Promo'.

**Q: Is an API key required to use this server?**
An API key is optional. The server will work without one using the public tier, but providing a key from pokemontcg.io allows for much higher rate limits and faster responses.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/pokemon-tcg](https://vinkius.com/mcp/pokemon-tcg)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Pokemon TCG** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `pokemon-tcg` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Pokemon TCG** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "pokemon-tcg": {
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
