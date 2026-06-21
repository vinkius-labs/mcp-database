# Kavak MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/kavak)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [industry-titans](../categories/industry-titans.md)

Browse, inspect, finance, and reserve certified used cars from Kavak — Mexico's largest online used car platform — directly from any AI agent.

## Description
Connect to the **Kavak** platform from any AI agent and navigate Mexico's largest certified pre-owned vehicle marketplace through natural conversation.

### What you can do

- **Vehicle Search** — Browse thousands of certified pre-owned vehicles with filters for make, model, year, price range, and free-text queries
- **240-Point Inspection Reports** — Access the detailed mechanical inspection results that every Kavak vehicle undergoes before listing
- **Vehicle History** — Check ownership count, accident records, service history, and legal status for any listed vehicle
- **Trade-In Valuations** — Get instant AI-powered buy-back offers for your current vehicle based on make, model, year, mileage, and condition
- **Financing Calculator** — View available credit plans across multiple terms (12-60 months) with different down payment scenarios
- **Reservations & Test Drives** — Reserve vehicles and schedule test drives at Kavak hubs across Mexico
- **Market Intelligence** — Query average prices, trends, and price ranges for any make/model/year in the Mexican used car market

### How it works

1. Subscribe to this server
2. Enter your Kavak API Key and Secret
3. Start browsing cars from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Car Buyers** — search, compare, and reserve vehicles without endlessly scrolling through listings
- **Used Car Dealers** — leverage Kavak's market pricing intelligence for competitive analysis
- **Financial Advisors** — calculate financing options for clients looking to purchase vehicles


## Available Tools (14)
- **create_reservation**: Requires buyer contact details. The vehicle will be taken off the marketplace during the reservation period.

Reserve a vehicle for purchase
- **estimate_trade_in**: The estimate factors in make, model, year, mileage, condition, and current Mexican market prices.

Get a trade-in value estimate for your current car
- **get_financing_options**: Calculate financing plans for a vehicle
- **get_vehicle_history**: Check the ownership and accident history of a car
- **get_vehicle_inspection**: View the 240-point mechanical inspection report
- **get_market_pricing**: Get market pricing intelligence for a car model
- **get_reservation**: Check the status of a vehicle reservation
- **get_vehicle**: Get full details of a specific car
- **list_locations**: Each location includes its address, operating hours, available services (test drives, inspections, deliveries), and contact details.

Find Kavak showroom locations
- **list_makes**: List all available car manufacturers
- **list_models**: List models available for a specific make
- **list_reservations**: List all your active reservations
- **schedule_test_drive**: Kavak also offers home test drives in select cities where the vehicle is delivered to the buyer's address.

Schedule a test drive for a vehicle
- **search_vehicles**: All vehicles listed on Kavak come with a 240-point mechanical inspection and Kavak warranty.

Search available used cars in the Kavak inventory


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Kavak** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Find me Toyota Corollas from 2020-2023 under $350,000 MXN."

**🤖 AI Agent:**
> I found 8 Toyota Corollas matching your criteria: 1. 2022 Corolla SE — $329,000 MXN (42,000 km, automatic, silver). 2. 2021 Corolla LE — $298,000 MXN (58,000 km, automatic, white). 3. 2020 Corolla Base — $265,000 MXN (71,000 km, manual, gray). All include Kavak's 240-point inspection and 3-month warranty. Would you like to see the inspection report or financing options for any of these?

---

**👤 You:**
> "What would Kavak offer me for my 2019 Nissan Sentra with 85,000 km?"

**🤖 AI Agent:**
> Based on Kavak's AI valuation engine, your 2019 Nissan Sentra (85,000 km, assumed 'good' condition) has an estimated trade-in value of $178,500 MXN. The current Kavak selling price for equivalent models is $215,000-$235,000 MXN. This offer is valid for 7 days. Would you like to proceed with the trade-in process or browse vehicles to buy with the trade-in credit?

---

**👤 You:**
> "Show financing options for vehicle ID KV-88201 with a $50,000 MXN down payment."

**🤖 AI Agent:**
> Financing options for KV-88201 (2022 Mazda 3 — $345,000 MXN) with $50,000 enganche: 12 months: $27,100/mo (12.9% rate, CAT 16.2%). 24 months: $14,500/mo (13.9% rate, CAT 17.5%). 36 months: $10,300/mo (14.5% rate, CAT 18.8%). 48 months: $8,250/mo (15.2% rate, CAT 19.5%). 60 months: $7,100/mo (15.9% rate, CAT 20.1%). Would you like to reserve this vehicle?


## ❓ FAQ

**Q: Can I get an instant trade-in offer for my current car?**
Yes! Use the `estimate_trade_in` tool with your car's make, model, year, mileage, and condition. Kavak's AI valuation engine will return an instant buy-back offer based on current Mexican market conditions and comparable recent transactions.

**Q: What does the 240-point inspection cover?**
Use `get_vehicle_inspection` to see the full 240-point report. It covers engine health, transmission status, brake system, tire condition, electrical systems, suspension, body/paint integrity, interior condition, and all safety features. Each point is rated as pass, warning, or replaced.

**Q: Can I calculate monthly payments for different financing scenarios?**
Yes. Use `get_financing_options` with the vehicle ID and an optional down payment amount (enganche). It returns a matrix of monthly payment options across 12, 24, 36, 48, and 60-month terms, each with interest rates, total cost, and CAT (Costo Anual Total).


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/kavak](https://vinkius.com/mcp/kavak)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Kavak** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `kavak` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Kavak** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "kavak": {
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
