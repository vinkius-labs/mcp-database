# Hyrule Compendium MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/hyrule-compendium)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [knowledge-management](../categories/knowledge-management.md)

Access the comprehensive Breath of the Wild and Tears of the Kingdom compendium — search creatures, monsters, materials, and equipment directly from your AI agent.

## Description
Connect your AI agent to the **Hyrule Compendium** and explore the vast world of Zelda: Breath of the Wild and Tears of the Kingdom through natural conversation.

### What you can do

- **Full Compendium Access** — Retrieve every entry in the database using `get_all_entries`, categorized for easy browsing of the Hylian ecosystem.
- **Specific Entry Lookup** — Use `get_entry` to get detailed metadata, common locations, and dropped items for any creature, monster, or equipment by its name or ID.
- **Category Filtering** — Narrow down your search with `get_category` to focus on specific groups like monsters, materials, creatures, equipment, or treasure.
- **Ecology & Stats** — Inspect descriptions and properties of items to understand their role in the game world.

### How it works

1. Subscribe to this server
2. No complex API keys required for this public data source
3. Start asking about Hylian wildlife, weapons, or materials from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Zelda Players** — quickly check locations and drops for materials or monster parts while playing without leaving your screen.
- **Lore Enthusiasts** — explore the detailed descriptions and ecology of Hyrule's inhabitants through an interactive encyclopedia.
- **Developers** — test MCP tool-calling capabilities with a clean, structured, and fun dataset.


## Available Tools (3)
- **get_all_entries**: Get all entries in the Hyrule Compendium
- **get_category**: Get all entries within a specific category
- **get_entry**: g., 1 or silver_lynel).

Get a single entry by ID or name


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Hyrule Compendium** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Show me the details for entry number 100 in the compendium."

**🤖 AI Agent:**
> I've retrieved entry #100. It is the 'Blue Sparrow', a small bird found in the Lanayru Great Spring and Hyrule Ridge areas. It drops Chickloo Tree Nuts when startled.

---

**👤 You:**
> "List all monsters found in Hyrule."

**🤖 AI Agent:**
> Fetching the monster category... I've found various entries including Bokoblins, Moblins, and Lynels. Would you like details on a specific monster or a list of the most dangerous ones?

---

**👤 You:**
> "Get all materials used for cooking or upgrades."

**🤖 AI Agent:**
> Accessing the materials category... I've found entries like 'Silent Princess', 'Big Hearty Truffle', and 'Voltfin Trout'. Which material would you like to know more about?


## ❓ FAQ

**Q: How can I find the stats for a specific creature like a 'Golden Horse'?**
Use the `get_entry` tool and provide 'golden_horse' as the id_or_name. The agent will return its common locations, drops, and description in seconds.

**Q: Can I list only the weapons and armor available in the game?**
Yes. Use the `get_category` tool with the category_name set to 'equipment' to see all gear recorded in the compendium.

**Q: Is it possible to browse the entire compendium at once?**
Absolutely. The `get_all_entries` tool fetches the complete database, organized by category, allowing your AI to act as a full Hylian encyclopedia.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/hyrule-compendium](https://vinkius.com/mcp/hyrule-compendium)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Hyrule Compendium** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `hyrule-compendium` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Hyrule Compendium** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "hyrule-compendium": {
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
