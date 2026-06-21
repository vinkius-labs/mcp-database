# Bandsintown MCP Server

Find concerts and live music events — search artists, browse tour dates, discover venues and get ticket links.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/bandsintown)

## Overview
**Category:** audio-music
**Tools Count:** 7

## Description
Connect to **Bandsintown** and discover live music events worldwide through natural conversation — no API key needed.

### What you can do

- **Artist Info** — Get artist profiles with follower counts, images and social links
- **Artist Events** — Browse all upcoming and past tour dates for any artist
- **Recommended Events** — Discover concerts near your city or coordinates
- **Venue Events** — See what shows are coming up at any venue
- **Date Filtering** — Filter events by upcoming, past, or specific date ranges

### How it works

1. Subscribe to this server
2. No API key needed — start searching immediately
3. Discover live music events from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Concert Goers** — find shows by your favorite artists and discover new events near you
- **Music Fans** — track tour dates, browse venue schedules and never miss a live show
- **Event Planners** — research venue lineups and artist touring patterns


## Available Tools
- **get_artist**: Get info for a specific artist
- **get_artist_by_facebook_id**: Get artist info by Facebook page ID
- **get_artist_by_id**: Get artist info by Bandsintown ID
- **get_artist_events**: Use date parameter to filter: "upcoming", "past", "all" or a date range "YYYY-MM-DD,YYYY-MM-DD".

Get upcoming and past events for an artist
- **get_artist_events_by_id**: Same as get_artist_events but uses numeric ID instead of name.

Get events for an artist by Bandsintown ID
- **get_recommended_events**: Filter by city name or latitude/longitude coordinates with radius. Returns event details with artist, venue, date, time and ticket links.

Get recommended events by location
- **get_venue_events**: Returns event details with artists, dates, times and ticket links.

Get upcoming events at a specific venue


## Installation & Usage

To install and use the **Bandsintown** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/bandsintown](https://vinkius.com/mcp/bandsintown)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
