# NHTSA Vehicle Safety MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/nhtsa-vehicle-safety)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [industry-titans](../categories/industry-titans.md)

Decode VINs, search recalls and complaints, check safety ratings and find car seat inspection stations.

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


## 💬 Prompt Examples

Here are some examples of how you can interact with the **NHTSA Vehicle Safety** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Decode VIN 1HGBH41JXMN109186."

**🤖 AI Agent:**
> 2021 Honda Accord Sedan. 4-door, 1.5L Turbo, FWD, Automatic. Made in Marysville, Ohio. Safety features: ABS, ESC, Tire Pressure Monitor, Front/Side Airbags.

---

**👤 You:**
> "Are there any recalls for a 2023 Ford F-150?"

**🤖 AI Agent:**
> Found 3 recalls for 2023 Ford F-150: 1) Rear Axle Hub Bolt (Campaign 23V-456, 2023-07-15) — 2) Windshield Wiper Motor (Campaign 23V-789, 2023-09-20) — 3) Backup Camera Display (Campaign 24V-012, 2024-01-10).

---

**👤 You:**
> "What's the safety rating for a 2024 Toyota Camry?"

**🤖 AI Agent:**
> 2024 Toyota Camry: Overall 5/5 ⭐. Frontal Crash: 5/5. Side Crash: 5/5. Rollover: 4/5. Excellent safety ratings across all categories.


## ❓ FAQ

**Q: Do I need an API key?**
No! NHTSA data is completely free and open government data. No authentication required.

**Q: What is a VIN?**
VIN (Vehicle Identification Number) is a unique 17-character code assigned to every vehicle. It encodes the manufacturer, model, year, engine type, assembly plant and more. Find it on your dashboard or driver's door jamb.

**Q: Can I check recalls for my car?**
Yes! Use get_recalls_by_vehicle with your car's make, model and year. Or use decode_vin with your VIN for complete vehicle details including any open recalls.

**Q: What do safety ratings mean?**
NHTSA rates vehicles 1-5 stars in frontal crash, side crash and rollover tests. Overall rating combines all categories. 5 stars is the highest safety rating.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/nhtsa-vehicle-safety](https://vinkius.com/mcp/nhtsa-vehicle-safety)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **NHTSA Vehicle Safety** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `nhtsa-vehicle-safety` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **NHTSA Vehicle Safety** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "nhtsa-vehicle-safety": {
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
