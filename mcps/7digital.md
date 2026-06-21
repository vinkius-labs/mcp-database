# 7digital MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/7digital)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/7digital-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/7digital-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [audio-music](../categories/audio-music.md)

Search music catalog — find artists, albums, tracks with previews and purchase options worldwide.

## Description
Connect to **7digital** and access a global music catalog through natural conversation.

### What you can do

- **Artist Search** — Search for artists by name with release counts and profile info
- **Artist Details** — Get artist profiles with images, similar artists and discographies
- **Artist Releases** — Browse all albums, singles and EPs by an artist
- **Release Search** — Search albums and releases by title or artist
- **Release Details** — Get full release info including label, genre, release date and track list
- **Release Tracks** — Get the full track listing for any album
- **Track Search** — Search for individual tracks by title or artist
- **Track Previews** — Get 30-second preview streaming URLs for any track
- **Shopping Basket** — Manage your 7digital shopping basket (add items, checkout)

### How it works

1. Subscribe to this server
2. Enter your 7digital API Key (free at 7digital.com/developer)
3. Start exploring the music catalog from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Music Fans** — discover new artists, browse albums and listen to track previews
- **Developers** — integrate music catalog data, previews and purchasing into apps
- **Retailers** — access global music catalog with pricing and checkout integration


## Available Tools
- **get_track_preview**: Returns the preview URL, content type (audio/mpeg) and duration. Use the track ID from search_track or get_release_tracks results.

Get a preview/stream URL for a specific track
- **add_to_basket**: Returns the updated basket contents with prices. Use the release ID from search_release results.

Add a release to your 7digital shopping basket
- **get_artist_details**: Use the artist ID from search_artist results.

Get detailed info for a specific artist
- **get_artist_releases**: Returns album/singles titles, release dates, types (Album, Single, EP, Compilation) and 7digital URLs. Use the artist ID from search_artist.

Get all releases (albums/singles) by an artist
- **get_basket**: Returns release titles, prices and quantities. Requires an active 7digital developer account with basket access.

View items currently in your 7digital shopping basket
- **get_checkout_url**: Returns the URL where users can complete their purchase. Optional returnUrl parameter for redirecting after purchase.

Get a checkout URL for your current basket
- **get_release_details**: Use the release ID from search_release or get_artist_releases results.

Get detailed info for a specific album release
- **get_release_tracks**: Returns track titles, artists, durations, track numbers and explicit content flags. Use the release ID from search_release or get_release_details.

Get all tracks from a specific album release
- **search_artist**: Returns artist names, number of releases and 7digital URLs. Use country code (e.g. "US", "GB", "DE") for region-specific results.

Search for music artists by name
- **search_release**: Returns release titles, artists, release dates, types and 7digital URLs.

Search for album releases by title or artist
- **search_track**: Returns track titles, artists, durations, release info and explicit content flags.

Search for individual tracks by title or artist


## 💬 Prompt Examples

Here are some examples of how you can interact with the **7digital** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Search for Radiohead albums."

**🤖 AI Agent:**
> Found 12 Radiohead releases: OK Computer (1997), Kid A (2000), In Rainbows (2007), The Bends (1995), A Moon Shaped Pool (2016) and more. Each with track lists, genres and purchase links.

---

**👤 You:**
> "Get the track listing for OK Computer."

**🤖 AI Agent:**
> OK Computer (1997) — 12 tracks: 1. Airbag (4:44) 2. Paranoid Android (6:23) 3. Subterranean Homesick Alien (4:27) 4. Exit Music (For a Film) (4:24) 5. Let Down (4:59) 6. Karma Police (4:21) 7. No Surprises (3:48) 8. Lucky (4:19) 9. The Tourist (5:24) and more.

---

**👤 You:**
> "Play a preview of Paranoid Android."

**🤖 AI Agent:**
> Preview URL: https://preview.7digital.com/clip/xxxxx.mp3 (30s preview, audio/mpeg). Duration: 6:23.


## Installation & Usage

To install and use the **7digital** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/7digital](https://vinkius.com/mcp/7digital)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
