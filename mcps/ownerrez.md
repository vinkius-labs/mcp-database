# OwnerRez MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/ownerrez)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [finance-accounting](../categories/finance-accounting.md)

Manage vacation rental bookings, properties, guests, calendars, financials, inquiries, and channel connections for your OwnerRez account through natural conversation.

## Description
Connect your **OwnerRez** account to any AI agent and get the most advanced vacation rental intelligence at your fingertips.

### What you can do

- **Bookings** — All reservations with deep financial breakdown: charges, payments, balance
- **Properties** — Portfolio management with seasonal rates, cleaning fees, and house rules
- **Guests** — Search profiles with stay history, reviews, and lifetime revenue
- **Calendar** — Day-by-day availability per property with pricing and minimum stay
- **Financials** — Charges, payments, refunds, and full accounting trail
- **Inquiries** — Pending booking inquiries from all channels for conversion tracking
- **Channels** — Connected platforms status: Airbnb, VRBO, Booking.com, direct

### Who is this for?

- **Power Users** — OwnerRez is the tool for owners who want maximum control
- **Multi-Property Owners** — Portfolio-wide analytics and revenue optimization
- **Finance** — Deep charge/payment tracking and reconciliation
- **Direct Booking** — Inquiry management and conversion optimization


## Available Tools (10)
- **list_properties**: List rental properties
- **get_property**: Get property details
- **search_guests**: Returns contact info, stay history, reviews received, and total revenue.

Search guests
- **list_bookings**: Filter by status: booked, checked_in, checked_out, cancelled.

List rental bookings
- **list_channels**: com, direct website. With status and sync health.

List connected channels
- **get_booking**: Get booking details
- **get_calendar**: Get property calendar
- **list_charges**: Deep financial breakdown.

List booking charges
- **list_payments**: With amounts, dates, and processing status.

List booking payments
- **list_inquiries**: For conversion tracking.

List booking inquiries


## 💬 Prompt Examples

Here are some examples of how you can interact with the **OwnerRez** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What bookings do I have arriving this weekend and what's still owed?"

**🤖 AI Agent:**
> 🔑 **Weekend Arrivals — Oct 18-20**

1. **Johnson Family** — Lake House
   📅 Oct 18-22 | 👥 6 | 📱 VRBO
   💰 Total: $1,850 | Paid: $1,850 | ✅ Balance: $0

2. **Mike & Sarah Davis** — Mountain Cabin
   📅 Oct 19-21 | 👥 2 | 📱 Airbnb
   💰 Total: $420 | Paid: $420 | ✅ Balance: $0

3. **Thompson Party** — Beach Cottage
   📅 Oct 19-26 | 👥 8 | 📱 Direct
   💰 Total: $3,200 | Paid: $1,600 | ⚠️ **Balance: $1,600 due Oct 17**

---

**👤 You:**
> "Show me all properties in our Florida portfolio with their seasonal rates."

**🤖 AI Agent:**
> Here are 2 properties in Florida.
1. Ocean Breeze Villa: Summer rate $450/night, Winter rate $250/night.
2. Palm Retreat: Summer rate $300/night...

---

**👤 You:**
> "Find the booking for John Smith from last month and show the balance."

**🤖 AI Agent:**
> Booking #B12345 for John Smith (Stay: Sept 10-15). Total charges: $1,200. Total payments: $1,200. Balance due: $0. Security deposit of $300 was refunded.


## ❓ FAQ

**Q: What makes OwnerRez different from Guesty?**
OwnerRez is built for power users who want maximum control over pricing, financials, and channel management. It has the most flexible API, deep accounting features, and is popular with US vacation rental owners managing their own properties.

**Q: Does it support multiple channels like Airbnb and VRBO?**
Yes, OwnerRez acts as a powerful channel manager syncing availability, rates, and messaging across Airbnb, VRBO, Booking.com, and direct booking sites.

**Q: Can I manage cleaning schedules here?**
While OwnerRez primarily handles bookings and financials, it does push calendar events that can be used to trigger cleaning tasks and coordinate with external cleaning services.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/ownerrez](https://vinkius.com/mcp/ownerrez)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **OwnerRez** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `ownerrez` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **OwnerRez** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "ownerrez": {
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
