# Radarr (Movies) MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/radarr-movies)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [content-management](../categories/content-management.md)

Manage your movie library, search for new titles, and monitor download queues via Radarr.

## Description
Connect your **Radarr** instance to any AI agent to take full control of your movie collection and PVR workflows through natural conversation.

### What you can do

- **Library Management** — List all movies in your collection, fetch detailed metadata, and update movie configurations.
- **Discovery & Search** — Search for new movies using TMDB integration and add them to your library with specific quality profiles.
- **Download Monitoring** — Track your active download queue, view history of grabs/imports, and manage queue items.
- **System Operations** — Check disk space, system status, and execute internal commands like library refreshes.
- **Infrastructure Mapping** — Retrieve root folders and quality profiles to ensure correct organization of your media files.

### How it works

1. Subscribe to this server
2. Enter your Radarr URL and API Key
3. Start managing your media library from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Home Lab Enthusiasts** — manage your media server without opening the web UI
- **Content Collectors** — quickly search and add movies to your watchlist via chat
- **System Administrators** — monitor disk space and download health across your media stack


## Available Tools
- **add_movie**: Requires TMDB ID, quality profile, and root folder path.

Add a new movie to Radarr
- **delete_movie**: Remove a movie from Radarr
- **delete_queue_item**: Remove an item from the download queue
- **execute_command**: g., RescanMovie, MovieSearch, RefreshMovie, RenameMovie).

Execute a specific system command
- **get_commands**: List active or recently completed commands
- **get_disk_space**: Get disk space information
- **get_history**: View the history of grabs and imports
- **get_movie**: Get details for a specific movie
- **get_quality_profiles**: g., HD-1080p, Ultra-HD) configured in Radarr.

Get available quality profiles
- **get_queue**: Get the current download queue
- **get_root_folders**: Get configured root folders
- **get_system_status**: Get Radarr system status
- **list_movies**: List all movies in the Radarr library
- **lookup_movie**: g., "term=Inception" or "term=tmdb:27205").

Search for movies to add to Radarr
- **update_movie**: Provide the full movie object payload.

Update an existing movie in Radarr


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Radarr (Movies)** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all movies currently in my Radarr library."

**🤖 AI Agent:**
> I've retrieved your library. You have 124 movies managed. Recent additions include 'Oppenheimer' and 'Barbie'. Would you like details on a specific title?

---

**👤 You:**
> "Search for the movie 'Inception' and tell me its TMDB ID."

**🤖 AI Agent:**
> Searching TMDB... I found 'Inception' (2010) with TMDB ID: 27205. It's currently not in your library. Would you like me to add it?

---

**👤 You:**
> "Show me the current download queue and estimated completion times."

**🤖 AI Agent:**
> Checking the queue... You have 2 active downloads: 'Dune: Part Two' (65% complete, ~10 mins left) and 'Poor Things' (12% complete, ~45 mins left).


## ❓ FAQ

**Q: Can I search for movies on TMDB before adding them to my library?**
Yes! Use the `lookup_movie` tool with a search term. The agent will return potential matches from TMDB, which you can then add using `add_movie`.

**Q: How do I check if I have enough disk space for new downloads?**
Simply ask the agent to run the `get_disk_space` tool. It will provide a list of all connected drives and their available capacity.

**Q: Is it possible to remove a movie and its files from the disk simultaneously?**
Yes. When using the `delete_movie` tool, you can set the `deleteFiles` parameter to true to ensure the media is wiped from your storage.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/radarr-movies](https://vinkius.com/mcp/radarr-movies)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Radarr (Movies)** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `radarr-movies` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Radarr (Movies)** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "radarr-movies": {
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
