# Bandcamp MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/bandcamp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [ecommerce](../categories/ecommerce.md)

Discover independent music — search artists, albums and tracks, browse new releases and best sellers.

## Description
Connect to **Bandcamp** and discover independent music through natural conversation.

### What you can do

- **Music Search** — Search for artists, albums, tracks, labels and fans across all of Bandcamp
- **Artist Profiles** — Get artist bio, discography, location and social media links
- **Album Details** — View full album info including track lists, artwork, genres and purchase options
- **Track Info** — Get track details with duration, artwork and streaming options
- **New Releases** — Browse the latest album releases, optionally filtered by genre
- **Best Sellers** — Discover the best selling albums on Bandcamp
- **Featured Content** — Explore Bandcamp editorial picks for featured albums, tracks and artists
- **Genre Discovery** — Browse all available music genres on the platform

### How it works

1. Subscribe to this server
2. No API key needed — Bandcamp discovery is fully open
3. Start discovering indie music from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Music Fans** — discover new artists, explore albums by genre and find hidden gems
- **Journalists** — research indie artists, labels and music trends for articles and reviews
- **Curators** — find featured content, new releases and best sellers for playlists and collections


## Available Tools (8)
- **discover_music**: g. "electronic", "ambient", "hip-hop-rap", "rock", "jazz", "metal"). Returns albums with artist, title, art, and links. Use get_tags to see available genre tags.

Discover music on Bandcamp by genre
- **get_best_selling**: Returns titles, artists, artwork, and Bandcamp URLs.

Get best selling releases on Bandcamp by genre
- **get_featured**: Returns stories, albums, and curated picks.

Get featured editorial content from the Bandcamp front page
- **get_new_releases**: Returns titles, artists, artwork, release dates and Bandcamp URLs.

Get newest releases on Bandcamp by genre
- **get_page_data**: g. "https://artist.bandcamp.com/album/name"), extracts structured data including tracks, artist info, pricing, and embedded metadata. Works with album, track, and artist pages.

Extract album or artist data from a Bandcamp URL
- **get_recommended**: Returns titles, artists, artwork, and Bandcamp URLs.

Get recommended releases on Bandcamp by genre
- **get_tags**: Use these tags with discover_music, get_best_selling, and get_new_releases.

Get available genre tags on Bandcamp
- **search**: Returns names, types, URLs and artwork. Results include artists, albums, tracks, labels and fan profiles.

Search Bandcamp for artists, albums, tracks, labels and fans


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Bandcamp** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Search for ambient electronic artists."

**🤖 AI Agent:**
> Found 25 ambient electronic artists including: Stars of the Lid, Biosphere, Carbon Based Lifeforms, Loscil, 36. Each with bio, discography, location and social links.

---

**👤 You:**
> "What are the new releases in rock music?"

**🤖 AI Agent:**
> Found 20 new rock releases including albums from emerging and established artists. Each with artwork, track lists, genres, release dates and Bandcamp purchase links.

---

**👤 You:**
> "Show me Bandcamp's featured albums right now."

**🤖 AI Agent:**
> Current Bandcamp featured albums: 8 editorial picks across genres including post-rock, hip-hop, jazz, electronic and folk. Each with full details and purchase links.


## ❓ FAQ

**Q: Do I need an API key to use this?**
No! This integration works without any API key. Simply subscribe and start discovering music right away.

**Q: Can I stream music through the API?**
The API provides track metadata and links to Bandcamp pages where you can listen. Direct audio streaming is available on Bandcamp's website and app.

**Q: What genres are available?**
Bandcamp covers all major genres: rock, electronic, hip-hop, jazz, classical, metal, folk, ambient, punk, experimental, world music and many more. Use get_genres to see the full list.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/bandcamp](https://vinkius.com/mcp/bandcamp)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Bandcamp** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `bandcamp` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Bandcamp** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "bandcamp": {
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
