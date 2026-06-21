# AcoustID MCP Server

Identify songs by audio fingerprint — like Shazam for developers. Search recordings by name, artist or MusicBrainz ID.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/acoustid)

## Overview
**Category:** artificial-intelligence
**Tools Count:** 5

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


## Installation & Usage

To install and use the **AcoustID** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/acoustid](https://vinkius.com/mcp/acoustid)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
