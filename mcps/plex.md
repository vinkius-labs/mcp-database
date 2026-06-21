# Plex MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/plex)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [content-management](../categories/content-management.md)

Manage your Plex Media Server — browse libraries, search media, check active streams and control playback from any AI agent.

## Description
Connect to your **Plex Media Server** and manage your entire media library through natural conversation.

### What you can do

- **Server Info** — Check server status, version and connected clients
- **Active Sessions** — See who's watching what right now with playback progress
- **Libraries** — Browse all your media libraries (movies, shows, music, photos)
- **Search** — Find any movie, episode, artist or album by name
- **Recently Added** — Discover the newest additions to your library
- **On Deck** — See what's next to continue watching
- **Metadata** — Get full details on any media item including cast, file info and streams
- **Playlists** — Browse and manage your playlists
- **Watch Status** — Mark items as watched or unwatched

### How it works

1. Subscribe to this server
2. Enter your Plex Token and Server URL
3. Start managing your media library from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Home Media Users** — search your library, check what's playing and find new content to watch
- **Server Admins** — monitor active sessions, manage libraries and check server health
- **Family Managers** — see what family members are watching and manage playlists


## Available Tools (15)
- **get_all_episodes**: Useful for getting the complete episode list for a series.

Get all episodes of a TV show
- **get_children**: For TV shows this returns seasons. For artists this returns albums. Requires the parent item's rating key.

Get children of a media item (seasons or albums)
- **get_libraries**: Each library includes its key (ID), type (movie, show, music, photo), title, agent, scanner and updated/created timestamps. Use the library key with other library tools.

Get all libraries (sections) on the Plex server
- **get_library_content**: Filter by type: type=1 for movies, type=2 for TV shows, type=8 for artists, type=13 for photos. Requires the library key from get_libraries.

Get all content from a specific library
- **get_metadata**: Returns title, summary, year, runtime, rating, genres, director, cast, media streams, file path and more.

Get detailed metadata for a specific item
- **get_on_deck**: Returns the next unwatched episode for each in-progress show.

Get "On Deck" items (continue watching)
- **get_playlist_items**: Returns the items with their titles, types, durations and metadata. Requires the playlist ID.

Get items in a specific playlist
- **get_playlists**: Each playlist includes its ID, title, type (video, audio, photo), item count and duration.

Get all playlists on the Plex server
- **get_recently_added**: Returns movies, episodes and albums with their titles, addition dates and metadata.

Get recently added media to the library
- **get_server_info**: Useful for verifying server connectivity and checking server health.

Get Plex Media Server information
- **get_sessions**: Each session includes the user, the media being watched (movie/episode), playback progress, player device, bandwidth and transcoding info.

Get currently active streaming sessions
- **mark_unwatched**: This resets the item's watch status. Requires the item's rating key.

Mark a media item as unwatched
- **mark_watched**: This affects the item's watch status and removes it from "On Deck". Requires the item's rating key.

Mark a media item as watched
- **refresh_library**: Useful after adding or removing files from your media folders. Requires the library key.

Trigger a library scan/refresh
- **search_library**: Returns matching movies, shows, episodes, artists and albums with their titles, types and metadata.

Search the Plex media library


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Plex** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Show me what's currently playing on my Plex server."

**🤖 AI Agent:**
> Active sessions: 1. User 'John' watching 'The Last of Us S01E03' at 34:15/58:22 (Roku, Direct Play). 2. User 'Sarah' watching 'Oppenheimer' at 1:45:30/3:00:15 (iPhone, Transcoding 1080p).

---

**👤 You:**
> "Show me my movie libraries."

**🤖 AI Agent:**
> Found 3 libraries: 1. 'Movies' (key: 1, type: movie, 1,245 items) — 2. '4K Movies' (key: 5, type: movie, 342 items) — 3. 'Kids Movies' (key: 8, type: movie, 189 items).

---

**👤 You:**
> "What's on deck for me to watch?"

**🤖 AI Agent:**
> On Deck: 1. 'The Mandalorian S03E05' — 2. 'Stranger Things S04E07' — 3. 'Ted Lasso S02E03' — 4. 'The Office S07E19' — 5. 'Severance S01E04'. All are next unwatched episodes of shows you're currently watching.


## ❓ FAQ

**Q: How do I get my Plex Token?**
Log in to your Plex account at [**plex.tv**](https://plex.tv), go to **Settings > Server > General** and look for 'X-Plex-Token'. Alternatively, check your browser's network tab when loading the Plex web app.

**Q: What is my Server URL?**
For local access: `http://YOUR_SERVER_IP:32400` (e.g. `http://192.168.1.100:32400`). For remote access: `https://YOUR_PLEX_SUBDOMAIN.plex.direct:32400`. The IP is your Plex server's local network address.

**Q: Can I see what's currently playing?**
Yes! Use get_sessions to see all active playback sessions. Each session shows the user, media title, playback position, player device and whether it's direct playing or transcoding.

**Q: Can I search for specific media?**
Yes! Use search_library with any title. Results include movies, TV shows, episodes, artists and albums matching your query. Optionally filter by library key to search in a specific library only.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/plex](https://vinkius.com/mcp/plex)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Plex** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `plex` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Plex** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "plex": {
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
