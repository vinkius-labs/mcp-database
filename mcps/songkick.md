# Songkick MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/songkick)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/songkick-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/songkick-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [data-management](../categories/data-management.md)

Global live music database — search concerts, artists, and venues via AI.

## Description
Equip your AI agent with the most comprehensive live music intelligence available via **Songkick**. This unified server provides your agent with instant access to worldwide concert schedules, artist tour dates, and venue calendars. Your agent can instantly search for upcoming shows in specific cities, audit an artist's full gigography, and retrieve detailed event information without you ever needing to browse a ticketing site. Whether you are planning a night out or auditing the tour history of a specific band, your agent acts as a dedicated concert coordinator through natural conversation.

### What you can do

- **Concert Discovery** — Search for thousands of upcoming concerts and festivals by artist, location, or venue.
- **Artist Gigography** — Fetch complete tour histories and past events for any artist in the database.
- **Location Intelligence** — Retrieve upcoming events for specific metro areas to plan your local entertainment.
- **Venue Calendars** — Access the schedule of shows for specific concert venues worldwide.
- **Event Auditing** — Retrieve detailed metadata for specific events, including lineups and start dates.

### How it works

1. Subscribe to this server
2. Enter your Songkick API Key
3. Start managing your live music intelligence from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Live Music Fans** — instantly find when their favorite artists are playing nearby through natural language.
- **Tour Managers & Agents** — audit the gigography and upcoming schedules of artists for competitive analysis.
- **Event Organizers** — monitor venue calendars and local event densities for organizational planning.
- **Travelers** — quickly find concerts and festivals happening in their destination cities.
- **Developers** — integrate real-time concert data into their applications through an AI-guided interface.


## Available Tools
- **get_artist_calendar**: Get artist upcoming events
- **get_artist_gigography**: Get artist past events
- **get_event_details**: Get detailed event info
- **get_location_calendar**: Get events in a location
- **search_artists**: Search for artists
- **search_locations**: Search for locations
- **search_venues**: Search for venues
- **get_venue_calendar**: Get events at a venue


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Songkick** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Is 'Coldplay' on tour right now?"

**🤖 AI Agent:**
> Searching for Coldplay... Yes, they are currently on tour! I see upcoming shows in London, Paris, and Berlin. Would you like the specific dates and venue information?

---

**👤 You:**
> "Show me concerts in New York City next week."

**🤖 AI Agent:**
> Retrieving the NYC concert calendar... There are several exciting events, including 'The Killers' at Madison Square Garden and various indie bands at local clubs. Shall I list them by date for you?

---

**👤 You:**
> "Get the gigography for 'Radiohead'."

**🤖 AI Agent:**
> Fetching Radiohead's history... I've identified hundreds of past events spanning from their early club dates to major festival headlining slots. I can break this down by year or country if you're interested.


## Installation & Usage

To install and use the **Songkick** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/songkick](https://vinkius.com/mcp/songkick)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
