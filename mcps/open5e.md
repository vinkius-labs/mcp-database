# Open5e MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/open5e)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [developer-tools](../categories/developer-tools.md)

Access the comprehensive Open5e database for D&D 5th Edition — search monsters, spells, classes, and magic items directly from your AI agent.

## Description
Connect your AI agent to the **Open5e** API, the ultimate open-source resource for tabletop RPG data. This server allows you to query a vast library of 5th Edition content using natural language.

### What you can do

- **Global Search** — Use `search_open5e` to find any term across the entire dataset of rules, monsters, and items.
- **Bestiary Access** — List and filter creatures by type, size, or challenge rating using `list_creatures`.
- **Spellbook Management** — Query magic spells by level, school, or class with `list_spells`.
- **Character Building** — Retrieve details on classes, species (races), backgrounds, and feats to assist in character creation.
- **Equipment & Loot** — Browse magic items, weapons, and armor using `list_magic_items` and `list_equipment`.
- **Rules Reference** — Quickly look up status conditions and game sections to keep your session flowing.

### How it works

1. Subscribe to this server
2. Enter your Open5e API Key (if required by your instance) or a placeholder
3. Start querying RPG data from Claude, Cursor, or any MCP-compatible client

No more flipping through rulebooks mid-game. Your AI acts as a digital Dungeon Master's assistant, providing instant stats and descriptions.


## Available Tools (12)
- **list_backgrounds**: List character backgrounds
- **list_classes**: List character classes and archetypes
- **list_conditions**: List status effects and conditions
- **list_creatures**: Can filter by type, size, challenge rating (cr), etc.

List or search monsters and NPCs
- **list_documents**: List source documents and OGL metadata
- **list_equipment**: Can filter by category.

List weapons, armor, and gear
- **list_feats**: List character feats
- **list_magic_items**: Can filter by rarity, category.

List magic items and artifacts
- **search_open5e**: Global search across all Open5e resources
- **list_sections**: List rules and supplemental text sections
- **list_species**: List character species (races)
- **list_spells**: Can filter by level, school, class, etc.

List or search magic spells


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Open5e** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Search Open5e for 'Aboleth' and show me its stats."

**🤖 AI Agent:**
> I found the Aboleth (Large aberration). It has an AC of 17, 135 HP, and a Challenge Rating of 10. Its notable abilities include Enslave and Multiattack with its tentacles. Would you like the full action descriptions?

---

**👤 You:**
> "List all 3rd-level Evocation spells for Wizards."

**🤖 AI Agent:**
> I've retrieved 3rd-level Evocation spells for Wizards. Results include: Fireball, Lightning Bolt, Sending, and Melf's Minute Meteors. Which one should I provide details for?

---

**👤 You:**
> "Find legendary magic items in the 'Wondrous Item' category."

**🤖 AI Agent:**
> Searching for Legendary Wondrous Items... I found several, including the 'Apparatus of Kwalish', 'Cubic Gate', and 'Sovereign Glue'. Would you like to see the properties of the Apparatus of Kwalish?


## ❓ FAQ

**Q: How can I find a monster with a specific Challenge Rating?**
Use the `list_creatures` tool and provide the `cr` parameter (e.g., '1', '1/4', or '20'). You can also combine this with the `type` parameter to find, for example, all CR 5 Dragons.

**Q: Can I search for spells available only to a specific class?**
Yes! Use the `list_spells` tool and set the `class` parameter to your desired class, such as 'Wizard' or 'Cleric'. You can further filter by `level` to narrow down the results.

**Q: What is the best way to find a specific rule or condition?**
For status effects, use `list_conditions`. For general rules or supplemental text, use `list_sections`. If you aren't sure where it is, use `search_open5e` for a global search across all categories.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/open5e](https://vinkius.com/mcp/open5e)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Open5e** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `open5e` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Open5e** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "open5e": {
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
