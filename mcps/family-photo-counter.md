# Family Photo Counter MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/family-photo-counter)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Count photos across nested family photo albums.

## Description
This MCP server provides tools to manage and count digital family memories. It allows AI agents to browse available albums, retrieve specific album details, and calculate the total number of photos within an album hierarchy using `count_album_photos`. You can also use `list_albums` to find specific collections or `find_photos_by_album` to see the direct contents of a single album.


## Available Tools (4)
- **get_album_details**: Provides comprehensive information about a specific album
- **list_albums**: You can provide a search query to filter by name.

Retrieves a flat list of all available albums in the system
- **find_photos_by_album**: This does not include photos in sub-albums.

Lists the specific IDs of all photos contained within a single album
- **count_album_photos**: Calculates the total number of photos within an album, including all photos in nested sub-albums


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Family Photo Counter** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "How many total photos are in the 'Summer Vacation 2023' album and all its sub-folders?"

**🤖 AI Agent:**
> There are a total of 142 photos in the 'Summer Vacation 2023' album and its sub-albums.

---

**👤 You:**
> "List all the albums I have available."

**🤖 AI Agent:**
> You have the following albums: 'Summer Vacation 2023', 'Birthday Party', and 'Family Trip'.

---

**👤 You:**
> "What are the details for the album with ID 'abc-123'?"

**🤖 AI Agent:**
> Album 'abc-123' is named 'Christmas 2022'. It contains 15 photos and has 2 sub-albums.


## ❓ FAQ

**Q: How does the photo count work for nested albums?**
By using the `count_album_photos` tool, the system calculates a recursive total that includes all photos in the target album and all its sub-albums.

**Q: Can I search for a specific album?**
Yes, you can use the `list_albums` tool with a search query to filter and find specific albums by name.

**Q: Does this tool show photos in sub-albums when listing album contents?**
No, the `find_photos_by_album` tool only returns photos directly inside the specified album, not those in nested sub-albums.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/family-photo-counter](https://vinkius.com/en/ai-agent-connect/family-photo-counter)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Family Photo Counter** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `family-photo-counter` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Family Photo Counter** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "family-photo-counter": {
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
