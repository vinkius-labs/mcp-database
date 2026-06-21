# CellarPass MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/cellarpass)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/cellarpass-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/cellarpass-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [event-management](../categories/event-management.md)

Manage winery tasting room reservations, experiences, availability, venues, and guest history for your CellarPass account through natural conversation.

## Description
Connect your **CellarPass** tasting room to any AI agent and transform how you manage guest experiences.

### What you can do

- **Reservations** — View today's bookings, upcoming reservations, and guest details by date
- **Experiences** — Browse all tasting experiences: Reserve Tasting, Vineyard Tour, Food & Wine Pairing, Private Cellar
- **Availability** — Check open time slots for any experience on any date
- **Venues** — Manage multiple tasting room locations with hours and capacity
- **Guests** — Search guest profiles: visit history, favorite experiences, spending, and VIP status

### Who is this for?

- **Tasting Room Managers** — "Who's coming today? Any VIPs?" — instant daily briefing
- **Hospitality Directors** — Guest recognition, experience optimization, and capacity planning
- **Winery Owners** — Revenue per guest, popular experiences, and seasonal trends
- **Events Coordinators** — Booking management for private events and corporate tastings


## Available Tools
- **list_reservations**: Filter by date for daily planning. THE core tool for tasting room managers — "Who's coming today?"

List tasting reservations
- **get_reservation**: For pre-visit preparation.

Get reservation details
- **list_experiences**: With pricing, duration, capacity, and description.

List tasting experiences
- **get_experience**: Get experience details
- **check_availability**: Essential for booking coordination.

Check booking availability
- **list_venues**: For multi-location wineries.

List tasting venues
- **get_venue**: Get venue details
- **search_guests**: Returns visit history, favorite experiences, spending, and VIP status. For personalized hospitality.

Search guests


## 💬 Prompt Examples

Here are some examples of how you can interact with the **CellarPass** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What reservations do we have for this Saturday?"

**🤖 AI Agent:**
> 🎟️ **Saturday Reservations — Oct 18, 2025**

📊 **Summary**: 14 reservations | 47 guests | 3 experiences

**Morning**
- 10:00 — **Henderson Party** 👥 6 | Reserve Tasting | ⭐ VIP Club Member
- 10:30 — **Park Family** 👥 4 | Estate Tour
- 11:00 — **Chen Group** 👥 8 | Food & Wine Pairing | 🎂 Birthday
- 11:00 — **Williams** 👥 2 | Reserve Tasting

**Afternoon**
- 1:00 — **Torres Wedding Party** 👥 12 | Private Cellar | 🥂 Special Event
- 1:30 — **Johnson** 👥 2 | Estate Tour
- 2:00 — **Davis** 👥 4 | Reserve Tasting
...

> 💡 3 VIPs today. Henderson party has $47K lifetime spend — consider winemaker greeting.

---

**👤 You:**
> "Open a slot for Vineyard Tour tomorrow at 2PM."

**🤖 AI Agent:**
> Confirmed. I've updated CellarPass directly: there is now 1 open session assigned to Vineyard Tour tomorrow starting at 2:00 PM.

---

**👤 You:**
> "Look up John Doe's past visits and favored pairings."

**🤖 AI Agent:**
> Searching the guest CRM... John Doe visited the Estate three times prior, primarily booking the 'Food & Wine Pairing' events showcasing top-tier local cheddars.


## Installation & Usage

To install and use the **CellarPass** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/cellarpass](https://vinkius.com/mcp/cellarpass)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
