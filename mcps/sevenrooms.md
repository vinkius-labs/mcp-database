# SevenRooms MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/sevenrooms)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [event-management](../categories/event-management.md)

Manage restaurant reservations, guest CRM profiles, waitlists, table availability, and events for your SevenRooms venues through natural conversation.

## Description
Connect your **SevenRooms** restaurant to any AI agent — the premium hospitality CRM.

### What you can do
- **Reservations** — Tonight's covers, VIP arrivals, special occasions
- **Guest CRM** — Complete profiles: visit history, spend, preferences, allergies
- **Waitlist** — Real-time queue management with estimated wait times
- **Availability** — Open time slots for any party size and date
- **Events** — Wine dinners, chef tables, private dining
- **Multi-venue** — Cross-restaurant group analytics


## Available Tools
- **list_reservations**: "Who is dining tonight?"

List restaurant reservations
- **get_reservation**: Get reservation details
- **search_guests**: "Tell me about Mr. Silva."

Search guest profiles
- **get_guest**: Get guest profile
- **list_waitlist**: For real-time host management.

List waitlist
- **list_venues**: For multi-location restaurant groups.

List restaurant venues
- **check_availability**: Shows open tables, wait times, and dining room options.

Check table availability
- **list_events**: With date, capacity, pricing, and availability.

List restaurant events


## 💬 Prompt Examples

Here are some examples of how you can interact with the **SevenRooms** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Who are the VIP guests dining tonight and what are their preferences?"

**🤖 AI Agent:**
> 🍷 **Tonight's VIP Guests — Oct 18**

⭐ **James Henderson** — 19:30, party of 4
   💎 Platinum | 23 visits | $18,400 LTV
   🍷 Prefers: Burgundy, booth seating
   ⚠️ Allergy: shellfish
   🎂 Wife's birthday!

⭐ **Dr. Sarah Chen** — 20:00, party of 2
   💎 Gold | 11 visits | $6,200 LTV
   🥩 Prefers: rare steak, bar seating
   📝 Last order: Wagyu A5, Barolo 2018

---

**👤 You:**
> "Check availability for a party of 4 this Friday at 8 PM."

**🤖 AI Agent:**
> 📅 **Availability — Friday 8 PM (Party of 4)**

✅ 19:45 (Dining Room)
✅ 20:00 (Patio)
✅ 20:15 (Bar seating)

Would you like me to book any of these slots?

---

**👤 You:**
> "What events are scheduled for next month?"

**🤖 AI Agent:**
> 🍷 **Upcoming Events (Next Month)**

1. **Wine Dinner Series** | Nov 5, 19:00 | 20 tickets sold, 5 remaining
2. **Chef's Table Experience** | Nov 15, 20:00 | Fully booked
3. **Holiday Private Dining** | Nov 25, 18:00 | Open availability


## ❓ FAQ

**Q: What type of restaurants use SevenRooms?**
SevenRooms is the CRM of choice for premium and fine dining restaurants, hotel F&B outlets, nightclubs, and entertainment venues worldwide. It integrates with 100+ POS and tech partners.

**Q: Is SevenRooms suitable for multi-venue groups?**
Yes, SevenRooms natively supports multi-venue operators, offering cross-restaurant group analytics and unified guest profiles.

**Q: Does it manage waitlists in real-time?**
Yes, SevenRooms provides comprehensive real-time queue management tools with accurate estimated wait times.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/sevenrooms](https://vinkius.com/mcp/sevenrooms)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **SevenRooms** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `sevenrooms` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **SevenRooms** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "sevenrooms": {
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
