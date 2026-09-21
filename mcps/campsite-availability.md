# Campsite Availability MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/campsite-availability)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [travel](../categories/travel.md)

Real campsite availability from Recreation.gov — which nights are open at a campground, which sites fit a multi-night stay, and how campgrounds compare side by side.

## Description
Connects an AI agent to the campsite inventory of Recreation.gov, the reservation system of the US national parks and forests, and reads the same availability data the booking pages show.

### What you can do

- **Find a campground** — search by name or park, and get the numeric facility id every other tool needs
- **Read a campground** — description, facilities, fees, stay limits, directions, accessibility notes and contact
- **See a month** — for every arrival date, how many sites are open, reserved or closed, plus a breakdown by site type
- **Fit a stay** — the sites that are free for every night of a multi-night stay, even when the stay crosses a month boundary
- **Find the dates** — which arrival dates in a month have a site free for the whole stay, and how many
- **Compare** — several campgrounds side by side for one month

### Why this is the useful layer

A campground listing tells you a place exists; it does not tell you whether you can book it. Recreation.gov publishes availability per campsite and per arrival date, and an agent needs that grid aggregated before it can answer "where can we sleep next weekend". This server does the aggregation: a stay of N nights is a site that is Available on each of its N nights, so a partially-blocked site is excluded rather than reported as open.

Two properties of the source shape every answer. Availability is published one month at a time, always from the 1st, and reservations are released on a rolling basis roughly five months ahead, so a far-future month can legitimately come back empty. And the site mixes campgrounds with tours, permits and timed-entry listings; only campgrounds are kept, which is why a page can hold fewer rows than requested.


## Available Tools (6)
- **compare_campgrounds**: Give up to eight campground ids separated by commas and a month like "2026-07"; each row reports the site count, how many days hold at least one open site, the date with the most open sites and the first open arrival. A campground that errors is reported in its own row with the reason instead of failing the comparison, so a bad id does not lose the rest. Use this after search_campgrounds has given the ids, and before drilling into one campground with get_monthly_availability.

Campsite availability of several campgrounds side by side for one month — which one has open sites, how many, and on which dates
- **find_available_dates**: Give the campground id, a month like "2026-11" and the length of stay; the answer lists every arrival date in the month where at least one site is Available for all consecutive nights of the stay, with how many sites qualify on each date. A one-night stay reports the same nights as the open columns of the month table; longer stays are stricter, so a month with plenty of single nights open can still have no three-night window. An empty list means the month is before the release window, closed for the season, or fully booked — check get_monthly_availability to tell which, because it reports reserved and closed days rather than just open ones.

Which arrival dates in a month have a site free for a whole stay — the calendar view of when a campground can actually be booked
- **get_campground**: Holds the description, facilities, natural features, nearby attractions, accessibility notes, fees, stay limit, cancellation policy, contact phone and directions. This is the descriptive record only — it says nothing about whether a site is free on a given night, so pair it with get_monthly_availability or find_available_sites for that.

The full record of one Recreation.gov campground — what it has, what it costs, how to get there and the rules that apply
- **get_monthly_availability**: Give the campground id and a month like "2026-11"; the month is normalised to its first day, which the API requires. The answer is an aggregation over the per-site grid the site publishes: one row per arrival date with open, reserved, closed and other counts, a breakdown by campsite type, and a paginated site list where each site carries the longest run of open nights it has that month — the number to look at when a stay needs more than one night. A campground with no published inventory for the month says so: it may be first-come-first-served, closed for the season, or before the release window (Recreation.gov opens reservations on a rolling basis, roughly five months out, so a far-future month can legitimately be empty). Page the site list with offset; the day table always covers the whole month.

Campsite availability for one campground across a whole month — how many sites are open, reserved or closed on each arrival date, and which sites are free at all
- **search_campgrounds**: Search a park or campground name — "Upper Pines", "Yellowstone", "Joshua Tree" — and matching is on the name as Recreation.gov holds it, so a fragment is enough. The list also contains tours, permits and timed-entry listings, which this tool drops: only campgrounds come back, which is why a page can hold fewer rows than you asked for. Page through results by advancing offset by page_size, not by the number of rows returned. Optional state is a two-letter code and is matched here, not by the site, so with a state filter each page holds fewer rows still. Rows carry the campground id to hand to get_campground, get_monthly_availability and find_available_sites.

Find campgrounds on Recreation.gov by name — the campground inventory of the US national parks and forests, with the facility id every other tool needs
- **find_available_sites**: Give the campground id, an arrival date like "2026-11-20" and the number of nights; a site is returned only when it is Available on every night of the stay, because a booking needs one site free for all of them. A stay that crosses a month boundary is handled by fetching both months, so a "2026-11-28" arrival for three nights works even though it ends in December. Each site carries its number, loop, type and sleeping capacity. An empty answer means every site is blocked on at least one night — shorten the stay, move the arrival, or use find_available_dates to see which arrivals in the month do work. Nights cap at 14.

The campsites at one campground that are free for an entire stay — every night from the arrival date through the departure


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Campsite Availability** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "We want to camp in Yosemite in late January, three nights, arriving January 30. Which campgrounds have a site free for the whole stay, and what do they cost?"

**🤖 AI Agent:**
> Upper Pines Campground (id 232447) has 66 sites free for all three nights — the stay crosses into February, and both months are fetched so the boundary is handled. Sites 001, 002 and 006 in the Upper Pines loop are typical matches: standard non-electric, sleep six, about $36 a night. North Pines (232449) publishes nothing for January because it is first-come-first-served that month, and Lower Pines is closed for the season — the comparison reports both rather than listing them as fully booked.

---

**👤 You:**
> "I can be flexible. For Upper Pines in January, which arrival dates would let me stay four nights?"

**🤖 AI Agent:**
> 26 of the 31 days in January have at least one site free for four consecutive nights. The best arrivals are around January 18-20 and 24-27, where 70 to 84 sites are open for the whole stay; January 16 has none, and January 15 has only three, so the month is not uniformly bookable even with plenty of single nights free.

---

**👤 You:**
> "Compare three campgrounds near Yellowstone for July — which one has the most open sites?"

**🤖 AI Agent:**
> Madison (232451) has the widest open window with 28 of 31 days holding at least one free site and a best day of 74 open sites, Tower Fall (259308) is fully booked for the month — 31 sites, zero open days — and Lewis Lake (259309) has 12 open days peaking at 40 sites. Each row is fetched independently, so one campground that errors does not lose the others.


## ❓ FAQ

**Q: Do I need an API key or a Recreation.gov account?**
No. The server reads the same public availability data the Recreation.gov website loads, without authentication. Booking still happens on Recreation.gov itself — this server answers what is open, it does not hold or modify a reservation.

**Q: Why does a month come back empty even though the campground exists?**
Two common reasons. Recreation.gov releases reservations on a rolling schedule — roughly five months ahead, often on the 15th of the month — so a month beyond that window has no published inventory yet. Or the campground is first-come-first-served, or closed for the season, in which case there is simply nothing to reserve. The response says which of these it is rather than reporting zero sites as if the campground were gone.

**Q: A site is open on most nights of my stay — why is it not listed?**
Because a booking needs one site free on every night of the stay, not several sites free across it. A site blocked on a single night cannot host the booking, so it is excluded. Use find_available_dates instead to see which arrival dates do work for the length of stay you want.

**Q: Why do I get fewer campgrounds than the amount I asked for?**
Recreation.gov returns campgrounds, tours, permits and timed-entry listings in one mixed list, and its server-side filters are not reliable. This server keeps only campgrounds, so rows of other kinds are dropped and a page can hold fewer than requested. Advance the offset by the page size, not by the rows you received, to page through correctly.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/campsite-availability](https://vinkius.com/en/ai-agent-connect/campsite-availability)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Campsite Availability** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `campsite-availability` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Campsite Availability** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "campsite-availability": {
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
