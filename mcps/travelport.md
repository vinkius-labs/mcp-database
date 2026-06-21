# Travelport MCP Server

Access Travelport's Global Distribution System to search and book flights, hotels, and manage travel reservations directly through AI.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/travelport)

## Overview
**Category:** industry-titans
**Tools Count:** 21

## Description
Connect to **Travelport**, the world's leading travel commerce platform, and empower your AI agent to handle complex travel itineraries, real-time flight searches, and hotel bookings.

### What you can do

- **Flight Intelligence** — Search for catalog product offerings, price specific flight legs, and retrieve full pricing details for air offers.
- **Hotel Management** — Search for stays by location or ID, check real-time availability, and retrieve detailed hotel rules and policies.
- **Booking Workbench** — Initialize reservation sessions (workbench), add offers and travelers, and commit bookings to create official PNRs.
- **Payment & Security** — Validate credit cards, verify addresses, and manage payment authorizations directly within the booking flow.
- **Reservation Retrieval** — Fetch existing flight and hotel reservations to provide status updates or itinerary details.

### How it works

1. Subscribe to this server
2. Enter your Travelport credentials (Client ID, Secret, Username, Password, and Access Group)
3. Start searching and booking travel from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Travel Agents & Concierges** — Automate the search and booking process for clients using natural language.
- **Corporate Travel Managers** — Quickly retrieve reservation details and check flight availability without manual GDS entry.
- **Developers** — Integrate travel booking capabilities into custom AI workflows and travel assistants.


## Available Tools
- **add_offer_to_workbench**: Add an air offer to an existing workbench
- **add_traveler_to_workbench**: Add a traveler to an existing workbench
- **authorize_card**: Authorize a payment card
- **check_hotel_availability**: Check hotel availability (v11)
- **commit_workbench**: Commit a reservation workbench to create a booking
- **create_hotel_reservation**: Create a hotel reservation (v11)
- **create_workbench**: Create a new reservation workbench session
- **get_hotel_rules**: Get hotel rules (v11)
- **price_offer_full**: Price an air offer fully from products
- **price_offer_reference**: Price an air offer from a catalog reference
- **retrieve_flight_reservation**: Retrieve an existing flight reservation
- **retrieve_hotel_reservation**: Retrieve an existing hotel reservation
- **reverse_authorization**: Reverse a payment card authorization
- **search_flight_specific**: Perform a flight specific search
- **search_flights**: Search for flight catalog product offerings
- **search_next_leg**: Search for the next leg of a flight itinerary
- **search_stays_complete**: Perform a complete hotel search (v12)
- **search_stays_by_id**: Search for hotel properties by ID (v11)
- **search_stays_by_location**: Search for hotel properties by location (v11)
- **validate_card**: Validate a payment card
- **verify_address**: Verify a payment card address (AAVS)


## Installation & Usage

To install and use the **Travelport** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/travelport](https://vinkius.com/mcp/travelport)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
