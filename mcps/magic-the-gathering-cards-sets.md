# Magic: The Gathering Cards & Sets MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/magic-the-gathering-cards-sets)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [data-analytics](../categories/data-analytics.md)

Magic: The Gathering as an MCP: search 30+ years of cards across 500+ sets by name/color/CMC/type, browse sets, resolve Gatherer ids, check types — and open virtual booster packs from Alpha to today. Keyless.

## Description
**The first trading card game ever, fully queryable** — Magic: The Gathering's entire print history as a single MCP server.

### What you can do
- **Search the multiverse of cards** — by name, color (U/W/B/R/G), converted mana cost, type or set, across 500+ expansions since Alpha (1993)
- **Canonical lookups** — resolve any Gatherer multiverseid to its exact printing with rules text, power/toughness, artist and flavor
- **Set intelligence** — browse 500+ sets with codes, release dates and blocks; get full details of any one (LEA = Alpha, MH2 = Modern Horizons 2)
- **Open virtual booster packs** — a real gacha: 15 random cards from any set, the dopamine hit of opening Alpha or Zendikar again
- **Reprint hunting** — every printing of a single card side by side

### Why it matters
Magic's card database is cultural heritage: Black Lotus, the Power Nine, Lightning Bolt across 30 years of reprints. This MCP puts the catalog in front of an AI for deck discussion, price-print comparison, quiz building and nostalgia.

### Who is this for?
Deck builders, collectors, MTG content creators, quiz/website builders, spreadsheet modelers and AI agents that need authoritative MTG card data.


## Available Tools (7)
- **get_card_by_multiverseid**: Every Gatherer card URL maps to a multiverseid.

Get one MTG card by its official multiverseid (the canonical Gatherer id)
- **find_format_staples**: Find the most iconic printings of a card across all sets (reprints and price-light alternatives)
- **search_cards**: Colors use single letters U/W/B/R/G (e.g. "U" for blue; "blue" also works but only matches some printings). Pagination via page/page_size with the total returned in the response. Example combos: name=bolt; colors=U cmc=5; set=LEA.

Search Magic: The Gathering cards by name, color, mana cost, type or set (all 500+ sets)
- **list_sets**: Paginated — sorted alphabetically by code, so use the name filter mentally or browse pages.

List Magic sets: 500+ expansions from Alpha (1993) to today, with codes and release dates
- **get_set_details**: Use codes from list_sets (e.g. "LEA" = Limited Edition Alpha).

Get full details of one Magic set by code (Alpha, Modern Horizons...)
- **open_booster_pack**: Pure nostalgia dopamine: "open an Alpha pack for me". Works best with classic sets (LEA, 2ED, MMQ, ZEN...).

Open a virtual Magic booster pack: 15 random cards from any set (fun gacha simulator)
- **list_card_types**: Includes newer types like Battle and Conspiracy.

List all Magic card types (Creature, Instant, Battle, Planeswalker...)


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Magic: The Gathering Cards & Sets** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Open me an Alpha booster pack!"

**🤖 AI Agent:**
> 🃏 **Alpha (LEA) booster — 15 cards**

Commons: Forest, Lightning Bolt, Giant Growth...
Uncommons: Counterspell
**RARE: Black Lotus** 🎉 — "Adds 3 mana of any one color..."

That's the rarest pull in MTG history. Feeling lucky? Open a Zendikar next (fetch lands!)?

---

**👤 You:**
> "Show me every printing of Lightning Bolt across the years"

**🤖 AI Agent:**
> ⚡ **Lightning Bolt — all printings**

- Unlimited Edition (1993) {R} — "Deals 3 damage to any target"
- Revised (1994) · 4th/5th Edition · Mystery Booster
- Modern Masters, Double Masters 2022 (foil reprints)

Same {R} instant, 30 years of art. Want price-tier comparison or another staple (Counterspell, Swords to Plowshares)?

---

**👤 You:**
> "Find me all blue 5-cost dragons"

**🤖 AI Agent:**
> 🔵 **blue cmc=5 type=Dragon**

Top hits: (results from the search)...

Color letters matter here: U=blue, W=white, B=black, R=red, G=green. Want me to widen to cmc<=6 or find red equivalents?


## ❓ FAQ

**Q: Do I need an API key or registration?**
No. api.magicthegathering.io is fully public with a generous rate limit (1000 requests/hour) — all tools work without authentication.

**Q: How do colors work in searches?**
Use single letters: U (blue), W (white), B (black), R (red), G (green). "colors=U&cmc=5" is the reliable form; spelling "blue" only matches a subset of printings. Set codes are three-to-four letters (LEA = Alpha).


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/magic-the-gathering-cards-sets](https://vinkius.com/ai-agent-connect/magic-the-gathering-cards-sets)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Magic: The Gathering Cards & Sets** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `magic-the-gathering-cards-sets` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Magic: The Gathering Cards & Sets** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "magic-the-gathering-cards-sets": {
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
