# Cabify MCP Server

AI ride management for business: book rides, track trips, and manage corporate mobility via agents.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/cabify)

## Overview
**Category:** finance-accounting
**Tools Count:** 9

## Description
### What you can do

Connect AI agents to the Cabify Business platform for enterprise mobility management:

- **Get price estimates** across all Cabify tiers (Lite, Executive, Taxi)
- **Compare trip durations** with real-time traffic data
- **Request rides directly** with pickup and dropoff coordinates
- **Track active rides** with driver info, vehicle details, and live ETA
- **Cancel rides** when plans change
- **View complete ride history** with business expense tracking
- **Manage saved locations** for frequent business destinations
- **Check available service tiers** at any location in Spain and LATAM

### How it works

1. **Connect your Cabify Business account** via API key from Cabify Empresas portal
2. **Ask your AI agent** to estimate rides, book trips, or check ride history
3. **No app navigation needed** — natural language commands execute all operations
4. **Business expense tracking** integrated with your corporate Cabify account

### Who is this for?

Perfect for **business travelers**, **corporate assistants**, **travel managers**, **HR coordinators**, and **companies** using Cabify Empresas in Spain, Portugal, and Latin America. Let AI agents handle employee transportation, manage business travel expenses via ride history, and coordinate executive mobility. Ideal for companies with 10+ monthly corporate rides who want streamlined booking workflows, centralized expense tracking, and automated ride management across multiple offices.


## Available Tools
- **add_saved_location**: Common use cases: save office addresses, frequent client locations, hotels, airports. Returns the saved location details including the new location ID. Use this to build a library of frequently used destinations for faster ride booking.

Save a new location for the Cabify account
- **cancel_ride**: Cancellation policies vary based on ride status - cancellations after driver assignment may incur fees depending on Cabify Empresas policy. Use this to cancel rides that were booked by mistake or are no longer needed.

Cancel an existing Cabify ride request
- **get_available_products**: Returns product IDs, names, descriptions, capacity, and features. Use this to see which service options are available before requesting estimates or booking rides.

Get available Cabify service tiers at a location
- **get_price_estimate**: Prices are in local currency (EUR for Spain, local currency for LATAM). Use this to compare costs across different Cabify service tiers before booking.

Get price estimate for a Cabify ride between two locations
- **get_ride_details**: Use this to track your active ride or review past trip details.

Get details of a specific Cabify ride
- **get_ride_history**: Returns ride date, status, origin/destination, product type, driver, cost, and business expense category. Use this to review past rides, calculate business expenses, or find previous trip details.

Get ride history for the Cabify Business account
- **get_saved_locations**: Returns location IDs, names, addresses, and coordinates. Use this to quickly reference saved locations for ride requests without typing full addresses. Common for frequent business destinations.

Get saved locations for the Cabify account
- **get_time_estimate**: Accounts for current traffic conditions and typical route times. Use this to plan schedules and compare route efficiency across different pickup/dropoff points.

Get estimated trip duration for a Cabify ride
- **request_ride**: Requires origin and destination coordinates. Optionally specify product ID (from get_available_products), pickup address, and dropoff address for clarity. Returns the ride ID, driver assignment status, and estimated pickup time. Use this to book a ride after confirming price and availability.

Request a new Cabify ride


## Installation & Usage

To install and use the **Cabify** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/cabify](https://vinkius.com/mcp/cabify)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
