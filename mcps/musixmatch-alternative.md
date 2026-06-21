# Musixmatch MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/musixmatch-alternative)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [audio-music](../categories/audio-music.md)

Access the world's largest lyrics database — search tracks, retrieve synchronized subtitles, and explore global music charts directly from your AI agent.

## Description
Connect your **Musixmatch** developer account to any AI agent and unlock deep access to millions of lyrics, track metadata, and music charts through natural conversation.

### What you can do

- **Track Search** — Find any song in the Musixmatch catalogue using title, artist name, or even a specific phrase from the lyrics via `search_tracks`.
- **Lyrics & Subtitles** — Fetch full song lyrics with `get_track_lyrics` or get synchronized time-coded subtitles (LRC format) using `get_track_subtitle`.
- **Global Charts** — Retrieve the top trending artists and tracks for any specific country or worldwide using `get_chart_artists` and `get_chart_tracks`.
- **Artist & Album Insights** — Explore discographies, fetch artist metadata, and list all tracks within a specific album using `get_artist_albums` and `get_album_tracks`.
- **Music Genres** — Query the official list of music genres to categorize your search results effectively.

### How it works

1. Subscribe to this server
2. Enter your Musixmatch API Key
3. Start exploring the world of music data from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Music Enthusiasts** — instantly find lyrics or identify songs from a few remembered words.
- **Developers & Creators** — integrate music metadata and synchronized lyrics into your apps or creative workflows.
- **Data Analysts** — track music trends and popular artists across different regions globally.


## Available Tools (21)
- **get_chart_artists**: Get the list of top artists of a given country
- **get_chart_tracks**: Get the list of top tracks of a given country
- **get_album**: Get album metadata
- **get_album_tracks**: Get the list of tracks for an album
- **get_artist_albums**: Get the list of albums for an artist
- **get_artist**: Get artist metadata
- **get_lyrics_translation**: Get the translation of a track lyrics
- **get_music_genres**: Get the list of music genres
- **get_subtitle_translation**: Get the translation of a track synchronized lyrics
- **get_track_lyrics**: Get the lyrics for a track
- **get_track_richsync**: Get the rich synchronized lyrics (word-by-word)
- **get_track_snippet**: Get a snippet (short excerpt) of the lyrics
- **get_track_subtitle**: Get the synchronized lyrics (subtitles) for a track
- **get_track**: Get a track metadata by ID
- **match_lyrics**: Match a track and get its lyrics in one call
- **match_subtitle**: Match a track and get its subtitles
- **match_track**: Match a track and get its metadata
- **post_work**: Submit or update publishing data for a musical work
- **post_work_validity**: Submit the validity end date for a work
- **search_artists**: Search for an artist
- **search_tracks**: Search for a track in the Musixmatch catalogue


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Musixmatch** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Search for tracks with the lyrics 'is this the real life' and tell me the artist."

**🤖 AI Agent:**
> I found the track! It's 'Bohemian Rhapsody' by the legendary band Queen. Would you like me to fetch the full lyrics for you?

---

**👤 You:**
> "Show me the top 5 tracks currently trending in the United Kingdom."

**🤖 AI Agent:**
> Fetching the UK charts... The top 5 tracks are: 1. 'Flowers' by Miley Cyrus, 2. 'Kill Bill' by SZA... [etc]. Would you like to see the lyrics for any of these?

---

**👤 You:**
> "Get the synchronized subtitles for the track 'Imagine' by John Lennon."

**🤖 AI Agent:**
> I've retrieved the synchronized subtitles for 'Imagine'. They are in LRC format, starting with: [00:14.63] Imagine there's no heaven... Would you like the full file?


## ❓ FAQ

**Q: Can I search for a song if I only remember a few words from the lyrics?**
Yes! You can use the `search_tracks` tool and provide the lyrics snippet in the `q_lyrics` parameter. The AI will return the most relevant song matches.

**Q: How do I get synchronized lyrics for a karaoke application?**
Use the `get_track_subtitle` tool. It provides time-coded lyrics in formats like LRC, which are perfect for displaying lyrics in sync with the music.

**Q: Is it possible to see which artists are currently trending in a specific country?**
Absolutely. Use the `get_chart_artists` tool and specify the `country` code (e.g., 'US', 'BR', 'FR') to get a list of the top-performing artists in that region.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/musixmatch-alternative](https://vinkius.com/mcp/musixmatch-alternative)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Musixmatch** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `musixmatch-alternative` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Musixmatch** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "musixmatch-alternative": {
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
