# SoundCloud MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/soundcloud-alternative)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [audio-music](../categories/audio-music.md)

Search, stream, and manage SoundCloud tracks, playlists, and social interactions directly from your AI agent.

## Description
Connect your **SoundCloud** account to any AI agent to discover music, manage your library, and interact with the world's largest audio community through natural conversation.

### What you can do

- **Search & Discovery** — Find tracks using keywords, filters, and access levels to find exactly what you want to hear.
- **Streaming Access** — Retrieve stream URLs and transcoding details for specific tracks to integrate audio into your workflow.
- **Content Management** — Upload new tracks directly or create and organize playlists with ease.
- **Social Engagement** — Follow your favorite artists and like tracks or playlists to curate your personal feed.
- **URL Resolution** — Instantly convert any SoundCloud permalink into full API resource data for deep inspection.

### How it works

1. Subscribe to this server
2. Enter your SoundCloud Access Token
3. Start searching and managing audio from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Content Creators** — Quickly find and manage audio assets for projects without leaving the chat interface.
- **Music Enthusiasts** — Curate playlists and discover new artists through conversational search.
- **Developers** — Test SoundCloud API integrations and resolve track metadata directly within your IDE.


## Available Tools (9)
- **upload_track**: asset_data should be the raw file content or a placeholder for this MCP implementation.

Upload a new track to SoundCloud
- **create_playlist**: Create a new playlist
- **follow_user**: Follow a user
- **get_track_stream**: Get stream URLs for a track
- **like_playlist**: Like a playlist
- **like_track**: Like a track
- **get_me**: Get current SoundCloud user details
- **resolve_url**: Resolve a SoundCloud URL
- **search_tracks**: Search for tracks on SoundCloud


## 💬 Prompt Examples

Here are some examples of how you can interact with the **SoundCloud** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Search for lo-fi hip hop tracks on SoundCloud with a limit of 5 results."

**🤖 AI Agent:**
> I found 5 lo-fi hip hop tracks for you. Highlights include 'Midnight Study' by LofiGirl and 'Rainy Nights'. Would you like the stream URLs for any of these?

---

**👤 You:**
> "Identify the track at this URL: https://soundcloud.com/forss/flickermood"

**🤖 AI Agent:**
> Resolving URL... That link corresponds to the track 'Flickermood' by Forss (ID: 12345). It has over 1 million plays and is tagged as 'Electronic'.

---

**👤 You:**
> "Like the track with ID 12345 for me."

**🤖 AI Agent:**
> Done! I've added track 12345 ('Flickermood') to your liked tracks on SoundCloud.


## ❓ FAQ

**Q: How can I get the details of a track if I only have the browser URL?**
You can use the `resolve_url` tool. Simply provide the SoundCloud permalink (e.g., https://soundcloud.com/artist/track), and the agent will return the full API resource including ID, title, and metadata.

**Q: Can I upload audio files directly through this server?**
Yes! The `upload_track` tool allows you to send a title and the asset data to SoundCloud. This is perfect for automating uploads or managing your creator profile.

**Q: Is it possible to get the actual stream link for a track?**
Absolutely. Use the `get_track_stream` tool with a valid Track ID to retrieve available transcodings and direct stream URLs.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/soundcloud-alternative](https://vinkius.com/mcp/soundcloud-alternative)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **SoundCloud** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `soundcloud-alternative` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **SoundCloud** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "soundcloud-alternative": {
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
