# Mixcloud Shows & Mixes MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/mixcloud-shows-mixes)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [audio-music](../categories/audio-music.md)

Mixcloud as an MCP: search DJ mixes, radio shows and podcasts, get full cloudcast details with tracklists, browse uploader catalogues and 38 genre categories — public read-only API, no key needed.

## Description
**Mixcloud** — the home of DJ mixes, radio shows and long-form podcasts — as a single MCP server.

### What you can do
- **Search cloudcasts** — DJ sets, radio shows and podcasts by keyword, with play/favourite counts and audio length
- **Tracklists** — cloudcast details include the sections array (tracklist with timestamps when uploaded)
- **Uploader catalogues** — browse the entire show archive of any radio station, DJ or label
- **38 genre categories** — ambient to drum-and-bass to house: genre-based discovery with paging

### Why Mixcloud?
Unlike other audio platforms, Mixcloud specialises in **long-form audio with licensed tracklists** — the only place where commercial DJ sets and radio shows are legal. Its public API needs no key for discovery.

### Who is this for?
Music supervisors, DJs, radio producers, playlist curators, event promoters and AI agents that search curated audio shows by genre, uploader or tracklist.


## Available Tools (6)
- **get_cloudcast**: Keys come from search/list tools (format /user/slug/).

Get full cloudcast detail: tracklist sections, description, tags, stats
- **get_user**: username is the URL slug (e.g. Radio_RapTz from search_uploaders).

Get a Mixcloud uploader profile: bio, follower count and stats
- **search_cloudcasts**: Pagination via limit/offset. Note: no total count is returned — page until empty.

Search DJ mixes, radio shows and podcasts (cloudcasts) by keyword on Mixcloud
- **search_uploaders**: Search radio stations by name to explore their show archives.

Search Mixcloud users: DJs, radio stations, labels and podcast creators
- **browse_category**: Use for genre-based discovery: "what's new in drum and bass?".

Browse Mixcloud genre categories (38: ambient, bass, beats, dnb...) and their trending cloudcasts
- **list_user_cloudcasts**: Each entry: key (for get_cloudcast), name, play counts, tags, audio length. Great for exploring a radio station's full show archive.

List all cloudcasts (shows/mixes) published by a Mixcloud user


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Mixcloud Shows & Mixes** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Find lo-fi jazz mixes on Mixcloud"

**🤖 AI Agent:**
> 📻 **Cloudcast search: lo-fi jazz**

Top results:
- Groove Caché #8 Lo-Fi Jazz by MoFo (Radio_RapTz) — 848 plays, 1h30
- Lo-Fi Jazz Study Session — 12k plays

All with tracklist sections where provided. Want me to pull the full tracklist of the first one?

---

**👤 You:**
> "Explore the drum-and-bass category — what's trending?"

**🤖 AI Agent:**
> 🎧 **Category: drum-and-bass**

Browse via /categories/dnb/cloudcasts/ with offset paging:
- Weekly hospital records shows
- Classic 1990s jungle sets
- Liquid DNB megamixes

The category listing includes play counts for trend ranking. Want the top 10 by plays?

---

**👤 You:**
> "Explore Radio RapTz's full show archive"

**🤖 AI Agent:**
> 📻 **Radio RapTz — 7132 cloudcasts, 13.4k followers**

Full archive browseable with pagination: Underground Soundz Vol. 123 ft. Dj Halabi, Groove Caché series, weekly radio shows...

I can page through the entire catalogue, or pull the tracklist of any individual show.


## ❓ FAQ

**Q: Do I need an API key?**
Not for any discovery tool in this MCP — search, cloudcast details, user profiles, catalogues and categories are all public. An access token is only required if you want /me endpoints (your own favourites and uploads), which this MCP exposes as an optional credential.

**Q: How do I get a tracklist for a show?**
Use get_cloudcast with the cloudcast key from search results — the detail response includes the sections array, which is the tracklist with start-time offsets when the uploader timestamped their show.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/mixcloud-shows-mixes](https://vinkius.com/en/ai-agent-connect/mixcloud-shows-mixes)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Mixcloud Shows & Mixes** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `mixcloud-shows-mixes` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Mixcloud Shows & Mixes** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "mixcloud-shows-mixes": {
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
