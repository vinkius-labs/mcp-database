# BlaBlaCar MCP Server

AI carpool search: find rides, compare prices, and book shared journeys via agents.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/blablacar)

## Overview
**Category:** productivity
**Tools Count:** 8

## Description
### What you can do

Connect AI agents to the world's largest carpooling network for affordable, sustainable travel:

- **Search carpool rides** between any cities or GPS coordinates worldwide
- **Compare prices and schedules** across multiple drivers and departure times
- **Review driver profiles** with ratings, verification status, and vehicle details
- **Find bus trips** on BlaBlaCar Bus routes for longer distances
- **Search with flexible dates** to find cheapest travel days
- **International rides** across borders with country-specific filtering
- **Radius-based searches** for flexible pickup location options

### How it works

1. **Get your BlaBlaCar API key** from the developer portal
2. **Ask your AI agent** to search rides, compare options, or check driver profiles
3. **Natural language commands** replace manual website searches
4. **Instant comparisons** across dozens of available rides and schedules

### Who is this for?

Ideal for **budget travelers**, **students**, **eco-conscious commuters**, **travel planners**, and **digital nomads**. Let AI agents find the cheapest rides, compare schedules across dates, verify driver credibility, and plan multi-city carpool routes. Perfect for anyone taking 2+ intercity trips monthly who wants to save 40-60% vs trains while reducing carbon footprint through shared transportation.


## Available Tools
- **get_driver_profile**: Use this to verify driver credibility and read passenger reviews before booking a ride. Requires the driver user ID from a trip result.

Get driver profile and ratings on BlaBlaCar
- **get_trip_details**: Use this before booking to verify driver credibility, vehicle comfort, and exact pickup location.

Get complete details of a specific BlaBlaCar trip including driver and vehicle info
- **search_bus_trips**: BlaBlaCar operates both carpooling and bus services. Bus trips are operated by professional drivers on fixed routes. Returns bus departure/arrival times, prices, and availability. Use this for longer distance or when carpool options are limited.

Search BlaBlaCar Bus trips between two locations
- **search_flexible_dates**: Much larger result set than exact-date search. Useful when travel dates are not fixed and user wants to compare prices/availability across multiple days. Returns up to 50 results spanning several days.

Search carpool trips with flexible dates around a target date
- **search_international_trips**: Requires origin/destination coordinates plus country codes (e.g., FR, DE, ES, IT, PT). Returns all available international rides with driver details and pricing. Use this for trips crossing national borders.

Search international carpool trips between two countries on BlaBlaCar
- **search_trips_by_city**: More user-friendly than coordinate-based search. Returns all matching trips with departure/arrival points, times, prices, driver ratings, and available seats. Best for general city-to-city searches without needing exact coordinates.

Search carpool trips between two city names on BlaBlaCar
- **search_trips**: Requires latitude,longitude format for both points. Returns trip details including departure/arrival cities, times, price, driver info, and available seats. Use this for precise location-based searches when you know exact coordinates.

Search carpool trips between two GPS coordinates on BlaBlaCar
- **search_trips_with_radius**: Useful when exact pickup/dropoff locations are flexible. Larger radius returns more options but may require additional travel to reach departure points. Returns all rides within the specified radius.

Search carpool trips with flexible radius around coordinates


## Installation & Usage

To install and use the **BlaBlaCar** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/blablacar](https://vinkius.com/mcp/blablacar)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
