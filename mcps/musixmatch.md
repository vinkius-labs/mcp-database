# Musixmatch MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/musixmatch)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [audio-music](../categories/audio-music.md)

Largest music lyrics database — search tracks, retrieve lyrics, and identify artists via AI.

## Description
Equip your AI agent with the most comprehensive music intelligence available via **Musixmatch**. This unified server provides your agent with instant access to millions of lyrics, track metadata, and artist profiles. Your agent can search for songs by title or lyrics, retrieve full song texts, and explore artist discographies without you ever searching manually. Whether you are identifying a song from a snippet or auditing lyrics for creative projects, your agent acts as a dedicated global music expert and discographer through natural conversation.

### What you can do

- **Track Discovery** — Search for music tracks by name, artist, or even specific lyric keywords.
- **Lyrics Retrieval** — Fetch the complete lyrics for millions of songs across all genres and languages.
- **Artist Intelligence** — Search for artists and retrieve detailed metadata and discographies.
- **Lyrics Snippets** — Quickly identify a song using a short snippet of its lyrics.
- **Top Charts** — Access the top tracks chart for any country to stay updated on current music trends.
- **Discography Auditing** — List all albums for a specific artist to explore their entire body of work.

### How it works

1. Subscribe to this server
2. Enter your Musixmatch API Key
3. Start managing your music intelligence from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Music Enthusiasts** — find full lyrics and explore artist discographies through simple natural language.
- **Content Creators** — retrieve song snippets and metadata for video production and media analysis.
- **Karaoke & Event Organizers** — quickly compile lyrics lists and track information for themed events.
- **Data Analysts** — perform trend analysis on top tracks and artist popularity across different regions.
- **Songwriters & Musicians** — audit existing lyrics for inspiration and reference in their own creative process.


## Available Tools (9)
- **get_artist_albums**: Get artist albums
- **get_artist_details**: Get artist metadata
- **get_track_lyrics**: Get track lyrics
- **get_track_snippet**: Get track snippet
- **get_track_details**: Get track metadata
- **match_track_lyrics**: Match lyrics by track and artist
- **search_artists**: Search for artists
- **search_tracks**: Search for music tracks
- **get_top_tracks**: Get top tracks chart


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Musixmatch** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Search for the song lyrics of 'Bohemian Rhapsody' by Queen."

**🤖 AI Agent:**
> I've retrieved the lyrics for 'Bohemian Rhapsody'. It's a masterpiece that spans several musical styles. Would you like me to display the full text or just a specific section?

---

**👤 You:**
> "What albums has 'Coldplay' released?"

**🤖 AI Agent:**
> Searching for Coldplay's discography... I've found a comprehensive list of their albums, including 'Parachutes', 'A Rush of Blood to the Head', and 'Music of the Spheres'. Shall I list them all for you?

---

**👤 You:**
> "Show me the top 10 songs in the US right now."

**🤖 AI Agent:**
> Retrieving the current US top chart... Here are the top 10 tracks, featuring artists like Taylor Swift, Drake, and SZA. Would you like more details on any of these songs?


## ❓ FAQ

**Q: Can I search for a song using only a few words from the lyrics?**
Yes! Use the `search_tracks` tool and provide the words in the `q_lyrics` parameter. Your agent will find all tracks that contain those specific lyrics.

**Q: How do I get the full discography for a specific artist?**
First, find the artist's unique ID using `search_artists`. Then, use the `get_artist_albums` tool with that ID to retrieve the list of all their recorded albums.

**Q: Is it possible to see which songs are currently trending in my country?**
Absolutely. Use the `get_top_tracks` tool and provide your country code (e.g., 'us', 'br', 'fr'). Your agent will return the current top tracks chart for that location.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/musixmatch](https://vinkius.com/mcp/musixmatch)
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
3. Set Type to "SSE" (or "streamable HTTP"), enter `musixmatch` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Musixmatch** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "musixmatch": {
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
