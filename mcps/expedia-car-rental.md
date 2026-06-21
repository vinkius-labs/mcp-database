# Expedia Car Rental MCP Server

Automate car rental workflows via Expedia — search available vehicles, compare pricing by category, and manage rental bookings directly from any AI agent.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/expedia-car-rental)

## Overview
**Category:** order-management
**Tools Count:** 8

## Description
Connect your **Expedia Rapid API** account to any AI agent and search the full car rental inventory across major global rental agencies.

### What you can do

- **Vehicle Search** — Find available cars at any airport or city location, filtered by dates, vehicle category, and passenger capacity
- **Price Comparison** — Compare rental rates across economy, compact, SUV, and luxury categories with transparent pricing breakdowns
- **Pickup Locations** — Query all available pickup and drop-off points near your destination, including airport counters and city offices
- **Booking Management** — Create and cancel car rental reservations programmatically through the Rapid API
- **Agency Details** — Retrieve information about rental agencies including policies, hours, and contact details

### How it works

1. Sign up at the [Expedia Group Developer Hub](https://developers.expediagroup.com/) and create a Rapid API project
2. Generate your API Key and Shared Secret from the portal
3. Enter your credentials here and start searching car inventories from Claude, Cursor, or any MCP-compatible client

Your agent becomes a personal car rental assistant — finding the best deals across agencies without visiting multiple websites.

### Who is this for?

- **Corporate Travel Managers** — book fleet rentals for traveling teams with instant price comparison across agencies
- **Travel Planners** — build complete road trip itineraries with vehicle selection matched to route requirements
- **Operations Teams** — automate recurring rental bookings for field staff and regional offices


## Available Tools
- **book_car**: Requires the car offer ID from a previous search, driver details (first name, last name, email), and confirmation of rental terms. Returns the booking confirmation with itinerary ID, which is needed for future retrieval or cancellation of the reservation. Ensure all date/times match the original search parameters.

Book a rental car for the specified dates and location
- **cancel_itinerary**: Returns cancellation confirmation and any applicable refund details based on the rental supplier cancellation policy. Some bookings may incur cancellation fees if cancelled outside the free cancellation window. Always verify the itinerary details before cancelling.

Cancel an existing car rental reservation
- **get_car_details**: Use the car ID returned from the search_cars tool.

Get detailed information for a specific rental car offer
- **get_car_images**: Includes exterior shots, interior views, and representative images of the vehicle class. Helps users visually confirm the type of vehicle they are considering renting. Use the car ID from search results or car details.

Get images for a specific rental car vehicle
- **get_itinerary**: Use the itinerary ID returned when the booking was created.

Retrieve details of a confirmed car rental reservation
- **get_pickup_locations**: Returns detailed location information including address, operating hours, supplier counters available at each location, and special instructions. Useful for helping users find convenient rental locations near their travel destination.

Search for available car rental pickup locations
- **search_car_regions**: Returns region identifiers that can be used as pickup_location parameters in the search_cars tool. Useful for exploring rental options when the user knows a city or region name but not the specific location code. Supports partial text matching.

Search for car rental regions and destinations
- **search_cars**: Required parameters include pickup location identifier, pickup date-time, and dropoff date-time. Optional filters include vehicle class, supplier, max price, and currency preference. Returns a list of available vehicles with pricing, supplier details, vehicle class, and included amenities.

Search for available rental cars by location, dates, and optional filters


## Installation & Usage

To install and use the **Expedia Car Rental** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/expedia-car-rental](https://vinkius.com/mcp/expedia-car-rental)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
