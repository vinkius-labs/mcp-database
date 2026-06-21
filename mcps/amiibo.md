# Amiibo MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/amiibo)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [databases](../categories/databases.md)

Search and filter the complete Amiibo database — access figures, cards, and series data directly from any AI agent.

## Description
Connect to the **AmiiboAPI** and explore the vast world of Nintendo's Amiibo collectibles through natural conversation. This server provides comprehensive access to data on figures, cards, and plushies.

### What you can do

- **Search & Filter** — Find Amiibos by name, character, game series, or collection series using the `list_amiibos` tool.
- **Detailed Inspection** — Get precise metadata for a specific Amiibo using its unique 16-digit ID with `get_amiibo`.
- **Metadata Discovery** — List all available types, game series, and characters to understand the scope of the collection.
- **Database Status** — Check when the Amiibo database was last synchronized with the latest releases using `get_last_updated`.

### How it works

1. Subscribe to this server
2. No API key is required for the public AmiiboAPI
3. Start querying Nintendo collectible data from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Collectors** — quickly check which Amiibos exist in a specific series or for a favorite character
- **Developers** — integrate Amiibo metadata into gaming apps or inventory trackers
- **Nintendo Fans** — explore the history and variety of Amiibo releases across different platforms


## Available Tools
- **get_amiibo**: Get data for a specific Amiibo by ID
- **get_last_updated**: Get database last updated timestamp
- **list_amiibo_series**: Get all Amiibo Series
- **list_amiibos**: Can be filtered by name, character, game series, amiibo series, type, or ID segments.

List all Amiibo with optional filters
- **list_characters**: Get all Characters
- **list_game_series**: Get all Game Series
- **list_types**: g., Figure, Card).

Get all Amiibo types


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Amiibo** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all Mario Amiibos from the Super Smash Bros. series."

**🤖 AI Agent:**
> I've found several Mario Amiibos in the Super Smash Bros. series, including the standard Mario figure (ID: 0000000000000002) and Gold/Silver variants. Would you like the details for a specific one?

---

**👤 You:**
> "Show me all available Amiibo types."

**🤖 AI Agent:**
> The available Amiibo types are: Figure, Card, and Yarn. Most collectibles are Figures, but there are extensive Card collections for series like Animal Crossing.

---

**👤 You:**
> "When was the Amiibo database last updated?"

**🤖 AI Agent:**
> The Amiibo database was last updated on 2024-03-15. This ensures you have access to the most recent release information and metadata.


## ❓ FAQ

**Q: How can I filter Amiibos by a specific game series like Super Smash Bros.?**
You can use the `list_amiibos` tool and provide the series name in the `amiiboseries` or `gameseries` parameter. The agent will return all matching figures and cards from that collection.

**Q: Can I see all the different characters that have Amiibo versions?**
Yes! Use the `list_characters` tool to retrieve a complete list of every character represented in the Amiibo database.

**Q: How do I get the specific details of a single Amiibo if I have its ID?**
Simply provide the 16-digit ID to the `get_amiibo` tool. It will return detailed information including the character, series, release dates, and image URL.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/amiibo](https://vinkius.com/mcp/amiibo)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Amiibo** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `amiibo` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Amiibo** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "amiibo": {
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
