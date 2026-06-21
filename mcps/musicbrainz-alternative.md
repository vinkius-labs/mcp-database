# MusicBrainz MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/musicbrainz-alternative)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/musicbrainz-alternative-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/musicbrainz-alternative-mcp)
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


## Available Tools
- **add_collection_items**: Add items to a collection (Requires Auth)
- **browse_entities**: g., all releases for an artist).

Browse entities linked to another entity
- **lookup_discid**: Lookup a CD by its discid
- **lookup_isrc**: Lookup recordings by ISRC
- **lookup_iswc**: Lookup works by ISWC
- **lookup_entity**: Lookup a specific MusicBrainz entity by its MBID
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


## Installation & Usage

To install and use the **MusicBrainz** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/musicbrainz-alternative](https://vinkius.com/mcp/musicbrainz-alternative)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
