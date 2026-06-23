# Songkick MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/songkick)
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


## Available Tools (8)
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


## ❓ FAQ

**Q: How do I find upcoming concerts in a specific city?**
First, use the `search_locations` tool to find the correct `metroAreaId` for your city. Then, use the `get_location_calendar` tool with that ID to retrieve all upcoming events in that area.

**Q: Can I see the full tour history of an artist?**
Yes! Use the `get_artist_gigography` tool with the Artist ID. It provides a comprehensive list of past concerts and events recorded for that specific artist.

**Q: Does the integration provide details for specific concert venues?**
Absolutely. You can use the `search_venues` tool to find a venue by name and then use `get_venue_calendar` to see all upcoming shows scheduled at that specific location.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/songkick](https://vinkius.com/mcp/songkick)
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
3. Set Type to "SSE" (or "streamable HTTP"), enter `songkick` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Songkick** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "songkick": {
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
