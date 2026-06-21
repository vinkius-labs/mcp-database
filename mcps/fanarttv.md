# Fanart.tv MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/fanarttv)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/fanarttv-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/fanarttv-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [image-video](../categories/image-video.md)

Get high-quality artwork for movies, TV shows and music — posters, fanart, logos, banners and more.

## Description
Connect to **Fanart.tv** and access the world's largest fan-created artwork database through natural conversation.

### What you can do

- **Movie Art** — Get posters, fanart backgrounds, logos, clear art, disc art and more for any movie
- **TV Show Art** — Retrieve show banners, season posters, season banners, clear logos and show thumbs
- **HD TV Art** — Get high-resolution backgrounds and banners suitable for large displays
- **Music Artist Art** — Find artist thumbs, backgrounds, music logos, banners and concert thumbs
- **Album Art** — Get CD art, album covers, disc backgrounds and spine images for albums
- **Latest Artwork** — Browse recently added artwork for movies, TV shows and music

### How it works

1. Subscribe to this server
2. Enter your Fanart.tv API Key (free registration)
3. Start getting artwork from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Media Centers** — Power Plex, Kodi, Jellyfin and other media center applications with artwork
- **Developers** — integrate high-quality artwork into entertainment applications
- **Designers** — discover fan-created artwork for movies, shows and music artists


## Available Tools
- **get_album_art**: Returns album art including: CD art, album covers, disc backgrounds and spine images.

Get artwork for a music album by MusicBrainz ID
- **get_tv_art_hd**: Returns high-resolution versions of backgrounds and banners suitable for large displays.

Get HD artwork for a TV show by TVDb ID
- **get_latest_movies**: tv. Returns a list of movies with their TMDb IDs and recently added artwork types. Useful for discovering new artwork additions.

Get latest movie artwork added to Fanart.tv
- **get_latest_music**: tv. Returns a list of artists with their MusicBrainz IDs and recently added artwork.

Get latest music artist artwork added to Fanart.tv
- **get_latest_tv**: tv. Returns a list of TV shows with their TVDb IDs and recently added artwork.

Get latest TV show artwork added to Fanart.tv
- **get_movie_art**: Returns movie art including: movie posters, fanart backgrounds, logos, banners, clear art, clear logos, disc art and movie thumbs. Each image includes URL, language, likes count and dimensions.

Get artwork for a movie by TMDb ID
- **get_music_artist_art**: Returns artist art including: artist thumbs, artist backgrounds (fanart), music logos, music banners, artist logos and concert thumbs.

Get artwork for a music artist by MusicBrainz ID
- **get_tv_art**: Returns show art including: show banners, fanart backgrounds, season posters, season banners, clear logos, season thumbs and show thumbs.

Get artwork for a TV show by TVDb ID


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Fanart.tv** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Get artwork for The Matrix (TMDb ID: 603)."

**🤖 AI Agent:**
> Found artwork for The Matrix: 15 movie posters, 12 fanart backgrounds, 8 movie logos, 4 clear art images, 3 disc art images and 5 movie thumbs. All images include direct URLs and language information.

---

**👤 You:**
> "Get artwork for Game of Thrones (TVDb ID: 121361)."

**🤖 AI Agent:**
> Found artwork for Game of Thrones: 8 show banners, 20 fanart backgrounds, 7 season posters (all 8 seasons), 4 clear logos, 28 season thumbs. All images include direct URLs.

---

**👤 You:**
> "Get artwork for The Beatles (MBID: b10bbbfc-cf9e-42e0-be17-e2c3e1d2600d)."

**🤖 AI Agent:**
> Found artwork for The Beatles: 12 artist thumbs, 8 artist backgrounds (fanart), 5 music logos, 3 music banners, 4 artist logos and 2 concert thumbs. All images include direct URLs and like counts.


## Installation & Usage

To install and use the **Fanart.tv** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/fanarttv](https://vinkius.com/mcp/fanarttv)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
