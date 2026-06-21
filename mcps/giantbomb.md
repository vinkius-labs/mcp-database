# GiantBomb MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/giantbomb)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [databases](../categories/databases.md)

Access the world's largest video game database — query games, platforms, characters, and companies directly from your AI agent.

## Description
Connect the **Giant Bomb** encyclopedia to your AI agent to unlock deep insights into the history and data of the video game industry.

### What you can do

- **Game Discovery** — Search for any title or list games with specific filters like release dates or genres.
- **Deep Metadata** — Fetch detailed information for specific games, including descriptions, release info, and ratings using unique GUIDs.
- **Platform & Hardware** — Explore technical specs and history for consoles, handhelds, and legacy gaming platforms.
- **Industry Entities** — Query developers and publishers to understand the companies behind your favorite franchises.
- **Character Database** — Retrieve bios and appearances for thousands of iconic video game characters.
- **Universal Search** — Use a single query to find matches across games, characters, companies, and platforms simultaneously.

### How it works

1. Subscribe to this server
2. Enter your Giant Bomb API Key
3. Start exploring gaming history from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Gamers & Enthusiasts** — quickly settle debates about release dates or character backstories.
- **Game Developers** — research industry trends, platform history, and competitive landscapes.
- **Content Creators** — pull accurate metadata and descriptions for reviews or video scripts without leaving your workflow.


## Available Tools
- **get_character**: Retrieve details for a specific character
- **get_company**: Retrieve details for a specific company
- **get_game**: Retrieve details for a specific game
- **get_platform**: Retrieve details for a specific platform
- **list_characters**: Retrieve a list of characters
- **list_companies**: Retrieve a list of companies
- **list_games**: Use filters to narrow down results.

Retrieve a list of games
- **list_platforms**: ).

Retrieve a list of gaming platforms
- **search**: Search across multiple resources


## 💬 Prompt Examples

Here are some examples of how you can interact with the **GiantBomb** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Search for 'The Legend of Zelda' in the Giant Bomb database."

**🤖 AI Agent:**
> I found several matches for 'The Legend of Zelda'. The main game series entry is GUID 3030-4725. I also found characters like Link (GUID 3005-32) and various platforms. Which one would you like to explore?

---

**👤 You:**
> "Get the full details for the game with GUID 3030-4725."

**🤖 AI Agent:**
> Fetching details for 'The Legend of Zelda'... This classic action-adventure game was developed and published by Nintendo. It features a vast overworld, challenging dungeons, and introduced the iconic character Link. It was originally released for the Famicom Disk System in 1986.

---

**👤 You:**
> "List all gaming platforms released by SEGA."

**🤖 AI Agent:**
> Querying platforms... I've found several SEGA platforms including the Genesis (GUID 3045-6), Dreamcast (GUID 3045-37), Game Gear (GUID 3045-5), and Saturn (GUID 3045-42). Would you like the technical specifications for any of these?


## ❓ FAQ

**Q: How do I find the unique GUID for a specific game or character?**
You can use the `search` tool with your query. The results will include the `guid` (e.g., 3030-4725) for each item, which you can then use with `get_game` or `get_character` for full details.

**Q: Can I filter games by a specific platform or developer?**
Yes! Use the `list_games` tool and provide a string to the `filter` parameter (e.g., `platforms:146` or `name:Mario`). You can also use `field_list` to limit the data returned.

**Q: What kind of resources can I search for simultaneously?**
The `search` tool allows you to specify multiple types in the `resources` parameter, such as `game,character,company,platform`. This returns the most relevant matches across all those categories in one go.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/giantbomb](https://vinkius.com/mcp/giantbomb)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **GiantBomb** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `giantbomb` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **GiantBomb** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "giantbomb": {
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
