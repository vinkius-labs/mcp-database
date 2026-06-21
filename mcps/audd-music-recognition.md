# AudD Music Recognition MCP Server

Universal music recognition — identify songs from URLs, search lyrics, and find streaming links via AI.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/audd-music-recognition)

## Overview
**Category:** artificial-intelligence
**Tools Count:** 8

## Description
Equip your AI agent with the power of **AudD**, the leading music recognition and data platform. This integration allows your agent to identify songs from audio URLs, search for track information by title or artist, and retrieve full lyrics or snippets. Your agent can also find direct streaming links for identified tracks on platforms like Spotify and Apple Music. Whether you are identifying a background track from a video or searching for that one song with a specific lyric, your agent acts as a dedicated musicologist through natural conversation.

### What you can do

- **Music Recognition** — Identify songs from publicly accessible audio URLs with high precision.
- **Lyrics Search** — Find full lyrics or search for songs using fragments of text.
- **Metadata Retrieval** — Fetch detailed track, artist, and album information including release dates and labels.
- **Streaming Links** — Get direct URLs to listen to identified tracks on major music platforms.
- **Timecode Identification** — Start recognition from a specific offset to identify songs in long audio files.

### How it works

1. Subscribe to this server
2. Enter your AudD API Token
3. Start managing your music discovery from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Content Creators** — identify background music in videos or find tracks for their productions.
- **Music Enthusiasts** — search for lyrics and find where to stream their favorite songs.
- **Developers** — integrate music identification capabilities into their AI workflows.
- **Researchers** — analyze music metadata and release histories across a massive database.


## Available Tools
- **add_monitored_stream**: Add an audio stream to monitor for music
- **get_lyrics**: Get full lyrics for a specific track
- **list_monitored_streams**: List all monitored audio streams
- **recognize_at_time**: Useful for long files.

Recognize music starting at a specific offset
- **recognize_music**: Returns artist, title, album, and streaming links (Apple Music, Spotify, etc.).

Recognize a song from an audio URL
- **search_lyrics**: Returns matched lyrics and song metadata.

Search for song lyrics by text fragment
- **search_music**: Search for a song by text query
- **set_stream_callback_url**: Set the webhook URL for stream monitoring results


## Installation & Usage

To install and use the **AudD Music Recognition** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/audd-music-recognition](https://vinkius.com/mcp/audd-music-recognition)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
