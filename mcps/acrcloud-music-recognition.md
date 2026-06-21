# ACRCloud Music Recognition MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/acrcloud-music-recognition)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [artificial-intelligence](../categories/artificial-intelligence.md)

Identify and explore music via ACRCloud — recognize songs from audio files and retrieve rich metadata.

## Description
Connect your AI agent to **ACRCloud**, the world-leading automatic content recognition (ACR) service. This integration allows you to identify music from audio samples and explore a massive database of tracks, artists, and albums with rich metadata and streaming links.

### What you can do

- **Music Identification** — Send an audio file URL to instantly identify the song, artist, and album using advanced fingerprinting
- **Deep Metadata Search** — Query the global music database for tracks, albums, and artists using text or codes (ISRC)
- **Streaming Links** — Automatically retrieve IDs and direct links for Spotify, YouTube, and other major platforms
- **Professional Analytics** — Get confidence scores and release details for identified audio content

### How it works

1. Subscribe to this server
2. Enter your **ACRCloud Access Key**, **Secret**, and **Host** (available in your ACRCloud dashboard)
3. Start identifying and exploring music directly through natural conversation

### Who is this for?

- **Content Creators** — quickly identify background music or check for copyright metadata
- **Music App Developers** — integrate track identification and metadata retrieval into your AI workflows
- **Music Enthusiasts** — explore discographies and find streaming links for your favorite tracks


## Available Tools
- **get_track_by_isrc**: Retrieve detailed metadata for a track using its ISRC code
- **identify_music_from_url**: Identify a song from an audio file URL (e.g., mp3, wav)
- **search_albums**: Search for music albums by title or artist
- **search_artists**: Search for music artists by name
- **search_tracks**: Search for music tracks by name, artist, or lyric fragments


## 💬 Prompt Examples

Here are some examples of how you can interact with the **ACRCloud Music Recognition** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Identify this song: https://example.com/sample.mp3"

**🤖 AI Agent:**
> Identification successful! The song is 'Blinding Lights' by The Weeknd from the album 'After Hours'. Here is the Spotify link: [Spotify Link].

---

**👤 You:**
> "Search for tracks by 'Daft Punk'."

**🤖 AI Agent:**
> I've found several tracks by Daft Punk, including 'One More Time', 'Get Lucky', and 'Harder, Better, Faster, Stronger'. Which one would you like details for?

---

**👤 You:**
> "Get the Spotify link for the song with ISRC USAT20500447."

**🤖 AI Agent:**
> Searching... I've located the track 'Get Lucky' by Daft Punk. Here is the direct Spotify link: [Spotify Link]. It also includes metadata for Apple Music and YouTube.


## ❓ FAQ

**Q: How do I get ACRCloud credentials?**
Sign up at the [**ACRCloud Console**](https://console.acrcloud.com/), create a 'Music Recognition' project, and you will find your Access Key, Secret, and Host in the project settings.

**Q: Which audio formats are supported for identification?**
ACRCloud supports most common audio formats including MP3, WAV, AAC, and OGG. The agent will download the file from the provided URL and send it for fingerprinting.

**Q: Can I find the ISRC code for a specific track?**
Yes! When you identify a song or search for metadata, the `acr_music_search` tool returns industry-standard identifiers like ISRC, allowing you to track specific recordings across different systems.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/acrcloud-music-recognition](https://vinkius.com/mcp/acrcloud-music-recognition)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **ACRCloud Music Recognition** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `acrcloud-music-recognition` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **ACRCloud Music Recognition** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "acrcloud-music-recognition": {
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
