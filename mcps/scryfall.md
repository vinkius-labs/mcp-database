# Scryfall MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/scryfall)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [databases](../categories/databases.md)

Access the ultimate Magic: The Gathering database — search cards, fetch rulings, and explore sets directly from your AI agent.

## Description
Integrate **Scryfall**, the most powerful Magic: The Gathering API, into your AI workflow. Whether you are a deck builder, a collector, or a developer, this server provides instant access to the entire history of MTG through natural conversation.

### What you can do

- **Advanced Card Search** — Use the `search_cards` tool with full Scryfall syntax support (e.g., search by type, color, mana value, or oracle text)
- **Exact & Fuzzy Matching** — Quickly find specific cards like 'Black Lotus' or 'Jace' using `get_card_named` without needing exact spelling
- **Set & Expansion Data** — Browse the history of Magic by listing all sets or fetching specific expansion details with `list_sets` and `get_set_by_code`
- **Rules & Rulings** — Retrieve official judge rulings and oracle text to resolve complex card interactions instantly
- **Collection Management** — Fetch multiple cards at once using various identifiers (ID, name, or collector number) for deck analysis

### How it works

1. Subscribe to this server
2. Enter an optional User-Agent string to identify your requests
3. Start querying the multiverse from Claude, Cursor, or any MCP-compatible client

No more manual searching through browser tabs to check a card's legality or current price. Your AI acts as a master librarian for all things Magic.

### Who is this for?

- **Players & Deck Builders** — quickly check card synergies and rulings while discussing strategies
- **Collectors** — retrieve precise set information and collector numbers for inventory management
- **Developers** — integrate MTG data into coding projects or custom tools directly from the IDE


## Available Tools (19)
- **autocomplete_cards**: Get card name suggestions
- **get_bulk_data_by_type**: Get a specific bulk data file by type
- **get_card_by_arena_id**: Get a card by Arena ID
- **get_card_by_id**: Get a card by Scryfall ID
- **get_card_by_mtgo_id**: Get a card by MTGO ID
- **get_card_by_multiverse_id**: Get a card by Multiverse ID
- **get_card_by_set_number**: Get a card by set code and collector number
- **get_catalog**: Get a catalog of Magic data points
- **get_cards_collection**: Get a collection of cards by identifiers
- **list_bulk_data**: List all bulk data files
- **list_sets**: List all Magic sets
- **list_symbology**: List all card symbols
- **get_card_named**: Get a card by exact or fuzzy name
- **parse_mana**: Parse a mana string
- **get_rulings_by_id**: Get rulings for a card by Scryfall ID
- **get_rulings_by_set_number**: Get rulings for a card by set code and collector number
- **search_cards**: Search for Magic cards
- **get_set_by_code**: Get a set by its code
- **get_set_by_id**: Get a set by its Scryfall ID


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Scryfall** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Search for all legendary dragons that are red and cost 5 mana or less."

**🤖 AI Agent:**
> I found several cards matching your criteria, including 'Lathliss, Dragon Queen' and 'Rith, Liberated Primeval'. Would you like to see the full details for any of these?

---

**👤 You:**
> "Get the card details for 'Sol Ring'."

**🤖 AI Agent:**
> Sol Ring is a legendary artifact that costs 1 generic mana. Its ability is '{T}: Add {C}{C}'. It has been printed in many sets, including Alpha and Commander editions.

---

**👤 You:**
> "List all Magic: The Gathering sets released in 2023."

**🤖 AI Agent:**
> In 2023, Scryfall records several major releases including 'Phyrexia: All Will Be One' (ONE), 'March of the Machine' (MOM), and 'Wilds of Eldraine' (WOE).


## ❓ FAQ

**Q: Does the search tool support complex Scryfall syntax like 't:creature c:g cmc=3'?**
Yes! The `search_cards` tool accepts any valid Scryfall search query, allowing you to filter by type, color, mana cost, power/toughness, and more.

**Q: Can I find a card even if I don't remember the exact spelling of its name?**
Absolutely. Use the `get_card_named` tool with the `fuzzy` parameter. Scryfall's engine will suggest the closest match to your input.

**Q: How do I get the official rulings for a specific card interaction?**
You can use the `get_rulings_by_id` tool. By providing the card's Scryfall ID, the agent will return all official judge rulings and timing notes associated with that card.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/scryfall](https://vinkius.com/mcp/scryfall)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Scryfall** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `scryfall` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Scryfall** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "scryfall": {
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
