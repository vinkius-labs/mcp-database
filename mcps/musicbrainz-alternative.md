# MusicBrainz MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/musicbrainz-alternative)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [databases](../categories/databases.md)

Access the world's largest open music encyclopedia — search artists, lookup releases, and manage your music collections directly from your AI agent.

## Description
Connect to the **MusicBrainz** database to empower your AI agent with comprehensive music metadata. From identifying obscure recordings to browsing entire artist discographies, this server provides deep access to the world's most detailed music knowledge base.

### What you can do

- **Entity Lookup** — Retrieve detailed metadata for artists, releases, recordings, labels, and more using unique MusicBrainz Identifiers (MBIDs).
- **Advanced Search** — Use Lucene query syntax to find exactly what you're looking for across millions of musical entities.
- **Linked Data Browsing** — Discover relationships between entities, such as listing all releases for a specific artist or all recordings on a label.
- **Standard Identifiers** — Lookup music using industry standards like ISRC (recordings), ISWC (works), and DiscIDs (CDs).
- **Collection Management** — Authenticated users can submit tags, ratings, and manage their personal music collections directly through the agent.

### How it works

1. Subscribe to this server
2. Provide a User Agent string (required by MusicBrainz API policy)
3. (Optional) Provide your MusicBrainz Access Token for write operations
4. Start exploring the global music encyclopedia from your favorite MCP client

### Who is this for?

- **Music Researchers & Journalists** — instantly verify release dates, artist credits, and historical metadata.
- **Developers & Data Scientists** — query structured music data for applications or analysis without manual scraping.
- **Music Enthusiasts** — organize personal collections and discover new music through deep metadata exploration.


## Available Tools (10)
- **browse_entities**: g., all releases for an artist).

Browse entities linked to another entity
- **lookup_discid**: Lookup a CD by its discid
- **lookup_isrc**: Lookup recordings by ISRC
- **lookup_iswc**: Lookup works by ISWC
- **lookup_entity**: Lookup a specific MusicBrainz entity by its MBID
- **add_collection_items**: Add items to a collection (Requires Auth)
- **remove_collection_item**: Remove an item from a collection (Requires Auth)
- **search_entities**: Use Lucene syntax (e.g., "we will rock you" AND arid:0383dadf-2a4e-4d10-a46a-e9e041da8eb3).

Search for entities using Lucene query syntax
- **submit_ratings**: Submit ratings via XML POST (Requires Auth)
- **submit_tags**: Submit tags via XML POST (Requires Auth)


## 💬 Prompt Examples

Here are some examples of how you can interact with the **MusicBrainz** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Search for the artist 'Daft Punk' and give me their MBID."

**🤖 AI Agent:**
> I found Daft Punk. Their MusicBrainz Identifier (MBID) is `65f4f0c5-ef9e-490c-aee3-909e7ae6b2ab`. They are an electronic music duo from Paris, France.

---

**👤 You:**
> "List all releases for the artist with MBID 0383dadf-2a4e-4d10-a46a-e9e041da8eb3."

**🤖 AI Agent:**
> Browsing releases for Queen (MBID: 0383dadf-2a4e-4d10-a46a-e9e041da8eb3)... I've found several releases including 'A Night at the Opera', 'News of the World', and 'The Game'. Would you like details on a specific one?

---

**👤 You:**
> "Lookup the recording details for ISRC USRC10301589."

**🤖 AI Agent:**
> The ISRC USRC10301589 corresponds to the recording 'Seven Nation Army' by The White Stripes. It appears on the album 'Elephant' and has a duration of approximately 3:51.


## ❓ FAQ

**Q: How do I search for a specific artist if I don't have their MBID?**
Use the `search_entities` tool. Set the `entity_type` to 'artist' and provide the name in the `query` field. The agent will return a list of matches with their respective MBIDs.

**Q: Can I see all the recordings (songs) on a specific album?**
Yes! Use the `lookup_entity` tool with the release MBID and include 'recordings' in the `inc` parameter. This will fetch the full tracklist and metadata for that release.

**Q: Do I need an account to search the database?**
No. Searching and looking up data only requires a `MUSICBRAINZ_USER_AGENT`. An Access Token is only needed for actions like `submit_tags`, `submit_ratings`, or `add_collection_items`.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/musicbrainz-alternative](https://vinkius.com/mcp/musicbrainz-alternative)
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
3. Set Type to "SSE" (or "streamable HTTP"), enter `musicbrainz-alternative` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **MusicBrainz** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "musicbrainz-alternative": {
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
