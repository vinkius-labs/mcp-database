# Overpass (OpenStreetMap) MCP Server

Search OpenStreetMap data — find restaurants, shops, hospitals, schools, parks, ATMs and more worldwide.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/overpass-openstreetmap)

## Overview
**Category:** data-analytics
**Tools Count:** 16

## Description
Connect to **Overpass API** (OpenStreetMap) and query the world's largest free geographic database through natural conversation — no API key needed.

### What you can do

- **Amenity Search** — Find restaurants, cafes, hospitals, schools, pharmacies, ATMs, fuel stations and more
- **Shop Search** — Discover shops, supermarkets, bakeries, clothing stores and retail outlets
- **Nearby Search** — Find any amenity within a radius of any GPS coordinate
- **Hotel Search** — Locate hotels, hostels and tourist accommodation
- **Park Search** — Find parks, gardens and green spaces
- **EV Charging** — Locate electric vehicle charging stations
- **Custom Queries** — Execute custom Overpass QL queries for any OSM data

### How it works

1. Subscribe to this server
2. No API key needed — Overpass is a free public service
3. Start exploring geographic data from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Travelers** — find restaurants, hotels, ATMs and amenities near your location
- **Urban Planners** — analyze infrastructure, amenities and land use patterns
- **Developers** — integrate OpenStreetMap data into location-based applications


## Available Tools
- **custom_query**: The query should be valid Overpass QL syntax. The output format is automatically set to JSON. If no out statement is included, "out geom;" is appended automatically. Example: `node["amenity"="cafe"](51.5,-0.15,51.51,-0.14); out geom;`

Execute a custom Overpass QL query
- **search_amenities**: Common amenities: "restaurant", "cafe", "school", "hospital", "pharmacy", "bank", "atm", "fuel", "parking", "toilets", "library", "police", "fire_station", "post_office", "cinema", "theatre", "nightclub", "bar", "pub", "fast_food", "ice_cream". Bbox format: lat_min,lon_min,lat_max,lon_max.

Search for amenities (restaurants, schools, hospitals, etc.) in a bounding box
- **search_atms**: Returns ATM locations, operator/bank names, addresses, 24/7 availability and network info. Bbox format: lat_min,lon_min,lat_max,lon_max.

Search for ATMs in a bounding box
- **search_by_name**: Optional amenity filter to narrow results. Returns matching elements with full details including addresses, phone numbers and websites.

Search for OSM elements by name
- **search_by_tag**: Bbox format: lat_min,lon_min,lat_max,lon_max (e.g. "51.249,-0.15,51.251,-0.10" for central London). Useful for finding specific OSM-tagged features.

Search OpenStreetMap elements by tag key/value in a bounding box
- **search_charging_stations**: Returns station names, addresses, connector types, charging speeds, operator info and access details. Bbox format: lat_min,lon_min,lat_max,lon_max.

Search for EV charging stations in a bounding box
- **search_fuel_stations**: Returns station names, brands, addresses, fuel types offered, opening hours and operator info. Bbox format: lat_min,lon_min,lat_max,lon_max.

Search for fuel/gas stations in a bounding box
- **search_hospitals**: Returns facility names, addresses, phone numbers, emergency services info, specialties and operator info. Bbox format: lat_min,lon_min,lat_max,lon_max.

Search for hospitals and clinics in a bounding box
- **search_hotels**: Returns hotel names, addresses, star ratings, phone numbers, websites and room info. Bbox format: lat_min,lon_min,lat_max,lon_max.

Search for hotels in a bounding box
- **search_nearby**: Useful for finding nearby amenities without defining a full bounding box. Returns names, addresses, distances and details.

Search for OSM elements near a specific location
- **search_nearby_amenities**: Common amenities: "restaurant", "cafe", "pharmacy", "atm", "bank", "hospital", "school", "supermarket", "fuel", "charging_station", "parking", "toilets", "police", "fire_station", "post_office".

Search for specific amenities near a location
- **search_parks**: Returns park names, addresses, area sizes, features (playgrounds, sports facilities) and operator info. Bbox format: lat_min,lon_min,lat_max,lon_max.

Search for parks and green spaces in a bounding box
- **search_pharmacies**: Returns pharmacy names, addresses, phone numbers, opening hours, dispensing info and operator info. Bbox format: lat_min,lon_min,lat_max,lon_max.

Search for pharmacies in a bounding box
- **search_restaurants**: Optional cuisine filter: "italian", "chinese", "japanese", "indian", "mexican", "thai", "french", "american", "pizza", "burger", "sushi", "vegan", "vegetarian". Bbox format: lat_min,lon_min,lat_max,lon_max.

Search for restaurants in a bounding box
- **search_schools**: Returns school names, addresses, phone numbers, websites, student capacity and operator info. Bbox format: lat_min,lon_min,lat_max,lon_max.

Search for schools in a bounding box
- **search_shops**: Optional shop type filter: "supermarket", "convenience", "clothes", "bakery", "butcher", "electronics", "furniture", "hardware", "jewelry", "mall", "bookmaker", "car", "car_repair", "chemist", "florist", "gift", "hairdresser", "mobile_phone", "shoes", "sports", "toys". Bbox format: lat_min,lon_min,lat_max,lon_max.

Search for shops in a bounding box


## Installation & Usage

To install and use the **Overpass (OpenStreetMap)** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/overpass-openstreetmap](https://vinkius.com/mcp/overpass-openstreetmap)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
