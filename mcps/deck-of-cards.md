# Deck of Cards MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/deck-of-cards)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Simulate a full deck of cards via the Deck of Cards API — shuffle, draw, manage piles, and create custom decks for games or simulations.

## Description
Connect to the **Deck of Cards API** to integrate standard playing card mechanics into your AI agent. Perfect for building games, probability simulations, or interactive entertainment through natural conversation.

### What you can do

- **Deck Management** — Create new decks, shuffle existing ones, or generate partial decks with specific cards (e.g., only Aces and Kings).
- **Draw Mechanics** — Draw cards from the top, bottom, or random positions in a deck or specific named piles.
- **Pile Organization** — Create named piles (like 'Player 1 Hand' or 'Discard Pile') and move cards between them seamlessly.
- **Custom Configurations** — Include jokers or use multiple decks (up to 6 or more) for complex casino-style simulations.
- **State Tracking** — List cards in specific piles and track the remaining count in the main deck.

### How it works

1. Subscribe to this server
2. Initialize your session by providing a Deck ID or using the 'new' keyword
3. Start playing or simulating card games directly from Claude, Cursor, or any MCP-compatible client

No more manual randomization or complex state management for card games. Your AI acts as the dealer and game engine.

### Who is this for?

- **Game Developers** — prototype card game logic and mechanics quickly without writing a backend
- **Data Scientists** — run probability simulations and Monte Carlo experiments using a standardized card API
- **Hobbyists & Educators** — play simple card games or teach probability and statistics with interactive examples


## Available Tools (13)
- **add_to_pile**: Add cards to a pile
- **create_new_deck**: Create a brand new deck in standard order
- **create_partial_deck**: Create a partial deck with specific cards
- **draw_cards**: Draw cards from a deck
- **draw_from_pile_bottom**: Draw cards from the bottom of a pile
- **draw_from_pile_random**: Draw random cards from a pile
- **draw_from_pile**: Draw cards from a pile
- **list_pile**: List cards in a pile
- **reshuffle_deck**: Reshuffle an existing deck
- **return_pile_to_deck**: Return cards from a pile to the main deck
- **return_to_deck**: Return cards to the main deck
- **shuffle_new_deck**: Can optionally use multiple decks.

Create a new shuffled deck
- **shuffle_pile**: Shuffle a specific pile


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Deck of Cards** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Create a new shuffled deck using 6 standard decks for a blackjack simulation."

**🤖 AI Agent:**
> I've initialized a new multi-deck set. Deck ID: `3p40paa87x90`. It contains 312 cards and is fully shuffled. Ready to deal!

---

**👤 You:**
> "Draw 5 cards from deck 3p40paa87x90 and add them to a pile named 'player_hand'."

**🤖 AI Agent:**
> I've drawn 5 cards (8H, AD, 2C, KS, 4D) and moved them to the 'player_hand' pile. There are 307 cards remaining in the main deck.

---

**👤 You:**
> "List all the cards currently in the 'discard' pile for deck 3p40paa87x90."

**🤖 AI Agent:**
> The 'discard' pile currently contains 3 cards: Queen of Hearts (QH), 10 of Spades (0S), and 5 of Diamonds (5D).


## ❓ FAQ

**Q: Can I create a deck that includes Jokers for games like Rummy?**
Yes! Use the `create_new_deck` tool and set the `jokers_enabled` parameter to true. This will add two Jokers to your standard 52-card deck.

**Q: Is it possible to draw cards from the bottom of a pile instead of the top?**
Absolutely. Use the `draw_from_pile_bottom` tool by specifying the `deck_id` and `pile_name`. You can also use `draw_from_pile_random` if you need a random card from the middle of a pile.

**Q: How do I simulate a casino game that uses 6 shuffled decks?**
Use the `shuffle_new_deck` tool and set the `deck_count` parameter to 6. This will return a single `deck_id` containing 312 cards (52 * 6) in a randomized order.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/deck-of-cards](https://vinkius.com/mcp/deck-of-cards)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Deck of Cards** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `deck-of-cards` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Deck of Cards** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "deck-of-cards": {
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
