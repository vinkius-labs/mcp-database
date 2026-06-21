# Genius MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/genius-alternative)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/genius-alternative-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/genius-alternative-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [knowledge-management](../categories/knowledge-management.md)

Access the world's largest collection of song lyrics and musical knowledge. Search songs, artists, and annotations directly from your AI agent.

## Description
Connect your **Genius** account to any AI agent to explore the world's largest database of song lyrics and crowdsourced musical knowledge.

### What you can do

- **Search & Discovery** — Use `search` to find songs and artists or `lookup_web_page` to find Genius data for any URL.
- **Lyrics & Annotations** — Retrieve deep insights into song meanings with `get_annotation` and `get_referents`.
- **Artist Insights** — Fetch comprehensive artist profiles and their discography using `get_artist` and `get_artist_songs`.
- **Community Interaction** — Upvote, downvote, or create your own annotations using `upvote_annotation`, `downvote_annotation`, and `create_annotation`.
- **Account Management** — Access your own profile details with `get_account`.

### How it works

1. Subscribe to this server
2. Enter your Genius Client Access Token
3. Start exploring musical context from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Music Enthusiasts** — dive deep into the hidden meanings of your favorite tracks without leaving your chat interface.
- **Content Creators** — quickly verify lyrics and artist facts for videos, blogs, or social media.
- **Developers** — integrate musical metadata and annotations into your workflow seamlessly.


## Available Tools
- **create_annotation**: Requires create_annotation scope.

Create a new annotation on a public web page
- **delete_annotation**: Requires manage_annotation scope.

Delete an annotation
- **downvote_annotation**: Requires vote scope.

Downvote an annotation
- **get_account**: Requires me scope.

Get current user account information
- **get_annotation**: Get data for a specific annotation
- **get_artist_songs**: Get songs by a specific artist
- **get_artist**: Get data for a specific artist
- **get_referents**: Get referents (sections of content with annotations)
- **get_song**: Get data for a specific song
- **lookup_web_page**: Lookup a web page on Genius
- **search**: Search all song content hosted on Genius
- **unvote_annotation**: Requires vote scope.

Remove vote from an annotation
- **update_annotation**: Requires manage_annotation scope.

Update an annotation
- **upvote_annotation**: Requires vote scope.

Upvote an annotation


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Genius** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Search for the song 'Bohemian Rhapsody' and give me its ID."

**🤖 AI Agent:**
> I found 'Bohemian Rhapsody' by Queen. The Song ID is 63214. Would you like me to fetch the full details or annotations for this track?

---

**👤 You:**
> "Get all songs by the artist with ID 16775."

**🤖 AI Agent:**
> Fetching songs for Artist ID 16775 (Kendrick Lamar)... I've found tracks like 'HUMBLE.', 'DNA.', and 'Alright'. Would you like to see the full list or details for a specific song?

---

**👤 You:**
> "What does the annotation with ID 1034 say?"

**🤖 AI Agent:**
> Annotation 1034 explains the historical context of the opening verse, noting that the artist is referencing a specific event from 1969. It has 45 upvotes.


## Installation & Usage

To install and use the **Genius** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/genius-alternative](https://vinkius.com/mcp/genius-alternative)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
