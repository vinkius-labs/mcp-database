# Genius MCP Server

Search songs, get lyrics, annotations and artist info — the world's largest lyrics database.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/genius)

## Overview
**Category:** artificial-intelligence
**Tools Count:** 7

## Description
Connect to **Genius** and access the world's largest lyrics database through natural conversation.

### What you can do

- **Song Search** — Search millions of songs by title, lyrics, artist name or any keyword
- **Song Details** — Get full song info including lyrics (plain text), artist, album, release date and producers
- **Annotations** — Read community-written explanations of lyrics, references, wordplay and meaning
- **Artist Info** — Get artist profiles with IQ scores, images and Genius page URLs
- **Artist Songs** — Browse all songs by a specific artist
- **Album Info** — Get album details including track lists and artist info

### How it works

1. Subscribe to this server
2. Enter your Genius Access Token (free at genius.com/api-clients)
3. Start exploring lyrics and annotations from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Music Fans** — find song lyrics, read annotations and understand the meaning behind lyrics
- **Researchers** — analyze lyrics, annotations and music knowledge data
- **Content Creators** — access song info, lyrics and annotations for content creation


## Available Tools
- **get_album**: Returns album name, artist, cover art, release date and track list. Use the album ID from song results or search.

Get album details including track list and artist
- **get_annotation**: Returns the annotated text, full explanation body (in plain text and HTML), author info, vote counts and cosigns. Use the annotation ID from get_song_annotations results.

Get details for a specific annotation (explainer text)
- **get_artist**: Returns artist name, IQ score, profile image, description and Genius page URL. Use the artist ID from song search results or get_artist_songs.

Get artist profile info including name, IQ and image
- **get_artist_songs**: Returns song titles, pageview counts and Genius URLs. Paginated — use page parameter to navigate through results.

Get all songs by a specific artist
- **get_song**: Returns full title, artist, album, release date, producer info, song art, Genius page URL and full lyrics (in plain text and HTML formats). Use the song ID from search_songs results.

Get detailed info for a specific song including lyrics
- **get_song_annotations**: Annotations are community-written explanations of lyrics, references, wordplay and meaning. Returns annotated lyric fragments with explanation text, author info and vote counts. Use the song ID from search_songs.

Get annotations (explainer text) for a specific song
- **search_songs**: Returns song titles, artist names, pageview counts and Genius URLs. Use this to find songs before getting detailed info with get_song.

Search for songs on Genius by title, lyrics or artist


## Installation & Usage

To install and use the **Genius** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/genius](https://vinkius.com/mcp/genius)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
