# Bandsintown MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/bandsintown)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [audio-music](../categories/audio-music.md)

Find concerts and live music events — search artists, browse tour dates, discover venues and get ticket links.

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


## Available Tools (7)
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


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Bandsintown** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What concerts are coming up for Taylor Swift?"

**🤖 AI Agent:**
> Taylor Swift has 15 upcoming tour dates. Next shows: São Paulo (Allianz Parque, Dec 15), Buenos Aires (River Plate, Dec 20), London (Wembley, Jun 2025). All dates include venue info and ticket links.

---

**👤 You:**
> "Find recommended concerts in New York."

**🤖 AI Agent:**
> Found 25+ recommended events in New York: 1. The Strokes at Madison Square Garden (Dec 18) — 2. Billie Eilish at Barclays Center (Dec 22) — 3. Radiohead at Forest Hills Stadium (Jul 2025). All with venue details and ticket links.

---

**👤 You:**
> "What shows are happening at Red Rocks Amphitheatre?"

**🤖 AI Agent:**
> Red Rocks Amphitheatre has 40+ upcoming shows. Notable acts: Zach Bryan (Jun 15), Tyler the Creator (Jul 22), Dead & Company (Aug 10), Widespread Panic (Sep 5-7). The iconic outdoor venue near Denver hosts concerts from May through October.


## ❓ FAQ

**Q: Do I need an API key?**
No! Bandsintown's public API works without authentication using a default app_id. Just subscribe and start searching for concerts.

**Q: Can I find concerts near me?**
Yes! Use get_recommended_events with a city name (e.g. 'New York', 'London') or latitude/longitude coordinates. You can also set a search radius in miles.

**Q: Can I see past tour dates?**
Yes! Use get_artist_events with the date parameter set to 'past' to see completed shows, or 'all' to see both upcoming and past events.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/bandsintown](https://vinkius.com/mcp/bandsintown)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Bandsintown** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `bandsintown` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Bandsintown** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "bandsintown": {
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
