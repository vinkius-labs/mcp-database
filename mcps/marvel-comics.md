# Marvel Comics MCP Server

Explore the Marvel universe — search characters, comics, series, events and creators with full metadata from any AI agent.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/marvel-comics)

## Overview
**Category:** content-management
**Tools Count:** 10

## Description
Connect to the **Marvel Comics API** and explore the entire Marvel universe through natural conversation.

### What you can do

- **Characters** — Search and discover Marvel characters (Spider-Man, Iron Man, X-Men, Avengers) with bios and images
- **Comics** — Find specific comics by title or browse by character, with issue numbers, formats and cover dates
- **Series** — Explore comic series from classic runs to modern limited series with start/end years
- **Events** — Discover major crossover events (Civil War, Secret Wars, Infinity War) with involved comics and characters
- **Creators** — Find writers, artists, editors and colorists who brought Marvel stories to life

### How it works

1. Subscribe to this server
2. Enter your Marvel Public and Private API Keys
3. Start exploring the Marvel universe from Claude, Cursor, or any MCP-compatible client

No more navigating the Marvel website or wikis to find character bios or comic details. Your AI acts as a dedicated Marvel archivist.

### Who is this for?

- **Comic Fans** — discover character backstories, find specific comics and explore major story arcs
- **Collectors** — search for comics by character, series or title to track down specific issues
- **Researchers** — explore Marvel's publication history, creator credits and event timelines


## Available Tools
- **get_character**: Returns the character name, description, thumbnail image URL, comics appearances, series, events and related creators. Use list_characters to find character IDs by name first.

Get a Marvel character by ID
- **get_comic**: Returns the comic title, description, issue number, format, publication date, prices, creators and characters. Use list_comics to find comic IDs first.

Get a Marvel comic by ID
- **get_creator**: ) by their numeric ID. Returns their full name, role, comics worked on, series and events. Use list_creators to find creator IDs by name first.

Get a Marvel creator by ID
- **get_event**: g. "Civil War", "Secret Wars", "Infinity War"). Returns the event title, description, start/end dates, number of comics/series/characters involved and thumbnail.

Get a Marvel event by ID
- **get_series**: Returns the series title, description, start/end years, number of issues, thumbnail and related content.

Get a Marvel series by ID
- **list_characters**: Returns character IDs, names, descriptions and thumbnail images. Useful for discovering character IDs to use with get_character, get_comics (by character) and other tools. Optionally set limit (max 100) and offset for pagination.

Search Marvel characters by name
- **list_comics**: Returns comic titles, issue numbers, formats, publication dates and cover images. Optionally filter by a specific character using their ID. Set limit (max 100) and offset for pagination.

Search Marvel comics by title or character
- **list_creators**: ) by first or last name prefix. Returns creator IDs, full names, thumbnails and their primary roles. Useful for discovering who worked on specific comics. Set limit (max 100) for pagination.

Search Marvel creators by name
- **list_events**: Returns event titles, descriptions, start/end dates and number of involved comics/series. Useful for discovering major story arcs. Set limit (max 100) for pagination.

Search Marvel events by name or character
- **list_series**: Returns series titles, start/end years, issue counts and thumbnails. Useful for finding ongoing series and limited runs. Set limit (max 100) for pagination.

Search Marvel series by title or character


## Installation & Usage

To install and use the **Marvel Comics** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/marvel-comics](https://vinkius.com/mcp/marvel-comics)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
