# Lyrics.ovh MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/lyricsovh)
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


## ❓ FAQ

**Q: How do I find the lyrics for a specific song?**
Use the `get_lyrics` tool by providing the exact artist name and song title. The agent will return the full lyrics available in the database.

**Q: What if I don't know the exact title of a song?**
You can use the `suggest_songs` tool with any search term (artist, partial title, or album). It will return a list of matching suggestions to help you identify the correct track.

**Q: Is there a limit to how many lyrics I can fetch?**
The server supports standard egress limits (up to 2MB per request), which is more than enough for any song lyrics. You can query as many songs as needed for your conversation.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/lyricsovh](https://vinkius.com/mcp/lyricsovh)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Lyrics.ovh** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `lyricsovh` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Lyrics.ovh** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "lyricsovh": {
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
