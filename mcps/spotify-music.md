# Spotify Music MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/spotify-music)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/spotify-music-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/spotify-music-mcp)
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


## Installation & Usage

To install and use the **Spotify Music** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/spotify-music](https://vinkius.com/mcp/spotify-music)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
