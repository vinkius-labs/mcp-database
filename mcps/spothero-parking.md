# SpotHero Parking MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/spothero-parking)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/spothero-parking-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/spothero-parking-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Search, compare, and book parking spots in 400+ cities via SpotHero API.

## Description
Connect **SpotHero** to any AI agent and simplify urban mobility — search parking by location, compare prices, book reservations, and manage vehicle details through natural conversation.

### What you can do
- **Spot Search** — Find available parking spots by coordinates and time range
- **Dynamic Pricing** — Compare rates and get real-time pricing for specific durations
- **Instant Booking** — Create reservations instantly with vehicle info and payment method
- **Reservation Management** — View, update vehicle details, or cancel existing bookings
- **Event Awareness** — Discover nearby events that might impact parking availability
- **Garage Details** — Access garage amenities, hours, and contact info

### How it works
1. Subscribe to this server
2. Enter your SpotHero Partner API Key and Base URL
3. Start managing urban parking from Claude, Cursor, or any MCP-compatible client

SpotHero is the leading parking marketplace in North America, covering over 400 cities.

### Who is this for?
- **Navigation Apps** — integrate real-time parking availability and booking into route planning
- **Event Organizers** — help attendees find and reserve parking near venues automatically
- **Fleet Managers** — book parking for delivery vehicles or company cars efficiently


## Available Tools
- **book_parking**: Requires spot ID, start/end times, payment method ID, and vehicle info (make, model, plate, color).

Book a parking spot and create a reservation
- **cancel_reservation**: Check cancellation policy for refund eligibility.

Cancel an active parking reservation
- **get_spot_details**: Get detailed information and pricing for a specific parking spot
- **search_events**: Useful for anticipating demand.

Search for nearby events that might affect parking availability or pricing
- **get_garage_details**: Get information about a specific garage
- **get_reservation**: Get details of a specific parking reservation
- **list_reservations**: Optional status filter (upcoming, past, cancelled).

List all parking reservations for the authenticated account
- **get_pricing**: Useful for comparing rates before booking.

Get dynamic pricing for a parking spot for a specific duration
- **search_parking**: Use this to find parking options for users. Times must be in ISO 8601 format.

Search for available parking spots near a location for a specific time range
- **update_vehicle_info**: Use this if the user changes cars before parking.

Update vehicle information for an existing reservation


## 💬 Prompt Examples

Here are some examples of how you can interact with the **SpotHero Parking** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Find parking near Times Square for 2 hours starting now."

**🤖 AI Agent:**
> Found 5 spots within 0.5 miles. Cheapest: Icon Parking at $15/hr. Most convenient: Edison ParkFast (2 min walk) at $22 total.

---

**👤 You:**
> "Book spot 12345 from 9 AM to 5 PM tomorrow."

**🤖 AI Agent:**
> Reservation created! ID: SH-998877. Total cost: $24. QR Code sent to your email. Vehicle: Black Honda Civic (ABC-1234).

---

**👤 You:**
> "What events are happening downtown tonight?"

**🤖 AI Agent:**
> Found 3 events: 1) Concert at City Hall (7 PM). 2) Sports Game at Arena (8 PM). Parking rates nearby are +20% due to high demand.


## Installation & Usage

To install and use the **SpotHero Parking** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/spothero-parking](https://vinkius.com/mcp/spothero-parking)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
