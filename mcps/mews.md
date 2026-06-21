# Mews MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/mews)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/mews-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/mews-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [erp-operations](../categories/erp-operations.md)

Manage hotel reservations, guests, rooms, billing, housekeeping, and services for your Mews property through natural conversation.

## Description
Connect your **Mews** hotel to any AI agent and transform your front desk into an intelligent, voice-ready concierge.

### What you can do

- **Reservations** — Today's check-ins, upcoming arrivals, room assignments, and booking status
- **Guests** — Search profiles, loyalty tiers, preferences, allergies, and past stays
- **Rooms** — Real-time room status: vacant/occupied, housekeeping (clean/dirty/inspected)
- **Billing** — Guest folios, charges, payments, and balance tracking
- **Rates & Services** — Rate plans, bookable services, and POS outlet items
- **Property** — Hotel configuration, departments, and operational settings

### Who is this for?

- **Front Desk** — "Who is checking in today? Any VIP arrivals?" — instant morning briefing
- **Revenue Managers** — Rate plan performance, occupancy trends, and ADR analysis
- **Housekeeping** — Room status dashboard, turnover priorities, and out-of-order tracking
- **General Managers** — Daily operational KPIs across all departments


## Available Tools
- **get_reservations**: Filter by date range. THE core tool — "Who is checking in today?" "How many rooms tonight?"

Get hotel reservations
- **list_bills**: Filter by guest for their complete financial history.

List guest bills
- **list_payments**: With amounts, dates, and settlement status.

List payments
- **get_property_info**: Get hotel configuration
- **get_reservation**: Get reservation details
- **search_guests**: Returns profile, contact info, nationality, loyalty status, past stays, preferences, and billing history.

Search hotel guests
- **get_guest**: Get guest profile
- **list_rooms**: List hotel rooms
- **list_room_blocks**: With dates, room types, and release dates.

List room blocks
- **list_rates**: With pricing, restrictions, and availability rules.

List room rates
- **list_services**: List hotel services
- **list_outlet_items**: With pricing and categories.

List POS items


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Mews** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Who is checking in today and are there any VIP guests?"

**🤖 AI Agent:**
> 🏨 **Today's Check-ins — Oct 18**

📊 **12 arrivals** | 3 VIP | 2 groups

**VIP Arrivals** ⭐
- **Sir James & Lady Henderson** — Presidential Suite 801
  💎 Platinum loyalty | 14 past stays | $127,000 LTV
  🍾 Pre-arrival: champagne, flowers, late check-out

- **Dr. Sarah Chen** — Deluxe King 412
  💎 Gold loyalty | Business travel
  🚗 Airport transfer confirmed 14:30

**Group: Acme Corp Retreat** (8 rooms)
- Arriving 15:00-17:00 | Conference Room B reserved
- Contact: Maria Lopez, VP Operations

---

**👤 You:**
> "Show me the housekeeping status for the 3rd floor."

**🤖 AI Agent:**
> On the 3rd floor: 12 rooms are Clean and Inspected, 5 rooms are Dirty (currently occupied), and Room 304 is Out of Order due to a plumbing issue. Housekeeping should prioritize Room 310 which has a VIP arrival at 2:00 PM.

---

**👤 You:**
> "What is our average daily rate (ADR) for this weekend?"

**🤖 AI Agent:**
> The projected Average Daily Rate (ADR) for this upcoming Friday to Sunday is $245. This is driven by high demand and strong performance in our premium suite categories.


## Installation & Usage

To install and use the **Mews** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/mews](https://vinkius.com/mcp/mews)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
