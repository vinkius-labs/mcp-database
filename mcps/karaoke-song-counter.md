# Karaoke Song Counter MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/karaoke-song-counter)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Analyze and count karaoke song queues based on artists, users, and unique songs.

## Description
This MCP server provides tools to manage and analyze karaoke session queues. It allows AI agents to calculate total request volumes, identify unique song-artist pairings, and filter statistics by specific artists or users. Use `get_queue_summary` to get a high-level overview of the session, or `count_unique_songs` to see the diversity of the repertoire.


## Available Tools (5)
- **count_songs_by_user**: Counts how many songs a specific user requested
- **count_total_requests**: Counts the total number of song requests in the queue
- **count_unique_songs**: Counts the number of unique song-artist pairings in the queue
- **get_queue_summary**: Provides an overall summary of the karaoke queue
- **count_songs_by_artist**: Counts how many times a specific artist was requested


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Karaoke Song Counter** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is the summary of this karaoke queue: [{"title": "Bohemian Rhapsody", "artist": "Queen", "user": "Alice"}, {"title": "Bohemian Rhapsody", "artist": "Queen", "user": "Bob"}, {"title": "Stayin' Alive", "artist": "Bee Gees", "user": "Alice"}]?"

**🤖 AI Agent:**
> The queue has 3 total requests, 2 unique songs, and the most requested artist is Queen.

---

**👤 You:**
> "How many unique songs are in this queue: [{"title": "Song A", "artist": "Artist 1"}, {"title": "Song A", "artist": "Artist 1"}, {"title": "Song B", "artist": "Artist 2"}]?"

**🤖 AI Agent:**
> There are 2 unique songs in the queue.

---

**👤 You:**
> "How many times has Queen been requested in this queue: [{"title": "Bohemian Rhapsody", "artist": "Queen"}, {"title": "Dancing Queen", "artist": "ABBA"}, {"title": "Killer Queen", "artist": "Queen"}]?"

**🤖 AI Agent:**
> Queen has been requested 2 times.


## ❓ FAQ

**Q: How do I provide the song queue?**
You must provide the song queue as a JSON string array of objects containing song and artist metadata.

**Q: How does the system handle duplicate songs?**
The `count_unique_songs` tool identifies unique song-artist pairings, while `count_total_requests` counts every single entry in the queue.

**Q: Can I filter songs by a specific person?**
Yes, you can use `count_songs_by_user` to find out how many songs a specific user has requested.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/karaoke-song-counter](https://vinkius.com/en/ai-agent-connect/karaoke-song-counter)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Karaoke Song Counter** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `karaoke-song-counter` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Karaoke Song Counter** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "karaoke-song-counter": {
      "url": "https://edge.vinkius.com/[TOKEN]/mcp"
    }
  }
}
```

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius connector registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
