# Genius MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/genius)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [artificial-intelligence](../categories/artificial-intelligence.md)

Search songs, get lyrics, annotations and artist info — the world's largest lyrics database.

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


## Available Tools (7)
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


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Genius** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Search for Bohemian Rhapsody."

**🤖 AI Agent:**
> Found: Bohemian Rhapsody — Queen. 15M+ pageviews. Release: 1975. Album: A Night at the Opera. 🔗 genius.com/Queen-bohemian-rhapsody-lyrics

---

**👤 You:**
> "Get the lyrics for Bohemian Rhapsody."

**🤖 AI Agent:**
> Full lyrics returned including all verses: 'Is this the real life? Is this just fantasy...' through 'Anyway the wind blows'. Includes artist, album, producers and release date.

---

**👤 You:**
> "Show me annotations for 'Scaramouche' in Bohemian Rhapsody."

**🤖 AI Agent:**
> Found annotation for 'Scaramouche, Scaramouche, will you do the Fandango': Explains the commedia dell'arte character reference and the Fandango dance. 500+ upvotes.


## ❓ FAQ

**Q: How do I get a Genius access token?**
Register at [**genius.com/api-clients**](https://genius.com/api-clients) and create an API client. You'll get an access token immediately. It's free.

**Q: Can I get full lyrics for songs?**
Yes! The get_song endpoint returns full lyrics in plain text and HTML formats. Annotations provide explanations of specific lyric fragments.

**Q: What are annotations?**
Annotations are community-written explanations of specific lyric fragments. They explain references, wordplay, cultural context, biographical details and the meaning behind the lyrics. Each annotation has vote counts showing community approval.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/genius](https://vinkius.com/mcp/genius)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Genius** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `genius` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Genius** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "genius": {
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
