# Song Count Total MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/song-count-total)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [utilities](../categories/utilities.md)

Aggregate and analyze song counts across musical albums.

## Description
This MCP server provides tools to analyze music collections by calculating song counts. Use `find_albums_by_artist` to locate specific discographies, `get_album_details` to retrieve individual track counts, `calculate_collection_total` to sum songs across multiple albums, and `get_album_density` to compare an album's size against the catalog average.


## Available Tools (4)
- **get_album_details**: 
- **calculate_collection_total**: 
- **find_albums_by_artist**: 
- **get_album_density**: 


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Song Count Total** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "How many songs are in the album with ID 'alb-123'?"

**🤖 AI Agent:**
> The album 'Midnight Melodies' contains 12 songs.

---

**👤 You:**
> "What is the total number of songs in albums 'alb-001', 'alb-002', and 'alb-003'?"

**🤖 AI Agent:**
> The total number of songs across those 3 albums is 34.

---

**👤 You:**
> "List all albums by the artist 'Luna Ray'."

**🤖 AI Agent:**
> Luna Ray has released the following albums: 'Starlight Echoes' (alb-456) and 'Lunar Phases' (alb-789).


## ❓ FAQ

**Q: How can I find all albums by a specific artist?**
You can use the `find_albums_by_artist` tool by providing the artist's name.

**Q: Can I sum the songs from multiple albums at once?**
Yes, the `calculate_collection_total` tool allows you to provide a list of album IDs to get a combined song count.

**Q: How do I know if an album is larger than average?**
Use the `get_album_density` tool to compare a specific album's song count against the system average.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/song-count-total](https://vinkius.com/en/ai-agent-connect/song-count-total)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Song Count Total** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `song-count-total` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Song Count Total** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "song-count-total": {
      "url": "https://edge.vinkius.com/[TOKEN]/mcp"
    }
  }
}
```

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius connector registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
