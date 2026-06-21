# ClassPass MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/classpass)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [ecommerce](../categories/ecommerce.md)

Manage your ClassPass schedule, reservations, inventory, and performance analytics for your fitness venue through natural conversation.

## Description
Connect your **ClassPass** venue to any AI agent and manage your marketplace presence through natural conversation.

### What you can do

- **Schedule** — View classes published to ClassPass with credit pricing and availability
- **Reservations** — Track ClassPass bookings, check-ins, and no-shows
- **Inventory** — Manage SmartSpot allocation and dynamic credit pricing
- **Performance** — Analyze revenue, fill rates, and partner metrics
- **Venue** — Access your venue profile, amenities, and ratings
- **Locations** — Manage multiple physical locations

### Who is this for?

- **Studio Partners** — Optimize ClassPass revenue and SmartSpot settings
- **Operations** — Track daily ClassPass bookings alongside direct reservations
- **Marketing** — Monitor venue ratings, reviews, and marketplace visibility
- **Multi-location** — Compare ClassPass performance across all locations


## Available Tools
- **list_schedule**: Filter by date range.

List ClassPass schedule
- **get_class_detail**: Get class details
- **list_reservations**: List ClassPass reservations
- **get_venue_info**: Get venue profile
- **list_locations**: List venue locations
- **get_performance**: Use date range for period analysis.

Get performance analytics
- **list_inventory**: List SmartSpot inventory


## 💬 Prompt Examples

Here are some examples of how you can interact with the **ClassPass** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "How is our ClassPass performance this month?"

**🤖 AI Agent:**
> ClassPass performance — March 2026:

💰 **Revenue**: $3,240 (+18% vs Feb)
📊 **Reservations**: 312 bookings
✅ **Check-in rate**: 87%
🎫 **Avg credits/class**: 7.2
📈 **Fill rate contribution**: ClassPass fills 15% of your total capacity

Your 6 PM HIIT class is your #1 ClassPass performer with 48 bookings this month.

---

**👤 You:**
> "Check total no-shows for yesterday's 6 PM HIIT class."

**🤖 AI Agent:**
> Yesterday's 6 PM HIIT class had exactly 3 no-shows from ClassPass members out of the 15 total external bookings.

---

**👤 You:**
> "Increase the credit pricing for tomorrow's Pilates session to 8 credits."

**🤖 AI Agent:**
> Done. Tomorrow's Pilates session dynamic base price now rests at 8 SmartSpot credits to capitalize on higher morning demand.


## ❓ FAQ

**Q: Do I need to be a ClassPass partner?**
Yes. This server is for ClassPass venue partners. You need a Partner Dashboard account, a Venue ID, and API credentials obtained through your ClassPass partner manager.

**Q: Can it change SmartSpot credit allocation algorithms?**
Absolutely. You can prompt the AI to review fill rates and apply strategic modifications to the underlying SmartSpot settings for any class type directly.

**Q: How exactly are no-shows tracked?**
The tool parses check-in flags from the ClassPass partner API in real-time, instantly reporting members who missed their slot without late cancellation.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/classpass](https://vinkius.com/mcp/classpass)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **ClassPass** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `classpass` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **ClassPass** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "classpass": {
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
