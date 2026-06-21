# Expedia MCP Server

Automate travel planning via Expedia — search hotels, compare flights, find rental cars, and build complete trip itineraries directly from any AI agent.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/expedia)

## Overview
**Category:** ecommerce
**Tools Count:** 13

## Description
Connect your **Expedia Group** developer account to any AI agent and take programmatic control over one of the world's largest travel ecosystems — hotels, flights, and car rentals in a single integration.

### What you can do

- **Hotel Search & Booking** — Find properties by destination, dates, and guest count, then pull room quotes and create bookings directly
- **Flight Discovery** — Search flight routes by origin, destination, and date, then retrieve detailed quotes for specific itineraries
- **Car Rental Lookup** — Query available vehicles at any airport, compare categories, and get pricing quotes
- **Quote Comparison** — Pull detailed pricing breakdowns for hotels, flights, and cars to make data-driven travel decisions
- **Booking Management** — Create and cancel reservations across all travel categories programmatically

### How it works

1. Sign up at the [Expedia Group Developer Hub](https://developers.expediagroup.com/) and create an API project
2. Generate your API Key and API Secret from the developer portal
3. Enter your credentials here and start planning trips from Claude, Cursor, or any MCP-compatible client

Your agent becomes a full-service travel assistant — searching across hotels, flights, and cars without switching between tabs or websites.

### Who is this for?

- **Corporate Travel Managers** — build complete team travel itineraries combining flights, hotels, and ground transport in one conversation
- **Travel Agencies** — automate multi-segment trip research for clients with real-time pricing from a single source
- **Executive Assistants** — plan and modify complex business travel schedules without navigating multiple booking platforms


## Available Tools
- **book_flight**: Book an airline passenger ticket
- **cancel_booking**: Cancel an active property reservation
- **create_booking**: Execute a lodging booking reservation
- **get_car_quotes**: Get active quotes for a rental car class
- **get_flight_quotes**: Get exact real-time pricing for a queried flight
- **get_property_detail**: Get detailed content for a specific property
- **get_room_quotes**: Get live room rates and availability
- **search_cars**: Search for rental cars at specific airport branches
- **search_flights**: Search for airline flights
- **search_properties**: Search for hotels and lodging properties
- **book_car**: Requires driver name and email for confirmation. Returns a booking ID that can be used to manage the reservation. ALWAYS confirm booking details with the user before executing this action.

Book a rental car using a quote ID
- **cancel_flight**: Refund eligibility depends on the fare class and airline cancellation policy. Returns the cancellation status and any applicable refund details. ALWAYS confirm the booking ID and inform the user about potential cancellation fees before executing.

Cancel an existing flight booking
- **search_regions**: Returns region IDs, names, types, and coordinates. This is the essential first step before searching for properties — you need a valid destination identifier from this tool to use search_properties. For example, searching "Paris" returns the city region ID, specific arrondissements, and CDG airport.

Search for geographic regions by name


## Installation & Usage

To install and use the **Expedia** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/expedia](https://vinkius.com/mcp/expedia)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
