# Songkick MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/songkick-alternative)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [audio-music](../categories/audio-music.md)

Find concerts and live music events via Songkick — search artists, venues, and locations to track upcoming performances directly from your AI agent.

## Description
Connect your AI agent to **Songkick**, the world's largest live music database, to discover concerts and track your favorite artists' tours through natural conversation.

### What you can do

- **Event Discovery** — Search for upcoming concerts and festivals by artist name, location, or specific date ranges.
- **Artist Tracking** — Find unique Songkick IDs for artists and retrieve their complete upcoming tour calendars.
- **Venue Insights** — Search for specific music venues and access their full schedule of upcoming performances.
- **Location-Based Search** — Identify metro areas and find live music happening near specific coordinates or cities.
- **Detailed Filtering** — Narrow down results by event type (concert vs. festival) to find exactly what you're looking for.

### How it works

1. Subscribe to this server
2. Enter your Songkick API Key
3. Start discovering live music from Claude, Cursor, or any MCP-compatible client

No more manually checking multiple tour websites. Your AI acts as a personal concert concierge, keeping you updated on every show in your area.

### Who is this for?

- **Music Fans** — instantly find when your favorite bands are playing nearby without leaving your chat interface.
- **Event Planners** — research venue schedules and artist availability for market analysis or trip planning.
- **Travelers** — check what live music is happening in a city you're planning to visit by searching metro area IDs.


## Available Tools
- **get_artist_calendar**: Get the upcoming events for a specific artist
- **search_artists**: Find artists and their unique Songkick IDs
- **search_events**: Search for upcoming events based on criteria
- **search_locations**: Find locations (metro areas) and their unique Songkick IDs
- **search_venues**: Find venues and their unique Songkick IDs
- **get_venue_calendar**: Get the upcoming events for a specific venue


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Songkick** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Search for upcoming Radiohead concerts in London."

**🤖 AI Agent:**
> I've searched for Radiohead events in London. I found an upcoming performance at the O2 Arena on October 15th. Would you like more details on this event?

---

**👤 You:**
> "Find the Songkick ID for the artist 'Daft Punk'."

**🤖 AI Agent:**
> I found the artist 'Daft Punk' with Songkick ID: 549607. You can use this ID to check their full tour calendar.

---

**👤 You:**
> "Get the upcoming events for venue ID 1234."

**🤖 AI Agent:**
> Retrieving the calendar for venue ID 1234... There are 3 upcoming events: 'The Jazz Trio' on Friday, 'Rock Night' on Saturday, and 'Indie Showcase' next Tuesday.


## ❓ FAQ

**Q: How do I find the unique Songkick ID for an artist?**
Use the `search_artists` tool with the artist's name. The agent will return a list of matching artists along with their unique Songkick IDs, which you can then use for calendar lookups.

**Q: Can I see the schedule for a specific concert hall or venue?**
Yes! First, find the venue's ID using `search_venues`. Once you have the ID, use the `get_venue_calendar` tool to retrieve all upcoming events scheduled at that location.

**Q: Is it possible to filter events by date or type?**
Absolutely. The `search_events` tool allows you to specify `min_date`, `max_date`, and `type` (concert or festival) to refine your search results.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/songkick-alternative](https://vinkius.com/mcp/songkick-alternative)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Songkick** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `songkick-alternative` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Songkick** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "songkick-alternative": {
      "url": "https://edge.vinkius.com/[TOKEN]/mcp"
    }
  }
}
```

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
