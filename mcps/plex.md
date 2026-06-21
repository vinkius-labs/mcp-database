# Plex MCP Server

Manage your Plex Media Server — browse libraries, search media, check active streams and control playback from any AI agent.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/plex)

## Overview
**Category:** content-management
**Tools Count:** 15

## Description
Connect to your **Plex Media Server** and manage your entire media library through natural conversation.

### What you can do

- **Server Info** — Check server status, version and connected clients
- **Active Sessions** — See who's watching what right now with playback progress
- **Libraries** — Browse all your media libraries (movies, shows, music, photos)
- **Search** — Find any movie, episode, artist or album by name
- **Recently Added** — Discover the newest additions to your library
- **On Deck** — See what's next to continue watching
- **Metadata** — Get full details on any media item including cast, file info and streams
- **Playlists** — Browse and manage your playlists
- **Watch Status** — Mark items as watched or unwatched

### How it works

1. Subscribe to this server
2. Enter your Plex Token and Server URL
3. Start managing your media library from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Home Media Users** — search your library, check what's playing and find new content to watch
- **Server Admins** — monitor active sessions, manage libraries and check server health
- **Family Managers** — see what family members are watching and manage playlists


## Available Tools
- **get_all_episodes**: Useful for getting the complete episode list for a series.

Get all episodes of a TV show
- **get_children**: For TV shows this returns seasons. For artists this returns albums. Requires the parent item's rating key.

Get children of a media item (seasons or albums)
- **get_libraries**: Each library includes its key (ID), type (movie, show, music, photo), title, agent, scanner and updated/created timestamps. Use the library key with other library tools.

Get all libraries (sections) on the Plex server
- **get_library_content**: Filter by type: type=1 for movies, type=2 for TV shows, type=8 for artists, type=13 for photos. Requires the library key from get_libraries.

Get all content from a specific library
- **get_metadata**: Returns title, summary, year, runtime, rating, genres, director, cast, media streams, file path and more.

Get detailed metadata for a specific item
- **get_on_deck**: Returns the next unwatched episode for each in-progress show.

Get "On Deck" items (continue watching)
- **get_playlist_items**: Returns the items with their titles, types, durations and metadata. Requires the playlist ID.

Get items in a specific playlist
- **get_playlists**: Each playlist includes its ID, title, type (video, audio, photo), item count and duration.

Get all playlists on the Plex server
- **get_recently_added**: Returns movies, episodes and albums with their titles, addition dates and metadata.

Get recently added media to the library
- **get_server_info**: Useful for verifying server connectivity and checking server health.

Get Plex Media Server information
- **get_sessions**: Each session includes the user, the media being watched (movie/episode), playback progress, player device, bandwidth and transcoding info.

Get currently active streaming sessions
- **mark_unwatched**: This resets the item's watch status. Requires the item's rating key.

Mark a media item as unwatched
- **mark_watched**: This affects the item's watch status and removes it from "On Deck". Requires the item's rating key.

Mark a media item as watched
- **refresh_library**: Useful after adding or removing files from your media folders. Requires the library key.

Trigger a library scan/refresh
- **search_library**: Returns matching movies, shows, episodes, artists and albums with their titles, types and metadata.

Search the Plex media library


## Installation & Usage

To install and use the **Plex** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/plex](https://vinkius.com/mcp/plex)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
