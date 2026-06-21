# Uber MCP Server

AI ride management: estimate prices, track trips, and manage locations via agents.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/uber)

## Overview
**Category:** industry-titans
**Tools Count:** 9

## Description
### What you can do

Connect your AI agents to the Uber platform for seamless ride management and trip planning:

- **Get available ride products** (UberX, Black, Comfort) at any location
- **Estimate prices** across all ride types before booking
- **Compare pickup times** to choose the fastest option
- **View complete trip history** with pricing and route data
- **Save and manage favorite places** (Home, Work, custom locations)
- **Autocomplete place searches** for accurate pickup/dropoff coordinates

### How it works

1. **Connect your Uber account** via Server Token from the Uber Developer Portal
2. **Ask your AI agent** to estimate rides, check history, or manage saved locations
3. **No app navigation needed** — natural language commands execute all operations
4. **Instant insights** on pricing and availability across all Uber products

### Who is this for?

Perfect for **frequent travelers**, **executive assistants**, **travel planners**, and **corporate teams** managing business transportation. Let AI agents handle ride planning, expense tracking via trip history, and location management. Ideal for professionals taking 10+ Uber rides monthly who want streamlined booking workflows and cost comparison automation.


## Available Tools
- **add_saved_place**: Requires alias name, latitude, and longitude. Optionally include a full address string. The alias can be home, work, or any custom string. Returns the saved place details.

Save a new place for the authenticated Uber user
- **get_trip_history**: Returns trip date, start/end locations, product used, distance, and price. Use this to review past rides, calculate expenses, or find a previous trip details.

Get trip history for the authenticated Uber user
- **get_user_profile**: Use this to verify authentication and confirm which Uber account is connected.

Get the authenticated Uber user profile
- **get_place_autocomplete**: Requires current user location to bias results. Returns place descriptions and structured address components. Use this to help users select valid pickup/dropoff locations before requesting rides.

Autocomplete place predictions for Uber locations
- **get_price_estimate**: Prices are in local currency. Use this to compare costs across different Uber ride types before booking.

Get price estimate for an Uber ride between two locations
- **get_products**: ) available at the specified latitude/longitude. Returns product IDs, display names, capacity, and descriptions. Use this to see which ride options are available before requesting a ride or price estimate.

Get available Uber products at a location
- **get_ride_estimate**: More specific than price estimates as it targets one product. Use this to get exact pricing before requesting a ride.

Get detailed ride estimate for a specific Uber product
- **get_saved_places**: Returns place aliases, addresses, and coordinates. Use this to quickly reference saved locations for ride requests or price estimates without typing addresses.

List saved places for the authenticated Uber user
- **get_time_estimate**: Use this to compare how quickly different Uber services can pick you up. Lower times mean faster pickups.

Get estimated pickup time for Uber at a location


## Installation & Usage

To install and use the **Uber** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/uber](https://vinkius.com/mcp/uber)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
