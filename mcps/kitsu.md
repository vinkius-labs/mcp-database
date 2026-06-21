# Kitsu MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/kitsu)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Search and manage your anime and manga collections via Kitsu — browse titles, check user profiles, and update your library directly from any AI agent.

## Description
Connect your **Kitsu** account to any AI agent to explore the world of anime and manga and manage your personal tracking lists through natural conversation.

### What you can do

- **Anime & Manga Discovery** — Search through thousands of titles using filters like categories, seasons, or years via `list_anime` and `list_manga`.
- **Detailed Metadata** — Fetch comprehensive information about specific series, including descriptions, genres, and production details using `get_anime` and `get_manga`.
- **Library Management** — List, create, and update your personal library entries to keep track of your progress with `list_library_entries`, `create_library_entry`, and `update_library_entry`.
- **User Profiles** — Retrieve profile information for specific users or your own authenticated account using `get_user` and `get_current_user`.

### How it works

1. Subscribe to this server
2. Enter your Kitsu Access Token
3. Start exploring anime and manga from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Anime Fans** — quickly find new series to watch and update your 'currently watching' list without leaving your chat.
- **Content Creators** — retrieve accurate metadata and descriptions for research or scriptwriting.
- **Developers** — integrate anime data into your workflows or test library management features via AI.


## Available Tools
- **create_library_entry**: Create a new library entry
- **get_anime**: Get details for a specific anime
- **get_current_user**: Get the currently authenticated user
- **get_manga**: Get details for a specific manga
- **get_user**: Get details for a specific user
- **list_anime**: Use filters to search by text, categories, season, or year.

List and search anime series
- **list_library_entries**: List a user's library entries (anime/manga list)
- **list_manga**: Use filters to search.

List and search manga series
- **update_library_entry**: Update an existing library entry


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Kitsu** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Search for action anime from the Summer 2023 season."

**🤖 AI Agent:**
> I found several action anime from Summer 2023, including 'Jujutsu Kaisen Season 2' and 'Zom 100: Bucket List of the Dead'. Would you like more details on any of these?

---

**👤 You:**
> "Get the details for anime with ID 12."

**🤖 AI Agent:**
> Fetching details for ID 12... That is 'One Piece'. It's an ongoing series about Monkey D. Luffy's quest to become the Pirate King. It has over 1000 episodes and is categorized under Action, Adventure, and Fantasy.

---

**👤 You:**
> "Show me my library entries."

**🤖 AI Agent:**
> I've retrieved your library. You have 15 entries, including 'Chainsaw Man' (Currently Watching) and 'Berserk' (Completed). Would you like to update the progress for any of these?


## ❓ FAQ

**Q: Can I search for anime by specific seasons or years?**
Yes! The `list_anime` tool allows you to filter by `filter_season` (winter, spring, summer, fall) and `filter_year` (e.g., 2023 or a range like 2010..2020).

**Q: How do I see what's currently in my library?**
You can use the `list_library_entries` tool with your `user_id`. If you don't know your ID, run `get_current_user` first to retrieve your profile details.

**Q: Can I update my progress on a manga I'm reading?**
Absolutely. Use the `update_library_entry` tool to modify the status or progress of any existing entry in your library.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/kitsu](https://vinkius.com/mcp/kitsu)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Kitsu** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `kitsu` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Kitsu** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "kitsu": {
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
