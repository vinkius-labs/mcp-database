# Overpass (OpenStreetMap) MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/overpass-openstreetmap)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [data-analytics](../categories/data-analytics.md)

Search OpenStreetMap data — find restaurants, shops, hospitals, schools, parks, ATMs and more worldwide.

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


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Overpass (OpenStreetMap)** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Find all restaurants in Lower Manhattan."

**🤖 AI Agent:**
> Found 250+ restaurants in Lower Manhattan (bbox: 40.70,-74.02,40.72,-73.98). Includes Italian, Chinese, Japanese, American, Mexican and many more cuisines. Names, addresses, phone numbers and opening hours included.

---

**👤 You:**
> "Find ATMs within 500m of Times Square (40.7580, -73.9855)."

**🤖 AI Agent:**
> Found 18 ATMs within 500m of Times Square. Operators include Chase, Bank of America, Citibank, Wells Fargo and independent ATM networks. Locations include buildings, stores and subway stations.

---

**👤 You:**
> "Find EV charging stations in downtown San Francisco."

**🤖 AI Agent:**
> Found 45 EV charging stations in downtown SF. Includes Tesla Superchargers, ChargePoint, EVgo and Blink stations. Connector types, charging speeds and access info provided.


## ❓ FAQ

**Q: Do I need an API key?**
No! Overpass API is completely free and open. No authentication required. Please be respectful with query sizes — avoid queries returning more than 10,000 elements.

**Q: What is a bounding box?**
A bounding box defines a geographic area using min_latitude, min_longitude, max_latitude, max_longitude. Example: "40.70,-74.01,40.72,-73.98" covers Lower Manhattan, NYC.

**Q: Can I search near my current location?**
Yes! Use search_nearby or search_nearby_amenities with your GPS coordinates and a radius in meters (e.g. lat=40.7128, lon=-74.0060, radius=1000 for 1km around NYC).

**Q: What amenities can I search for?**
Common amenities: restaurant, cafe, fast_food, bar, pub, hospital, clinic, pharmacy, school, university, library, atm, bank, fuel, parking, police, fire_station, post_office, toilets, cinema, theatre, nightclub, museum.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/overpass-openstreetmap](https://vinkius.com/mcp/overpass-openstreetmap)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Overpass (OpenStreetMap)** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `overpass-openstreetmap` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Overpass (OpenStreetMap)** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "overpass-openstreetmap": {
      "url": "https://edge.vinkius.com/[TOKEN]/mcp"
    }
  }
}
```

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
