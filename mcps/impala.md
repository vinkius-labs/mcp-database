# Impala MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/impala)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [ecommerce](../categories/ecommerce.md)

Search hotels, check availability, compare rates, and browse reviews through a unified global hotel data platform via natural conversation.

## Description
Connect **Impala** to any AI agent — the Stripe of hotel booking.

### What you can do
- **Search** — Find hotels by city, coordinates, or destination
- **Availability** — Real-time room availability for any dates
- **Rates** — Compare prices across room types with cancellation policies
- **Reviews** — Guest reviews and ratings
- **Photos** — Property and room photography


## Available Tools (8)
- **search_hotels**: "Find hotels near the Eiffel Tower."

Search hotels near coordinates
- **get_hotel**: Get hotel details
- **get_room_types**: Get hotel room types
- **check_availability**: Check hotel availability
- **get_rates**: Get hotel rates
- **get_reviews**: For reputation management.

Get hotel reviews
- **get_photos**: Get hotel photos
- **search_hotels_by_city**: "Show hotels in Barcelona."

Search hotels by city


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Impala** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Find 5-star hotels in Barcelona for next weekend"

**🤖 AI Agent:**
> 🏨 **5-Star Hotels in Barcelona**

1. ⭐⭐⭐⭐⭐ **Hotel Arts Barcelona**
   📍 Passeig Marítim | 💰 €320/night | 🛏️ Sea View Suite

2. ⭐⭐⭐⭐⭐ **W Barcelona**
   📍 Barceloneta | 💰 €285/night | 🛏️ Fabulous Room

---

**👤 You:**
> "Check room availability at the W Barcelona for tonight."

**🤖 AI Agent:**
> The W Barcelona currently has 4 rooms available for tonight: 2 'Fabulous Rooms' starting at €350/night, and 2 'Spectacular Rooms' starting at €420/night. Both include free cancellation until 6 PM.

---

**👤 You:**
> "Find hotels in central Tokyo with a minimum rating of 4.5."

**🤖 AI Agent:**
> I found 8 hotels in central Tokyo matching your criteria. Top suggestions include The Ritz-Carlton Tokyo (4.8/5) and the Palace Hotel Tokyo (4.7/5). Would you like to check their current rates?


## ❓ FAQ

**Q: What is Impala?**
Impala is a unified hotel data platform — the 'Stripe for hotels.' One API to search, compare, and book hotels worldwide.

**Q: Does Impala provide real-time availability and pricing?**
Yes, Impala connects directly to property management systems (PMS) to provide real-time room availability, up-to-date dynamic pricing, and exact cancellation policies.

**Q: Is test data available for developers without making real bookings?**
Yes, Impala provides a Sandbox environment with realistic test data, allowing developers to safely test search, availability updates, and simulated booking flows.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/impala](https://vinkius.com/mcp/impala)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Impala** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `impala` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Impala** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "impala": {
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
