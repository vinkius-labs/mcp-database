# NHTSA Vehicle Safety MCP Server

Decode VINs, search recalls and complaints, check safety ratings and find car seat inspection stations.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/nhtsa-vehicle-safety)

## Overview
**Category:** industry-titans
**Tools Count:** 13

## Description
Connect to **NHTSA** (National Highway Traffic Safety Administration) and access US vehicle safety data through natural conversation — no API key needed.

### What you can do

- **VIN Decoding** — Decode any 17-character VIN to reveal make, model, year, engine, transmission and safety features
- **Recall Search** — Search safety recalls by make, model and year or by campaign number
- **Consumer Complaints** — Browse vehicle owner complaints filed with NHTSA by make, model or ODI number
- **Safety Ratings** — Check NHTSA crash test ratings (overall, frontal, side, rollover)
- **Car Seat Stations** — Find certified car seat inspection stations by ZIP code or GPS coordinates

### How it works

1. Subscribe to this server
2. No API key needed — NHTSA data is open government data
3. Start exploring vehicle safety data from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Car Buyers** — check safety ratings, recalls and complaint history before purchasing
- **Car Owners** — look up recalls for your vehicle and find nearby car seat inspection stations
- **Researchers** — analyze safety data, complaint trends and recall patterns


## Available Tools
- **decode_vin**: Returns comprehensive vehicle specifications from the NHTSA database.

Decode a Vehicle Identification Number (VIN)
- **get_models_for_make_year**: Useful for discovering what models a brand offered in a particular year.

Get models for a manufacturer in a specific year
- **get_car_seat_stations_by_zip**: Returns station name, address, phone, hours and appointment requirements. Useful for parents needing car seat safety checks.

Find car seat inspection stations by ZIP code
- **get_complaint_by_odi**: Returns failure description, consequences, remedy, component, mileage and dates.

Get complaint details by ODI number
- **get_complaints_by_vehicle**: Returns complaints filed by vehicle owners including component, failure description, consequences, mileage at failure and date. At least one parameter recommended.

Search consumer complaints by make, model and year
- **get_car_seat_stations_by_location**: Returns station name, address, phone, hours and distance. Useful for finding nearby car seat safety checks.

Find car seat inspection stations by coordinates
- **get_makes_for_year**: Useful for discovering which brands were active in a particular year.

Get all manufacturers for a specific model year
- **get_models_for_make**: Useful for discovering the full lineup of a brand.

Get all models for a specific manufacturer
- **get_recalls_by_campaign**: Returns component, summary, consequence, remedy, manufacturer notes, dates and affected vehicle count.

Get recall details by campaign number
- **get_recalls_by_vehicle**: Returns recall details including campaign number, component affected, summary, remedy, manufacturer, dates and affected vehicle count. At least one parameter (make, model, year) is recommended.

Search safety recalls by make, model and year
- **get_safety_rating_by_vehicle_id**: Returns overall rating and detailed breakdown by crash type.

Get safety rating for a specific vehicle by NHTSA ID
- **get_safety_ratings**: Returns overall rating and breakdown by frontal crash, side crash and rollover. If only year provided, returns all vehicles for that year. Add make and model for specific vehicle ratings.

Get NHTSA safety ratings for vehicles
- **get_vehicle_types_for_make**: g. Passenger Car, Truck, SUV, Motorcycle, Trailer). Useful for discovering what categories a manufacturer produces.

Get vehicle types for a specific manufacturer


## Installation & Usage

To install and use the **NHTSA Vehicle Safety** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/nhtsa-vehicle-safety](https://vinkius.com/mcp/nhtsa-vehicle-safety)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
