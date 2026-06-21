# Lyrics.ovh MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/lyricsovh)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/lyricsovh-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/lyricsovh-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [audio-music](../categories/audio-music.md)

Retrieve song lyrics and music suggestions instantly. Search by artist and title or explore suggestions for any search term.

## Description
Access the **Lyrics.ovh** database to bring music context into your AI conversations. Whether you are looking for specific lyrics or searching for new tracks, this server provides direct access to a vast library of song data.

### What you can do

- **Fetch Lyrics** — Get the full text of any song by providing the artist and track title.
- **Song Suggestions** — Search for artists, albums, or tracks to get a list of relevant suggestions.
- **Music Research** — Use the data to analyze themes, verify verses, or build playlists.

### How it works

1. Subscribe to this server
2. This server connects to the public Lyrics.ovh API
3. Start asking about your favorite songs in Claude, Cursor, or any MCP client

### Who is this for?

- **Music Enthusiasts** — quickly find lyrics without leaving your chat.
- **Content Creators** — verify song lines and artist details for scripts or articles.
- **Developers** — integrate music data into your coding workflows or creative projects.


## Available Tools
- **get_lyrics**: Retrieve the lyrics for a specific artist and song title
- **suggest_songs**: Find song suggestions based on a search term


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Lyrics.ovh** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Get the lyrics for 'Bohemian Rhapsody' by Queen."

**🤖 AI Agent:**
> I've retrieved the lyrics for 'Bohemian Rhapsody'. It starts with: 'Is this the real life? Is this just fantasy?...' Would you like the full text?

---

**👤 You:**
> "Suggest some songs related to 'Daft Punk'."

**🤖 AI Agent:**
> Searching for suggestions... I found several tracks including 'Get Lucky', 'One More Time', and 'Harder, Better, Faster, Stronger'. Which one should I look up lyrics for?

---

**👤 You:**
> "Find the lyrics for 'Imagine' by John Lennon."

**🤖 AI Agent:**
> I found the lyrics for 'Imagine'. The song conveys a message of peace with lines like 'Imagine there's no heaven, It's easy if you try...'. Shall I provide the rest?


## Installation & Usage

To install and use the **Lyrics.ovh** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/lyricsovh](https://vinkius.com/mcp/lyricsovh)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
