# SpotHero Parking MCP Server

Search, compare, and book parking spots in 400+ cities via SpotHero API.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/spothero-parking)

## Overview
**Category:** productivity
**Tools Count:** 10

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


## Installation & Usage

To install and use the **SpotHero Parking** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/spothero-parking](https://vinkius.com/mcp/spothero-parking)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
