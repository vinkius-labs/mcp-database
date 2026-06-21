# Amenitiz MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/amenitiz)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [ecommerce](../categories/ecommerce.md)

Manage hotel reservations, room types, availability, rates, and guest profiles for your Amenitiz PMS through natural conversation.

## Description
Connect **Amenitiz** to any AI agent — the all-in-one PMS for independent hotels.

### What you can do
- **Reservations** — Browse bookings with guest details, dates, and payment
- **Room Types** — Categories with capacity, amenities, and base rates
- **Rooms** — Individual room status: clean, dirty, occupied
- **Availability** — Day-by-day openings by room type
- **Rates** — Seasonal pricing and promotions
- **Guests** — Guest database with visit history and preferences


## Available Tools
- **list_reservations**: List hotel reservations
- **get_reservation**: Get reservation details
- **list_room_types**: List room types
- **list_rooms**: List individual rooms
- **get_availability**: Get availability
- **get_rates**: Get room rates
- **list_guests**: List guests
- **get_property**: Get hotel property info


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Amenitiz** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What rooms are available for next weekend and at what rates?"

**🤖 AI Agent:**
> 🏨 **Availability — Oct 19-21**

1. 🛏️ **Deluxe Double** — 3/5 available | €149/night
2. 🛏️ **Superior Suite** — 1/2 available | €229/night
3. 🛏️ **Standard Single** — 4/6 available | €89/night

💡 Most popular: Deluxe Double (60% occupancy)


## ❓ FAQ

**Q: What is Amenitiz?**
Amenitiz is an all-in-one PMS for independent hotels — website builder, booking engine, channel manager, and operations management. Popular across Europe with 10,000+ hotels.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/amenitiz](https://vinkius.com/mcp/amenitiz)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Amenitiz** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `amenitiz` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Amenitiz** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "amenitiz": {
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
