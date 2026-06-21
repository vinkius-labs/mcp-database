# Spotify Music MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/spotify-music)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [industry-titans](../categories/industry-titans.md)

Control playback, search library, get audio features, and manage playlists via Spotify API.

## Description
Connect **Spotify** to any AI agent and turn your voice or text prompts into music actions — search millions of tracks, analyze audio features, get personalized recommendations, and control your playback.

### What you can do
- **Search Library** — Find any track, artist, album, or playlist by name
- **Player Control** — Play, pause, and add tracks to your queue directly
- **Audio Analytics** — Get deep insights like danceability, energy, valence, and tempo
- **Recommendations** — Discover new music based on your favorite artists or genres
- **Library Management** — View your playlists and get details about albums or artists
- **New Releases** — Discover the newest albums dropping on Spotify

### How it works
1. Subscribe to this server
2. Enter your Spotify Access Token (from the Developer Dashboard)
3. Start listening and discovering music from Claude, Cursor, or any MCP-compatible client

### Who is this for?
- **Music Lovers** — Discover new songs, get recommendations, and analyze their favorite tracks
- **Party Hosts** — Search for upbeat playlists and manage the playback queue without touching the app
- **Data Geeks** — Explore the audio features of songs to understand what makes a track 'danceable' or 'energetic'


## Available Tools
- **get_album**: Get information about a specific album
- **get_artist**: Get information about a specific artist
- **get_current_track**: Returns empty if nothing is playing.

Get the track currently playing on the user's device
- **search**: Search for tracks, artists, albums, or playlists on Spotify
- **get_track**: Get detailed information about a specific track
- **get_user_playlists**: Get the current user's playlists
- **get_audio_features**: Get audio features for a track (Danceability, Energy, Tempo, etc)
- **get_new_releases**: Get a list of new album releases
- **pause**: Pause playback on the user's device
- **play**: Start or resume playback on the user's device
- **get_playlist**: Get details of a specific playlist
- **add_to_queue**: Add a track to the playback queue
- **get_recommendations**: Get recommended tracks based on seed artists, genres, or tracks


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Spotify Music** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Play some energetic Jazz for studying."

**🤖 AI Agent:**
> Found some high-energy Jazz tracks. Adding to queue and resuming playback.

---

**👤 You:**
> "What are the audio features for 'Blinding Lights'?"

**🤖 AI Agent:**
> Blinding Lights: Danceability 51%, Energy 73%, Tempo 171 BPM, Valence 33%. It's a very fast, energetic song but with a somewhat melancholic vibe.

---

**👤 You:**
> "Show me the top 5 new releases."

**🤖 AI Agent:**
> Top New Releases: 1. New Album - Artist A. 2. Single Release - Artist B. 3. EP - Artist C. 4. Album - Artist D. 5. Single - Artist E.


## ❓ FAQ

**Q: How do I get a Spotify Access Token?**
Go to the Spotify Developer Dashboard, log in with your Spotify account, click 'Create App', and generate a token. The token expires every hour.

**Q: What are 'Audio Features'?**
Audio features are data points Spotify calculates for every track, including Danceability (0-100%), Energy (0-100%), Tempo (BPM), and Valence (Positivity). You can use `get_audio_features` to analyze a song's vibe.

**Q: Can I control playback on any device?**
Yes! The player tools (`play`, `pause`, `add_to_queue`) work on your currently active Spotify device, whether it's your phone, computer, or smart speaker.

**Q: Does it support podcasts?**
This integration currently focuses on music and library management. Podcast playback is not directly exposed as native commands.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/spotify-music](https://vinkius.com/mcp/spotify-music)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Spotify Music** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `spotify-music` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Spotify Music** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "spotify-music": {
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
