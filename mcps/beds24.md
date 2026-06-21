# Beds24 MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/beds24)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [erp-operations](../categories/erp-operations.md)

Manage properties, bookings, rooms, calendar, availability, and pricing for your Beds24 channel manager through natural conversation.

## Description
Connect **Beds24** to any AI agent — the ultra-flexible European channel manager.

### What you can do
- **Properties** — All your properties with rooms and capacity
- **Bookings** — Reservations from all channels with guest details
- **Calendar** — Price, availability, and restrictions by day
- **Availability** — Real-time open/closed status per room
- **Rooms** — Room types, capacity, and channel mappings


## Available Tools (8)
- **list_properties**: List properties
- **get_property**: Get property details
- **list_bookings**: List bookings
- **get_booking**: Get booking details
- **list_rooms**: List rooms for property
- **get_calendar**: Get room calendar
- **get_availability**: Get room availability
- **get_account**: Get account info


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Beds24** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Show me all bookings arriving this week"

**🤖 AI Agent:**
> 🛏️ **This Week's Arrivals**

1. **Ocean View Room** — Oct 18-22 | 👤 Hans Mueller | 💰 €420 | Booking.com
2. **Garden Suite** — Oct 19-21 | 👤 Sophie Dupont | 💰 €280 | Airbnb

---

**👤 You:**
> "Adjust the price for the Ocean View Room to Euro 150 for next weekend."

**🤖 AI Agent:**
> Price adjusted successfully: €150.00 assigned to Ocean View Room covering Friday through Sunday channels.

---

**👤 You:**
> "Generate a brief occupancy report for yesterday."

**🤖 AI Agent:**
> Yesterday closed with 85% occupancy. 6 out of 7 suites were actively checked in, producing a solid €1400 total revenue.


## ❓ FAQ

**Q: What is Beds24?**
Beds24 is a versatile channel manager and PMS popular in Europe. Swagger V2 API, competitive pricing from €15.50/month, connects to all major OTAs.

**Q: Can I automatically adjust nightly availability mapping via chat?**
Yes! The system exposes the availability calendar directly to your AI. Just instruct it to close out specific room types or open dates based on channel rules.

**Q: How quick are the price syncing updates to platforms like Booking.com?**
Changes command via MCP execute instantly against Beds24 API v2. From there, Beds24 dispatches the payload to integrated OTAs (Booking, Airbnb) usually within moments.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/beds24](https://vinkius.com/mcp/beds24)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Beds24** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `beds24` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Beds24** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "beds24": {
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
