# AcoustID MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/acoustid)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/acoustid-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/acoustid-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [artificial-intelligence](../categories/artificial-intelligence.md)

Identify songs by audio fingerprint — like Shazam for developers. Search recordings by name, artist or MusicBrainz ID.

## Description
Connect to **AcoustID** and identify music from audio fingerprints through natural conversation — no API key needed for basic use.

### What you can do

- **Song Identification** — Identify songs from audio fingerprints (like Shazam)
- **Recording Search** — Search for recordings by name, artist or MusicBrainz ID
- **MBID Lookup** — Find all AcoustIDs linked to a MusicBrainz recording
- **Metadata Lookup** — Get full metadata for recordings including artists and release groups
- **Fingerprint Submission** — Submit new audio fingerprints to expand the database

### How it works

1. Subscribe to this server
2. No API key needed for basic lookups
3. Start identifying songs from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Music Apps** — integrate song identification into audio players and streaming services
- **Researchers** — analyze audio fingerprints and MusicBrainz recording data
- **Music Enthusiasts** — identify unknown songs and explore recording metadata


## Available Tools
- **get_recording_metadata**: Returns all associated MusicBrainz recordings, artists, release groups and fingerprints linked to this AcoustID.

Get full metadata for a recording by AcoustID
- **lookup_by_fingerprint**: Returns matching recordings from the AcoustID database with song titles, artists, MusicBrainz IDs and match confidence scores. Requires the fingerprint string and audio duration in seconds. Use meta="recordings" for full recording details.

Identify a song by audio fingerprint
- **search_by_mbid**: Returns all AcoustID fingerprints linked to that MusicBrainz recording, useful for finding multiple audio fingerprints of the same song.

Search for AcoustIDs by MusicBrainz ID
- **search_by_recording**: Returns matching recordings with AcoustID, MusicBrainz ID, title and artist name. Useful for finding the AcoustID of a known song.

Search for recordings by name and/or artist
- **submit_fingerprint**: Requires the Chromaprint fingerprint string and audio duration. Optionally include recording name and artist for new songs. Returns the newly created AcoustID.

Submit an audio fingerprint to AcoustID


## 💬 Prompt Examples

Here are some examples of how you can interact with the **AcoustID** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Search for 'Bohemian Rhapsody' by Queen."

**🤖 AI Agent:**
> Found Bohemian Rhapsody by Queen. AcoustID: 0e5e5b5e-... MusicBrainz ID: b1a9c0e9-... Multiple fingerprints available for this recording.

---

**👤 You:**
> "Search recordings by Daft Punk."

**🤖 AI Agent:**
> Found multiple Daft Punk recordings: Get Lucky (95% match), One More Time (92% match), Around the World (89% match), Harder Better Faster Stronger (88% match). Each with AcoustID and MusicBrainz ID.

---

**👤 You:**
> "Get metadata for AcoustID 0e5e5b5e-."

**🤖 AI Agent:**
> AcoustID 0e5e5b5e-: Bohemian Rhapsody — Queen. Linked to MusicBrainz ID: b1a9c0e9-... from album 'A Night at the Opera' (1975). Multiple fingerprints associated with this recording.


## Installation & Usage

To install and use the **AcoustID** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/acoustid](https://vinkius.com/mcp/acoustid)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
