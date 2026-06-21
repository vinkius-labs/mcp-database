# CellarPass MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/cellarpass)
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


## Available Tools (8)
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


## ❓ FAQ

**Q: How many wineries use CellarPass?**
CellarPass serves 800+ wineries across Napa Valley, Sonoma, Oregon, Washington, and other premier wine regions. It's the #1 tasting room reservation platform.

**Q: Can I flag or review VIP guest history using this integration?**
Yes! Your AI can pull visitor profiles and tag high-revenue VIPs, highlighting lifetime spend seamlessly when generating your daily prep reviews.

**Q: Does it manage multiple tasting room venues?**
Correct. With 'Venues' configuration endpoints natively wired, the AI can cross-reference capacities against your separate tasting properties in a single conversational flow.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/cellarpass](https://vinkius.com/mcp/cellarpass)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **CellarPass** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `cellarpass` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **CellarPass** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "cellarpass": {
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
