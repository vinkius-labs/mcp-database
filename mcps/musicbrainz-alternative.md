# MusicBrainz MCP Server

Access the world's largest open music encyclopedia — search artists, lookup releases, and manage your music collections directly from your AI agent.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/musicbrainz-alternative)

## Overview
**Category:** databases
**Tools Count:** 10

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


## Installation & Usage

To install and use the **MusicBrainz** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/musicbrainz-alternative](https://vinkius.com/mcp/musicbrainz-alternative)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
