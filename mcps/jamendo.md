# Jamendo MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/jamendo)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [developer-tools](../categories/developer-tools.md)

Search and stream music from the Jamendo catalog — find tracks, albums, and artists, and explore playlists directly from your AI agent.

## Description
Connect to the **Jamendo** music library and integrate a world of independent music into your AI workflows through natural conversation.

### What you can do

- **Track Discovery** — Search the extensive catalog using tags, speed (high/medium/low), or vocal/instrumental filters via `search_tracks`.
- **Artist & Album Insights** — Fetch detailed metadata for artists and albums, including geographical locations and reviews.
- **Similar Music** — Use `get_similar_tracks` to find music similar to a specific track ID for perfect recommendations.
- **Playlist Exploration** — Search and filter public or user playlists to find curated collections.
- **Geographical Filtering** — Locate artists by country or city to discover local independent talent.

### How it works

1. Subscribe to this server
2. Enter your Jamendo Client ID
3. Start discovering and managing music from Claude, Cursor, or any MCP-compatible client

No more manual searching for royalty-free or independent music. Your AI acts as a music supervisor or personal DJ.

### Who is this for?

- **Content Creators** — instantly find background tracks based on specific moods, tags, or speeds.
- **Developers** — integrate music discovery and metadata retrieval into your coding environment.
- **Music Enthusiasts** — explore new independent artists and similar tracks through simple chat commands.


## Available Tools
- **get_album_reviews**: Browse and filter community album reviews
- **get_album_tracks**: Retrieve tracks belonging to specific albums
- **search_albums**: Search and filter albums
- **get_artist_albums**: Retrieve albums for specific artists
- **get_artist_locations**: Filter artists by geographical location
- **get_artist_tracks**: Retrieve tracks for specific artists
- **search_artists**: Search and filter artists
- **autocomplete_search**: Prefix-based search for tracks, albums, artists, and tags
- **get_feeds**: Editorial content and news from the Jamendo homepage
- **get_playlist_tracks**: Retrieve tracks within a playlist
- **search_playlists**: Search and filter public or user playlists
- **get_radio_stream**: Get stream URL and now playing info for a radio
- **list_radios**: List Jamendo radio stations
- **set_user_dislike**: Dislike a track. Requires OAuth2 access token
- **set_user_fan**: Become a fan of an artist. Requires OAuth2 access token
- **set_user_favorite**: Add a track to user favorites. Requires OAuth2 access token
- **set_user_like**: Like a track. Requires OAuth2 access token
- **set_user_playlist**: Create or update a user playlist. Requires OAuth2 access token
- **get_similar_tracks**: Find tracks similar to a given track ID
- **get_track_reviews**: Browse and filter community track reviews
- **search_tracks**: Search and filter the Jamendo track catalog
- **get_user_albums**: Retrieve albums a user has interacted with
- **get_user_artists**: Retrieve artists a user has interacted with
- **get_user_tracks**: Retrieve tracks a user has interacted with
- **get_users**: Lookup user profile information


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Jamendo** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Search for high-speed instrumental tracks with the tag 'rock'."

**🤖 AI Agent:**
> I've searched the Jamendo catalog for high-speed instrumental rock. I found several tracks, including 'Electric Storm' and 'Fast Lane'. Would you like the streaming links for these?

---

**👤 You:**
> "Find artists located in Paris, France."

**🤖 AI Agent:**
> I've queried the artist locations. In Paris, France, I found artists like 'L'Atelier' and 'The Parisian Jazz Project'. Would you like to see their top albums?

---

**👤 You:**
> "Get tracks similar to track ID 12345."

**🤖 AI Agent:**
> Analyzing track 12345... I've found 5 similar tracks that match its style and tempo, including 'Midnight Sun' and 'Ocean Breeze'. Shall I list their details?


## ❓ FAQ

**Q: Can I search for music based on specific moods or technical attributes like speed?**
Yes! Use the `search_tracks` tool with parameters like `tags` for mood and `speed` (high, medium, low) to filter the catalog exactly how you need.

**Q: How do I find artists from a specific city or country?**
You can use the `get_artist_locations` tool. Simply provide the `location_country` (code) or `location_city` to see a list of artists from that area.

**Q: Is it possible to get recommendations based on a track I like?**
Absolutely. Use the `get_similar_tracks` tool with the ID of the track you like, and the agent will return a list of musically similar tracks from the Jamendo library.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/jamendo](https://vinkius.com/mcp/jamendo)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Jamendo** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `jamendo` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Jamendo** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "jamendo": {
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
