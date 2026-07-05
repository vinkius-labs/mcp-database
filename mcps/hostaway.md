# Hostaway MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/hostaway)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [ecommerce](../categories/ecommerce.md)

Manage vacation rental listings, reservations, calendar, channels, guest conversations, and financials for your Hostaway properties through natural conversation.

## Description
Connect **Hostaway** to any AI agent — the leading vacation rental channel manager.

### What you can do
- **Listings** — All your properties with details, photos, and amenities
- **Reservations** — Bookings across Airbnb, Booking.com, VRBO, and direct
- **Calendar** — Day-by-day availability, pricing, and min stay
- **Channels** — Sync status across all connected platforms
- **Conversations** — Guest messages from all channels in one place
- **Financials** — Revenue breakdown with commissions and payouts


## Available Tools (8)
- **get_financials**: Get reservation financials
- **list_listings**: List vacation rental listings
- **get_listing**: Get listing details
- **list_reservations**: List reservations
- **get_reservation**: Get reservation details
- **get_calendar**: For revenue management.

Get availability calendar
- **list_channels**: com, VRBO, direct. With sync status.

List connected channels
- **list_conversations**: List guest conversations


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Hostaway** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Show me all reservations arriving this week and their revenue"

**🤖 AI Agent:**
> 🏠 **This Week's Arrivals**

1. 📍 **Beach Villa** — Oct 18-22
   👤 John Smith | 💰 $1,200 | 📱 Airbnb

2. 📍 **Downtown Loft** — Oct 19-21
   👤 Maria García | 💰 $480 | 🌐 Direct

💰 **Total Revenue**: $1,680

---

**👤 You:**
> "List the upcoming check-outs for tomorrow."

**🤖 AI Agent:**
> You have 3 check-outs scheduled for tomorrow: Room 101 (Airbnb), Beach House (Booking.com), and City Apartment (VRBO). I've notified the cleaning staff for turnover.

---

**👤 You:**
> "Update the base price for the Beach Villa to $350 for next month."

**🤖 AI Agent:**
> I have updated the base nightly price for the Beach Villa to $350 for the entire next month across all connected channels (Airbnb, VRBO, Booking.com).


## ❓ FAQ

**Q: What channels does Hostaway support?**
Hostaway connects to 200+ channels including Airbnb, Booking.com, VRBO, Expedia, Google, and TripAdvisor — managing 100,000+ listings worldwide.

**Q: Does Hostaway integrate with my own direct booking website?**
Yes, Hostaway provides a robust engine to manage direct bookings from your own website alongside bookings from major OTAs like Airbnb and Booking.com.

**Q: Can I manage automated guest messaging through this integration?**
Yes, the Hostaway API gives you full access to the unified inbox, allowing the AI to read messages, draft responses, and trigger automated communication workflows for your guests.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/hostaway](https://vinkius.com/mcp/hostaway)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Hostaway** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `hostaway` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Hostaway** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "hostaway": {
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
