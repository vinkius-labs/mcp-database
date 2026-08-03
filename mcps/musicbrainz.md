# MusicBrainz MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/musicbrainz)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [audio-music](../categories/audio-music.md)

Explore the open music encyclopedia — search artists, albums, tracks, labels and musical works.

## Description
Connect to **MusicBrainz**, the world's largest open music database, and explore music metadata through natural conversation — no API key needed.

### What you can do

- **Artist Search** — Find musicians, bands, orchestras and composers with types, countries and active dates
- **Release Search** — Search album releases with artists, dates, countries, labels and track counts
- **Track Search** — Find individual recordings with durations, ISRCs and album info
- **Release Groups** — Browse canonical albums and singles grouped across different releases
- **Label Search** — Find record labels and publishers
- **Work Search** — Search musical compositions distinct from recordings
- **Browse** — Get all releases by a specific artist or label

### How it works

1. Subscribe to this server
2. No API key needed — start searching immediately
3. Explore music data from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Music Enthusiasts** — discover artist discographies, find album versions and explore music metadata
- **Researchers** — access comprehensive music metadata for analysis and cataloging
- **Developers** — build music apps using open, structured music data with MBIDs


## Available Tools (15)
- **browse_releases_by_artist**: Returns release titles, dates, countries and labels. Pagination: max 100 results per request.

Browse all releases by a specific artist
- **browse_releases_by_label**: Returns release titles, artists, dates and countries. Pagination: max 100 results.

Browse all releases by a specific record label
- **get_artist**: Returns name, type, country, life span, disambiguation and more. Optionally include related data with inc parameter: "releases", "release-groups", "recordings", "works", "aliases".

Get detailed info for a specific artist by MBID
- **get_label**: Returns label name, type, country, founding date and more.

Get detailed info for a specific record label by MBID
- **get_recording**: Returns title, artist, duration, ISRCs, releases it appears on and more. Optionally include: "artists", "isrcs", "releases", "aliases".

Get detailed info for a specific recording by MBID
- **get_release**: Returns title, artist, date, country, label, barcode, track listing and more. Optionally include: "artists", "labels", "recordings", "discids", "isrcs", "media".

Get detailed info for a specific release by MBID
- **get_release_group**: Returns title, artist, primary type, first release date and more. Optionally include: "artists", "releases", "aliases".

Get detailed info for a specific release group by MBID
- **get_work**: Returns work title, writers, type, ISWC, languages and more.

Get detailed info for a specific musical work by MBID
- **search_areas**: Returns area names, types (country, city, subdivision, etc.) and ISO codes. Useful for finding area IDs to use in other searches.

Search for geographic areas (countries, cities, regions)
- **search_artists**: ). Returns artist names, IDs, types (person, group, orchestra, etc.), countries, active dates and disambiguation info. Supports Lucene query syntax for advanced searches. Pagination: max 100 results per request.

Search for music artists
- **search_labels**: Returns label names, types (original production, reissue, etc.), countries and founding dates. Pagination: max 100 results.

Search for record labels
- **search_recordings**: Returns recording titles, artists, durations, album names and ISRCs. Useful for finding specific track versions and metadata. Pagination: max 100 results.

Search for individual track recordings
- **search_release_groups**: Returns titles, artists, primary types (album, single, EP, etc.) and dates. Useful for finding the canonical album/single version. Pagination: max 100 results.

Search for release groups (albums, singles, EPs)
- **search_releases**: Returns release titles, artists, dates, countries, labels and track counts. Supports filtering by status (official, promotion, bootleg). Pagination: max 100 results.

Search for album releases
- **search_works**: Returns work titles, writers, types (song, opera, symphony, etc.) and ISWCs. Useful for finding composition metadata separate from specific recordings. Pagination: max 100 results.

Search for musical works (compositions)


## 💬 Prompt Examples

Here are some examples of how you can interact with the **MusicBrainz** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Search for the band Radiohead."

**🤖 AI Agent:**
> Found Radiohead (MBID: a74b1b7f-71a5-4011-9441-d0b5e4122711). Type: Group. Country: United Kingdom. Active: 1985-present. Genres: Alternative rock, electronic, experimental.

---

**👤 You:**
> "Show me all albums by Miles Davis."

**🤖 AI Agent:**
> Found 200+ releases by Miles Davis. Notable albums: 'Kind of Blue' (1959), 'Bitches Brew' (1970), 'Sketches of Spain' (1960), 'Miles Ahead' (1957), 'Birth of the Cool' (1957). Includes official releases, compilations and reissues.

---

**👤 You:**
> "Search for the recording of 'Bohemian Rhapsody' by Queen."

**🤖 AI Agent:**
> Found 'Bohemian Rhapsody' by Queen. Duration: 5:55. ISRC: GBAHK7500018. First released on 'A Night at the Opera' (1975). Multiple versions exist including single edit and remastered versions.


## ❓ FAQ

**Q: Do I need an API key?**
No! MusicBrainz is completely free and open. No authentication required. Just subscribe and start searching. Rate limit is 1 request per second.

**Q: What is an MBID?**
MBID stands for MusicBrainz Identifier — a unique UUID assigned to every entity in the database (artists, releases, recordings, labels, works). Use search tools to find MBIDs, then use get_* tools with the MBID for detailed info.

**Q: What's the difference between a release and a release group?**
A release is a specific physical or digital version of an album (e.g. the 2012 remastered CD). A release group groups all versions of the same album together (e.g. "The Dark Side of the Moon" as a canonical work). Use release groups for finding the canonical album.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/musicbrainz](https://vinkius.com/mcp/musicbrainz)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **MusicBrainz** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `musicbrainz` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **MusicBrainz** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "musicbrainz": {
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
