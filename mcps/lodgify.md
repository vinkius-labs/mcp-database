# Lodgify MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/lodgify)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/lodgify-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/lodgify-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [ecommerce](../categories/ecommerce.md)

Manage vacation rental properties, bookings, availability, rates, quotes, and channel connections for your Lodgify account through natural conversation.

## Description
Connect **Lodgify** to any AI agent — vacation rental management + booking website.

### What you can do
- **Properties** — All listings with amenities, photos, and house rules
- **Bookings** — Reservations with guest details and payment status
- **Availability** — Day-by-day calendar with min stay rules
- **Rates** — Seasonal pricing, discounts, and length-of-stay adjustments
- **Quotes** — Instant pricing for any dates and guest count
- **Channels** — OTA sync status


## Available Tools
- **list_properties**: List vacation rental properties
- **get_property**: Get property details
- **list_bookings**: List bookings
- **get_booking**: Get booking details
- **get_availability**: Get property availability
- **get_rates**: Get property rates
- **get_quote**: Get booking quote
- **list_channels**: com, VRBO, direct. With sync status.

List channels


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Lodgify** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "How much would it cost for 4 guests at the Lake House from Dec 20 to Jan 2?"

**🤖 AI Agent:**
> 🏡 **Lake House — 13 nights (Dec 20 - Jan 2)**

🛏️ 4 guests | Holiday Season Rates

💰 Pricing:
- Accommodation: $3,250 (13 × $250)
- Cleaning fee: $150
- Taxes: $340
- **Total: $3,740**

✅ Available! | Min 5 nights | Free cancellation until Dec 10

---

**👤 You:**
> "Block the calendar for the Beach Condo from October 10 to October 15 for maintenance."

**🤖 AI Agent:**
> I have successfully blocked the calendar for the Beach Condo property from October 10 to October 15. The 'maintenance' block will prevent any new bookings across your direct site and connected channels.

---

**👤 You:**
> "Show me the booking conversion rate for the last month."

**🤖 AI Agent:**
> In the last 30 days, your website received 1,200 views resulting in 48 quotes and 15 confirmed bookings. This represents a 1.25% visitor-to-booking conversion rate, slightly up from last month.


## Installation & Usage

To install and use the **Lodgify** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/lodgify](https://vinkius.com/mcp/lodgify)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
