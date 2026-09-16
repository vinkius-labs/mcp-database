# Audiomack MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/audiomack)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [audio-music](../categories/audio-music.md)

Stream and discover music via Audiomack — search tracks, manage playlists, and follow artists directly from your AI agent.

## Description
Connect your **Audiomack** account to any AI agent and explore a vast library of music and podcasts through natural conversation.

### What you can do

- **Music Discovery** — Fetch trending music, recent uploads, and top charts filtered by genre to stay ahead of the curve.
- **Artist Interaction** — Access artist profiles, view their latest uploads, and follow or unfollow creators to personalize your feed.
- **Playlist Management** — Create, update, and delete playlists, or add/remove specific tracks to curate your perfect sound.
- **Social Engagement** — Favorite or repost tracks and albums to support your favorite artists directly from the chat.
- **Streaming Access** — Generate temporary streaming URLs to play tracks immediately within your compatible environment.

### How it works

1. Subscribe to this server
2. Enter your Audiomack API credentials (Consumer Key, Secret, and OAuth tokens)
3. Start discovering and managing your music library from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Music Enthusiasts** — discover new underground hits and trending tracks without leaving your workspace.
- **Content Curators** — build and manage playlists for streams or projects using simple voice or text commands.
- **Developers** — integrate music discovery and metadata retrieval into your automated workflows.


## Available Tools (28)
- **get_artist**: Supply the artist’s slug.

Get artist profile info
- **get_playlist_by_id**: Provide the ID to fetch the details.

Get playlist info by ID
- **repost_music**: Supply the unique identifier of the content to be reposted.

Repost a track or album (Requires Auth)
- **add_track_to_playlist**: You must specify both the playlist ID and the music ID.

Add a track to a playlist (Requires Auth)
- **create_playlist**: You must provide a title and genre for the playlist.

Create a new playlist (Requires Auth)
- **follow_artist**: Supply the artist’s slug.

Follow an artist (Requires Auth)
- **get_artist_favorites**: Provide the artist slug to target the correct data.

Get artist favorites
- **get_artist_followers**: Provide the artist slug, as this is a required parameter.

Get followers of an artist
- **get_artist_following**: Use the artist slug to specify the source artist.

Get users an artist is following
- **get_artist_playlists**: Supply the artist slug to identify the source.

Get artist playlists
- **get_artist_uploads**: Always provide the artist slug to filter results.

Get artist uploads
- **get_charts**: Specify the page number to navigate results.

Get Audiomack charts
- **get_music_by_id**: Get song or album info by ID
- **get_music_by_slug**: Get song or album info by slug
- **get_playlist_by_slug**: Provide either the artist or playlist slug.

Get playlist info by slug
- **get_trending_music**: Get trending music
- **play_music**: Play a track (Requires Auth)
- **remove_track_from_playlist**: Specify both the playlist ID and the music ID.

Remove a track from a playlist (Requires Auth)
- **search_autosuggest**: Provide a search query to get suggestions.

Get search autosuggestions
- **search**: Provide a search query to begin the search.

Search for music, artists, or albums
- **unfavorite_music**: Provide the unique identifier of the content to remove.

Remove a track or album from favorites (Requires Auth)
- **unfollow_artist**: Supply the artist’s slug.

Unfollow an artist (Requires Auth)
- **unrepost_music**: Provide the unique identifier of the content to un-repost.

Remove a reposted track or album (Requires Auth)
- **update_playlist**: You must provide the playlist ID to modify the details.

Edit an existing playlist (Requires Auth)
- **get_recent_music**: Get most recent music
- **delete_playlist**: Supply the unique playlist ID to confirm deletion.

Delete a playlist (Requires Auth)
- **favorite_music**: Use this tool only when the user explicitly requests favoriting content.

Favorite a track or album (Requires Auth)
- **flag_music_unplayable**: Supply both the artist and music slugs.

Flag a track or album as unplayable


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Audiomack** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Show me the top trending hip-hop songs on Audiomack right now."

**🤖 AI Agent:**
> I've fetched the trending hip-hop charts. Currently, 'Song Title A' by Artist X and 'Song Title B' by Artist Y are leading. Would you like to hear one of them?

---

**👤 You:**
> "Search for the artist '21 Savage' and list their latest uploads."

**🤖 AI Agent:**
> I found 21 Savage (ID: 54321). Their latest uploads include the album 'American Dream' and the single 'Redrum'. Should I add any of these to your favorites?

---

**👤 You:**
> "Create a new playlist called 'Focus Beats' and add track ID 987654 to it."

**🤖 AI Agent:**
> Playlist 'Focus Beats' has been created successfully. I've also added track 987654 to it. You can now manage this playlist using ID 112233.


## ❓ FAQ

**Q: How can I get a direct link to stream a song?**
You can use the `play_music` tool with the specific Music ID. It will register the play and return a temporary streaming URL for the MP3 file.

**Q: Is it possible to find the most popular songs in a specific genre like 'Afrobeats'?**
Yes! Use the `get_trending_music` or `get_charts` tools and provide the genre slug (e.g., 'afrobeats') to see what's currently topping the charts.

**Q: Can I add tracks to my existing playlists through the AI?**
Absolutely. Use the `add_track_to_playlist` tool by providing the Playlist ID and the Music ID you wish to add.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/audiomack](https://vinkius.com/en/ai-agent-connect/audiomack)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Audiomack** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `audiomack` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Audiomack** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "audiomack": {
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
