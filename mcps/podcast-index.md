# Podcast Index MCP Server

Access the open podcast ecosystem — search for shows, retrieve episode metadata, and discover trending content directly from your AI agent.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/podcast-index)

## Overview
**Category:** audio-music
**Tools Count:** 16

## Description
Connect to the **Podcast Index** to tap into a massive, independent database of podcasts and episodes. This MCP server allows your AI agent to browse the open podcasting directory without the restrictions of proprietary platforms.

### What you can do

- **Deep Search** — Find podcasts by general terms, specific titles, or even by the people (hosts/guests) featured in them.
- **Metadata Retrieval** — Fetch comprehensive details using RSS feed URLs, Index IDs, Podcast GUIDs, or iTunes IDs.
- **Episode Discovery** — List all episodes for a specific feed or find individual episodes by their unique GUID.
- **Trending & Recent** — Stay updated with recent feeds and episodes, or discover something new with random episode selection.

### How it works

1. Subscribe to this server
2. Enter your Podcast Index API Key and Secret
3. Start exploring the world of podcasts from Claude, Cursor, or any MCP client

### Who is this for?

- **Content Researchers** — quickly find episodes on specific topics or featuring certain guests.
- **Developers** — integrate podcast data into applications without building complex scrapers.
- **Podcast Enthusiasts** — discover new shows and stay updated on the latest releases through natural conversation.


## Available Tools
- **get_episode_by_guid**: Get a specific episode by its GUID
- **get_episodes_by_feed_id**: List episodes for a specific feed ID
- **get_episodes_by_feed_url**: List episodes for a specific feed URL
- **get_podcast_by_feed_id**: Get podcast details using its internal Index ID
- **get_podcast_by_feed_url**: Get podcast details using its RSS feed URL
- **get_podcast_by_guid**: Get podcast details using its Podcast GUID
- **get_podcast_by_itunes_id**: Get podcast details using its iTunes ID
- **get_random_episodes**: Get a selection of random episodes
- **get_recent_episodes**: Get the most recently published episodes
- **get_recent_feeds**: Get the most recently added or updated feeds
- **get_recent_new_feeds**: Get feeds newly added to the index
- **get_value_by_feed_id**: Get the value block by feed ID
- **get_value_by_feed_url**: Get the value block (e.g., Lightning Network details) for a feed URL
- **search_by_person**: Search for podcasts featuring a specific person
- **search_by_term**: Search for podcasts by a general search term
- **search_by_title**: Search for podcasts by title


## Installation & Usage

To install and use the **Podcast Index** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/podcast-index](https://vinkius.com/mcp/podcast-index)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
