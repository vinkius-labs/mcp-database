# NYC Events & Permits MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/nyc-events-permits)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [events](../categories/events.md)

Keyless NYC events data: upcoming and historical city-permitted events with street-closure flags, event-type rankings, and Parks summer sports & Kids in Motion program sessions — no API key.

## Description
New York City permitted events and park recreation programs, keyless. Built for trip planning — what is on, what is closing streets, where the city runs free summer sports.

### What you can do
- **Upcoming events** — the ~31,000 city-permitted events starting within a forward window (default 90 days, max 365): event name, start/end date-time, permitting agency, event type, borough, location and street closure type; the table carries planned dates into 2027
- **Event type rankings** — the upcoming event types ranked by count, to discover the exact type values
- **Event count** — a fast count of upcoming events in a window, optionally filtered
- **Historical events** — the ~2.9-million permitted events since 2007 in a lookback window (default 90 days, max 365, capped at today)
- **Historical type rankings** — the past event mix by type in a window
- **Summer sports sessions** — Parks Summer Sports & Entertainment (S.S.E) and Kids in Motion (K.I.M.) program sessions with borough, park, date and attendance in a lookback window
- **Top parks / top sports** — the parks and sports with the most sessions in a window

### Who is this for
Visitors and trip planners: the upcoming-events tools answer "what's on this weekend", and the closures_only flag surfaces events that close streets (plan routes around them). Recurring programs ("Sport - Youth", "Sport - Adult") dominate the counts, so filter on the leisure types ("Farmers Market", "Block Party", "Special Event", ...) or use closures_only. Every text filter is an exact match on the stored value; the entertainment agency is stored as "Mayors Office of Media & Entertainment" (straight apostrophe).


## Available Tools (8)
- **count_events**: A single fast count — use it to gauge how large a list_events call will be before fetching rows.

Count upcoming NYC permitted events in a window
- **list_events**: Each row has the event name, start/end date-time, the permitting agency, the event type, the borough (full name, e.g. "Manhattan"), the event location (venue or street range) and the street closure type. The table also carries future planned dates (into 2027). Recurring programs ("Sport - Youth", "Sport - Adult") dominate the counts; for things-to-do look at "Special Event", "Street Event", "Farmers Market", "Block Party", "Religious Event", "Production Event", "Sidewalk Sale" and "Open Street Partner Event". Set closures_only to "true" to return only events that close streets (street_closure_type becomes "Full Street Closure", "Partial Sidewalk Closure" or "Curb Lane Only" instead of "N/A"). Filters are exact matches on stored values: event types and boroughs as listed above; the entertainment agency is stored as "Mayor's Office of Media & Entertainment" (straight apostrophe).

List upcoming NYC permitted events
- **list_summer_sports**: I.M.) program sessions held in a lookback window on session date (days defaults to 90, max 365), most recent first. Each row is one session with its borough, park or playground name, date, the program code ("K.I.M" for Kids in Motion, "S.S.E" for Summer Sports & Entertainment) and the reported attendance. The program runs seasonally (roughly April to mid-July): the 2026 season data ends at 2026-07-17, so a window starting in autumn may return few or no rows. Most sessions leave the sport unspecified (null in the result); filter on sport only with stored values such as "Various Sports", "Basketball", "Soccer", "Flag Football", "Pickleball" or "Tennis".

List summer sports & Kids in Motion sessions
- **search_historical_events**: The historical table holds about 2.9 million events since 2007; a 365-day window holds roughly 190,000 rows and returns in under a second. Row shape and filters are the same as list_events: event type, borough, agency, street closure type, and closures_only for street closures. Historical types include "Parade", "Street Festival", "Plaza Event" and "Theater Load in".

Search historical NYC permitted events
- **top_event_types**: Each row is one event type with the number of events starting in the window. Use it to pick an event type before calling list_events.

Rank upcoming event types by count
- **top_historical_event_types**: Each row is one event type with its count in the window. Use it to compare how the event mix of the last year compares to the upcoming window in top_event_types.

Rank historical event types by count in a window
- **top_summer_sports**: The top row is the unspecified sport — most sessions do not report one — followed by "Various Sports", "Basketball", "Soccer", "Flag Football" and "Pickleball".

Top reported sports in summer sessions
- **top_summer_sports_parks**: Each row is one park or playground name with its session count in the window.

Top parks by summer sports session count


## 💬 Prompt Examples

Here are some examples of how you can interact with the **NYC Events & Permits** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What farmers markets are on in Manhattan this weekend?"

**🤖 AI Agent:**
> list_events with event_type: "Farmers Market", event_borough: "Manhattan" and days: "14" returns the permitted farmers-market sessions starting in the next two weeks, soonest first, with their location and times.

---

**👤 You:**
> "Which events are closing streets in NYC this week?"

**🤖 AI Agent:**
> list_events with days: "7" and closures_only: "true" returns only the events of the week that close streets — street_closure_type comes back as "Full Street Closure", "Partial Sidewalk Closure" or "Curb Lane Only" instead of "N/A"; plan routes around them.

---

**👤 You:**
> "Which parks hosted the most summer sports sessions this season?"

**🤖 AI Agent:**
> top_summer_sports_parks with days: "365" ranks the parks and playgrounds by their Kids in Motion and summer sports session count over the last year; list_summer_sports with that park name then returns the individual sessions with dates and attendance.


## ❓ FAQ

**Q: Do I need an API key?**
No. NYC Open Data serves all public datasets anonymously over its SODA API (data.cityofnewyork.us). This MCP defines no credentials and needs nothing configured.

**Q: Do the text filters ignore case or match partial values?**
No. The NYC data platform only supports exact-match filters, so a filter value must equal the stored value. In this MCP, event types are stored as "Sport - Youth", "Special Event", "Farmers Market", "Block Party", "Street Event", "Parade" and similar; boroughs as full names ("Manhattan", "Staten Island"); the permitting agencies as "Parks Department", "Street Activity Permit Office", "Police Department" and "Mayors Office of Media & Entertainment" (the entertainment agency is stored with a straight apostrophe); street closures as "N/A", "Full Street Closure", "Partial Sidewalk Closure" or "Curb Lane Only". Use top_event_types, or a list tool with no filters, to see the exact stored values before filtering.

**Q: Why do the upcoming-event tools use a forward window?**
The current permitted-events table holds about 31,000 rows and carries future planned dates (into 2027), so list_events and the type rankings scan a forward window from today (default 90 days, max 365). The historical table holds about 2.9 million rows, so its tools scan a lookback window instead (default 90 days, max 365, capped at today). Both windows keep every query under a second.

**Q: Why does list_summer_sports return few or no rows in autumn?**
The Parks summer sports and Kids in Motion programs run seasonally, roughly April to mid-July. The 2026 season data ends at 2026-07-17, so a lookback window starting in autumn holds few or no sessions. Use days: "365" to reach back into the last full season. Most sessions also leave the sport unspecified, so the top_sports ranking starts with an "Unspecified" row.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/nyc-events-permits](https://vinkius.com/en/ai-agent-connect/nyc-events-permits)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **NYC Events & Permits** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `nyc-events-permits` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **NYC Events & Permits** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "nyc-events-permits": {
      "url": "https://edge.vinkius.com/[TOKEN]/mcp"
    }
  }
}
```

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius connector registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
