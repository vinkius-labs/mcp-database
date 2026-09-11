# Zelda Universe Encyclopedia MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/zelda-universe-encyclopedia)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [entertainment](../categories/entertainment.md)

The complete Legend of Zelda encyclopedia as an MCP: all 32 games (1986-today), 400+ monsters, bosses, dungeons, items (Master Sword), places and characters — searchable, keyless.

## Description
**Nearly 40 years of Hyrule history** as a single MCP server — every game, enemy, dungeon, item and character of The Legend of Zelda franchise.

### What you can do
- **All 32 games** — from the 1986 Famicom original to Tears of the Kingdom, with story summaries and appearance data
- **The bestiary** — 400+ monsters and enemies: Lynel, Bokoblin, Octorok, ReDead... with which games each appeared in
- **Dungeons & bosses** — the Water Temple, Divine Beasts, Ganon incarnations — fuel for the hardest-dungeon debates
- **Legendary items** — Master Sword, Hylian Shield, Ocarina of Time, Majora's Mask, each with full lore
- **World & cast** — Hyrule, Termina, Koholint; Link, Zelda, Ganondorf, Impa and hundreds more

### Why it matters
Zelda lore is famously scattered: five branching timelines, reincarnating heroes, retconned origins. This encyclopedia consolidates it into a queryable catalog an AI can navigate — for content creators, quiz builders, wiki editors and fans settling timeline arguments.

### Who is this for?
Content creators, streamers, wiki editors, trivia/quiz builders, game designers studying the franchise, and every fan who wants Zelda lore on demand.


## Available Tools (8)
- **browse_zelda_database**: Categories: games (32, 1986-2026), monsters (400+), bosses, places, items, dungeons, characters, staff. The name filter is CASE-SENSITIVE substring ("Lynel" finds Lynel/Golden Lynel; "lynel" finds nothing). Page is the page index starting at 0 (offset = page x limit, limit max 50).

Browse The Legend of Zelda encyclopedia: games, monsters, bosses, places, items, dungeons or characters
- **get_zelda_games**: Perfect for timelines, "which Zelda should I play first?" and lore discussions.

List every Legend of Zelda game ever released with description and chronology
- **get_zelda_items**: Returns name, description and appearance count. The lore backbone for equipment questions.

Browse legendary items and equipment: Master Sword, Hylian Shield, Ocarina of Time
- **get_zelda_entry**: Take ids from browse_zelda_database. Great for deep dives: "tell me everything about the Master Sword".

Get the full encyclopedia entry of one Zelda entity by id (monsters, bosses, items, places...)
- **search_zelda_bestiary**: Returns name, short description and appearance count per page. Use for enemy deep dives and "which games had X enemy?" questions.

Search the Zelda bestiary: 400+ monsters and enemies across all games
- **get_zelda_locations**: g. "Hyrule", "Kakariko", "Lorule"). Returns name, description and appearance count. Ideal for world-building questions and geography lore.

Explore the Zelda world map: regions, towns and landmarks (Hyrule, Termina, Koholint...)
- **get_zelda_characters**: Returns name, description and appearance count. For character studies and lore timelines.

Browse Zelda characters: Link, Zelda, Ganondorf, Impa and the rest of the cast
- **get_zelda_dungeons**: Returns name, description and appearance count. Perfect for "hardest dungeon" debates and gameplay retrospectives.

Browse Zelda dungeons: Water Temple, Forest Temple, Divine Beasts


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Zelda Universe Encyclopedia** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Tell me everything about the Lynel enemies"

**🤖 AI Agent:**
> ⚔️ **Lynel family (Zelda bestiary)**

Found 3 variants: **Lynel**, Blue/White Lynels and **Golden Lynel** (the strongest, exclusive to The Legend of Zelda 1986 oracle events).

Golden Lynel: "recurring Enemies in The Legend of Zelda... only found in the Oracle of Seasons Hero's Cave". They're centaur-like beasts considered the toughest non-boss foes — in Breath of the Wild they guard the best weapons. Want the Bokoblin family too?

---

**👤 You:**
> "Which Zelda game should I play first?"

**🤖 AI Agent:**
> 🎮 **Zelda games (32 in the encyclopedia)**

Best entry points:
- **Breath of the Wild (2017)** — modern open-air, no prior knowledge needed
- **Link's Awakening (1993/2019)** — self-contained story on Koholint Island
- **A Link to the Past (1991)** — the classic blueprint

The 1986 original: "centers its plot around a boy named Link... came out as early as 1986 for the Famicom". Want the full chronological list?

---

**👤 You:**
> "Build me a quiz about Zelda items — hardest questions possible"

**🤖 AI Agent:**
> 🧠 **Hard Zelda items quiz (from the encyclopedia)**

1. Which item's description mentions the Oracle of Seasons Hero's Cave? (Golden Lynel connection)
2. Name an item that appears in exactly 4 games...
3. Which shield is described as "indestructible"? (Hylian Shield)

All answers verified against the items database. Want 10 more with multiple choice?


## ❓ FAQ

**Q: Do I need an API key or registration?**
No. The Zelda encyclopedia API is fully public — browsing, searching and detail lookups all work without authentication.

**Q: Why does my name search return nothing?**
The name filter is CASE-SENSITIVE: "Lynel" works, "lynel" returns nothing. Always capitalise names as they appear in the games ("Master Sword", not "master sword").


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/zelda-universe-encyclopedia](https://vinkius.com/en/ai-agent-connect/zelda-universe-encyclopedia)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Zelda Universe Encyclopedia** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `zelda-universe-encyclopedia` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Zelda Universe Encyclopedia** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "zelda-universe-encyclopedia": {
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
