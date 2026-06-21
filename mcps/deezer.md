# Deezer MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/deezer)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [audio-music](../categories/audio-music.md)

Search music, browse artists, albums and playlists, and explore charts via AI.

## Description
Connect **Deezer** music catalog to any AI agent and search millions of tracks, discover artists, explore albums and playlists, and check global charts through natural language.

### What you can do

- **Track Search** — Search millions of tracks by title, lyrics, or keywords with preview links
- **Artist Discovery** — Find artists, view fan counts, and get their top tracks and radio stations
- **Album Browsing** — Look up albums by title or artist with release dates and track listings
- **Playlist Exploration** — Search public playlists by mood, genre, or curator
- **Charts** — Check top tracks, albums, artists, and playlists globally or by country
- **Genre Navigation** — Browse music genres and find curated playlists per genre

### How it works

1. Subscribe to this server
2. No API key required — Deezer public API is open for reading
3. Start exploring music from Claude, Cursor, or any MCP-compatible client


## Available Tools
- **get_album**: Get detailed album information
- **get_album_tracks**: Get tracks from an album
- **get_artist_radio**: Get artist radio tracks
- **get_artist**: Get detailed artist information
- **get_artist_top_tracks**: Get top tracks for an artist
- **get_chart**: Optionally filter by country using ISO 3166-1 country code.

Get Deezer charts
- **get_genre_playlists**: Get playlists for a genre
- **get_genre**: Get genre information
- **get_playlist**: Get detailed playlist information
- **get_track**: Get detailed track information
- **search_albums**: Returns albums with release date, track count, and cover art info.

Search for albums on Deezer
- **search_artists**: Returns artist info including fan count, album count, and profile links.

Search for artists on Deezer
- **search_playlists**: Returns playlist info including creator, track count, and fan count.

Search for playlists on Deezer
- **search_tracks**: Returns tracks with title, artist, album, duration, and preview link. Supports pagination with limit and offset index.

Search for tracks on Deezer


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Deezer** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Search for songs by Daft Punk."

**🤖 AI Agent:**
> Found 25 Daft Punk tracks. Top results: 'Get Lucky' (feat. Pharrell Williams, 6:09), 'One More Time' (5:20), and 'Harder Better Faster Stronger' (3:45). Want their top 10 tracks?

---

**👤 You:**
> "What's trending in Brazil right now?"

**🤖 AI Agent:**
> Brazil's top tracks: #1 'Barulho do Foguete' by Zé Neto & Cristiano, #2 'Oi Balde' by Henrique & Juliano. Top album: 'Nosso Quadro' by Ana Castela. Would you like the full top 10?

---

**👤 You:**
> "Find me chill playlists for studying."

**🤖 AI Agent:**
> Found 5 chill study playlists: 'Chill Study' (120 tracks, 45K fans), 'Lo-Fi Beats' (85 tracks), 'Peaceful Piano' (200 tracks). The top one has a great mix of ambient and lo-fi.


## ❓ FAQ

**Q: Do I need a Deezer account or API key to use this?**
No! The Deezer public API is open for reading without authentication. You can search tracks, artists, albums, playlists, and charts immediately.

**Q: Can I listen to song previews?**
Yes! Every track returned by the search includes a 30-second preview URL that you can play directly in your browser.

**Q: Can I get charts for a specific country?**
Yes! Use the `get_chart` tool with a country code (e.g., US, BR, FR, DE) to get the top tracks, albums, artists, and playlists for that region.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/deezer](https://vinkius.com/mcp/deezer)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Deezer** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `deezer` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Deezer** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "deezer": {
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
