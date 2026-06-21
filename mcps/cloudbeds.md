# Cloudbeds MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/cloudbeds)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/cloudbeds-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/cloudbeds-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [ecommerce](../categories/ecommerce.md)

Manage hotel reservations, guests, rooms, housekeeping, availability, and revenue dashboard for your Cloudbeds property through natural conversation.

## Description
Connect your **Cloudbeds** property to any AI agent and run your hotel from a single conversation.

### What you can do

- **Reservations** — Browse, filter by status, and drill into booking details
- **Guests** — Search profiles, view stay history and lifetime value
- **Rooms & Housekeeping** — Real-time room status and cleaning priorities
- **Availability** — Check open rooms for any date range instantly
- **Transactions** — Track charges, payments, and guest balances
- **Dashboard** — Today's KPIs: occupancy, revenue, ADR, check-ins/outs

### Who is this for?

- **Hotel Owners** — Morning briefing with one question: "How did we do yesterday?"
- **Front Desk** — Instant guest lookup, availability checks, and booking details
- **Revenue Managers** — ADR trends, occupancy forecasting, and rate optimization
- **Housekeeping** — Prioritized room cleaning lists and status updates


## Available Tools
- **list_reservations**: Filter by status: confirmed, checked_in, checked_out, cancelled. Core front-desk tool.

List hotel reservations
- **get_dashboard**: The GM's morning briefing.

Get property dashboard
- **get_reservation**: Get reservation details
- **search_guests**: Returns profile, contact, nationality, past stays, preferences, and lifetime value.

Search hotel guests
- **get_guest**: Get guest profile
- **list_rooms**: List hotel rooms
- **list_room_types**: With max occupancy, amenities, base rate, and room count.

List room types
- **get_housekeeping**: For housekeeping management.

Get housekeeping status
- **check_availability**: Essential for booking inquiries and revenue management.

Check room availability
- **list_transactions**: Filter by reservation to see a guest's complete financial history.

List financial transactions


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Cloudbeds** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What's our occupancy and revenue for today?"

**🤖 AI Agent:**
> 🏨 **Today's Dashboard — Oct 18**

📊 **Occupancy**: 87% (52/60 rooms)
💰 **Revenue**: $8,420
📈 **ADR**: $161.92

🔄 **Movement**:
- 8 check-ins expected
- 5 check-outs completed
- 3 rooms available tonight

🧹 **Housekeeping**: 5 rooms dirty, 3 inspected

---

**👤 You:**
> "List dirty rooms pending turnover for the afternoon layout."

**🤖 AI Agent:**
> Checking housekeeping statuses... Currently, Suite 104, Room 201, and Room 305 remain in 'Dirty' status awaiting cleaning. Room 102 was just marked 'Inspected'.

---

**👤 You:**
> "Find the ongoing reservation of Mr. Anderson."

**🤖 AI Agent:**
> Guest profile fetched. Thomas Anderson occupies Room 205 (Ocean View). Checked in on Tuesday, scheduled to check out tomorrow at 11 AM. Balance owed: $0.00.


## Installation & Usage

To install and use the **Cloudbeds** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/cloudbeds](https://vinkius.com/mcp/cloudbeds)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
