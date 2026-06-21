# Corrently Energy MCP Server

Access German energy market data — GrünstromIndex, CO₂ forecasts, solar predictions, electricity prices, and optimized scheduling for smart energy consumption.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/corrently-energy)

## Overview
**Category:** data-analytics
**Tools Count:** 12

## Description
Connect to **Corrently Energy APIs** and bring real-time German energy market intelligence to any AI agent. Monitor renewable energy availability, optimize consumption schedules, and make data-driven decisions for sustainable power usage.

### What you can do

- **GrünstromIndex (GSI)** — Get hourly forecasts for renewable energy availability, showing when green power from wind and solar is most abundant
- **CO₂ Predictions** — Track carbon intensity of electricity consumption by German zip code with real-time and forecasted emissions data
- **Best Hour Finder** — Automatically identify optimal time windows for energy-intensive activities based on renewable peaks and lowest CO₂
- **Market Data** — Access current electricity market prices, wholesale costs, and regional pricing forecasts
- **Solar Forecasts** — Predict photovoltaic generation output for specific solar installations based on location and capacity (kWp)
- **Energy Scheduling** — Create intelligent operating schedules for EVs, heat pumps, and industrial equipment optimized for price, solar, or emissions
- **Merit Order** — View the current energy generation mix showing which power plants are active and their cost efficiency
- **Real-Time CO₂ Meter** — Check instant carbon intensity readings (g CO₂/kWh) for any German location
- **PHEV Decision Support** — Get smart advice for plug-in hybrid drivers on whether to charge electrically or use fuel
- **CO₂ Offset Calculator** — Calculate compensation requirements and available options for neutralizing carbon footprints
- **Renewable Dispatch** — Monitor renewable energy feed-in data showing wind and solar contributions to the grid
- **Stromkonto Balance** — Check electricity account balances and green energy certificates

### How it works

1. Subscribe to this server
2. (Optional) Enter your Corrently API token for higher rate limits — many endpoints work without authentication
3. Start querying German energy data from Claude, Cursor, or any MCP-compatible client

Your AI becomes an energy analyst, helping you consume electricity when it's greenest, cheapest, or cleanest.

### Who is this for?

- **Homeowners with Solar Panels** — predict your PV system output and find the best times to run appliances using self-generated clean energy
- **EV Owners** — schedule charging sessions during high renewable availability or lowest electricity prices
- **Energy Consultants** — retrieve market data, merit order lists, and dispatch information for analysis
- **Sustainability Teams** — monitor CO₂ intensity and calculate offsets for corporate environmental reporting
- **Smart Home Enthusiasts** — integrate energy-aware decision logic into automated home systems


## Available Tools
- **get_best_hour**: Perfect for scheduling energy-intensive activities.

USE WHEN:
- User asks when is the best time to use energy-intensive appliances
- User wants to optimize energy consumption for green power or low emissions
- User needs to schedule operations during clean energy peaks
- User asks about optimal charging times for EVs or running machinery

PARAMETERS:
- zip (REQUIRED): German zip code (Postleitzahl) - exactly 5 digits
- hours (OPTIONAL): Number of consecutive hours needed (default: 1, min: 1, max: 168)

EXAMPLES:
- "When is the best 3-hour window to run my dishwasher in Berlin 10115?" → call with zip="10115", hours=3
- "Best time to charge my EV in Munich tonight" → call with zip="80331", hours=6
- "When should I use high-power appliances today?" → call with zip="70173", hours=2

Find the best hours for energy consumption based on renewable availability and low CO₂ emissions
- **calculate_co2_offset**: Helps users understand how to neutralize their carbon footprint.

USE WHEN:
- User asks how to offset their CO₂ emissions
- User wants to calculate carbon compensation needed
- User needs information about CO₂ compensation options
- User asks about neutralizing their carbon footprint from activities

PARAMETERS:
- co2_kg (REQUIRED): Amount of CO₂ in kilograms to offset (minimum: 0.1)
- activity_type (OPTIONAL): Type of activity that generated emissions (e.g. "flight", "car", "heating")

EXAMPLES:
- "How much does it cost to offset 500 kg of CO₂?" → call with co2_kg=500
- "Calculate offset for my flight emissions" → call with co2_kg=250, activity_type="flight"
- "I drove 1000km, what is the CO₂ compensation?" → call with co2_kg=180, activity_type="car"

Calculate CO₂ offset requirements and available compensation options
- **get_co2_meter**: Shows grams of CO₂ per kWh right now.

USE WHEN:
- User asks about current/real-time CO₂ levels in the electricity grid
- User wants instant carbon intensity data
- User needs to know how clean/dirty the electricity is right now
- User asks about live carbon emissions from power

PARAMETERS:
- zip (REQUIRED): German zip code (Postleitzahl) - exactly 5 digits

EXAMPLES:
- "What is the current CO₂ intensity in Berlin 10115?" → call with zip="10115"
- "Show me real-time carbon levels for Munich 80331" → call with zip="80331"
- "Current CO₂ emissions from electricity in Cologne" → call with zip="50667"

Get real-time CO₂ meter readings for a German zip code
- **get_co2_prediction**: Shows how carbon-intensive the power grid will be over time.

USE WHEN:
- User asks about CO₂ emissions or carbon footprint of electricity
- User wants to know when electricity is cleanest/lowest emissions
- User needs carbon intensity data for a location

PARAMETERS:
- zip (REQUIRED): German zip code (Postleitzahl) - exactly 5 digits

EXAMPLES:
- "What are the CO₂ emissions for Hamburg 20095?" → call with zip="20095"
- "Show carbon intensity for Frankfurt 60311" → call with zip="60311"

Get CO₂ emissions forecast for electricity consumption in Germany
- **create_energy_schedule**: Schedules are optimized based on electricity prices, solar generation peaks, CO₂ emissions, or comfort levels.

USE WHEN:
- User wants to create an automated schedule for energy devices
- User needs to optimize when to run appliances for cost or green energy
- User asks to schedule energy consumption for the next hours
- User wants smart scheduling for their heat pump, EV charger, or machinery

PARAMETERS:
- zip (REQUIRED): German zip code (Postleitzahl) - exactly 5 digits
- hours (REQUIRED): Number of hours for the schedule operation (1-36 hours)
- optMode (OPTIONAL): Optimization mode - "price" (cheapest), "solar" (max solar), "emission" (lowest CO₂), "comfort" (balanced). Default: "price"

EXAMPLES:
- "Create a 12-hour schedule for Berlin 10115 optimized for lowest price" → call with zip="10115", hours=12, optMode="price"
- "Schedule my EV charging for next 8 hours in Munich using solar energy" → call with zip="80331", hours=8, optMode="solar"
- "Optimize my heat pump for 24 hours with lowest emissions in Hamburg" → call with zip="20095", hours=24, optMode="emission"

Create an optimized energy schedule for appliances and devices
- **get_dispatch**: Shows how much renewable energy is being fed into the grid and its composition.

USE WHEN:
- User asks about renewable energy feed-in for a location
- User needs dispatch data for renewable energy sources
- User wants to understand the renewable energy flow in their area
- User asks about wind and solar contribution to the grid

PARAMETERS:
- zip (REQUIRED): German zip code (Postleitzahl) - exactly 5 digits

EXAMPLES:
- "Show renewable energy dispatch for Berlin 10115" → call with zip="10115"
- "How much renewable energy is being fed into the grid in Munich?" → call with zip="80331"
- "Wind and solar dispatch for Hamburg 20095" → call with zip="20095"

Get renewable energy dispatch information for a German zip code
- **get_gsi_prediction**: USE WHEN:
- User asks about green energy availability or renewable power forecast
- User wants to know the GrünstromIndex or GSI for a location
- User needs to understand when clean energy is most abundant

PARAMETERS:
- zip (REQUIRED): German zip code (Postleitzahl) - exactly 5 digits, e.g. "10115" for Berlin
- token (OPTIONAL): API token for higher rate limits - auto-provided from credentials

EXAMPLES:
- "What is the renewable energy forecast for Berlin 10115?" → call with zip="10115"
- "Show me the green power index for Munich 80331" → call with zip="80331"

Get GrünstromIndex (Green Power Index) prediction for a German zip code
- **get_market_data**: Includes wholesale prices and regional cost data.

USE WHEN:
- User asks about electricity prices or costs in a specific location
- User needs market data, wholesale prices, or energy cost forecasts
- User wants to compare energy costs across time periods
- User asks about cheap/expensive electricity hours

PARAMETERS:
- zip (REQUIRED): German zip code (Postleitzahl) - exactly 5 digits

EXAMPLES:
- "What are current electricity prices in Berlin 10115?" → call with zip="10115"
- "Show me energy market data for Cologne 50667" → call with zip="50667"
- "When is electricity cheapest today in Stuttgart 70173?" → call with zip="70173"

Get current electricity market data and pricing information for a German location
- **get_merit_order_list**: This shows which energy sources are being used to generate electricity and their cost efficiency.

USE WHEN:
- User asks about the current energy generation mix
- User wants to understand which power plants are active
- User needs merit order data for market analysis
- User asks about energy source prioritization in the grid

EXAMPLES:
- "Show me the current merit order list" → call with no extra params
- "What energy sources are currently generating power?" → call with no extra params
- "Merit order ranking for Germany" → call with no extra params

Get the current merit order list for the German energy market
- **get_phev_charge_or_fuel**: USE WHEN:
- User asks whether to charge their PHEV or use fuel
- PHEV driver needs advice on optimal energy source
- User wants to know if now is a good time to charge their hybrid
- User asks about cost-efficiency of electric vs fuel for their PHEV

PARAMETERS:
- zip (REQUIRED): German zip code (Postleitzahl) - exactly 5 digits

EXAMPLES:
- "Should I charge my PHEV or use fuel in Berlin 10115?" → call with zip="10115"
- "Charge or fuel decision for Munich 80331" → call with zip="80331"
- "Is now a good time to charge my hybrid in Hamburg?" → call with zip="20095"

Get decision support for plug-in hybrid (PHEV) drivers - charge or fuel
- **get_solar_prediction**: Shows expected energy production over time.

USE WHEN:
- User asks about solar panel output or PV system generation
- User needs forecasts for their solar installation
- User wants to know expected renewable energy production
- User asks how much energy their solar panels will generate

PARAMETERS:
- zip (REQUIRED): German zip code (Postleitzahl) - exactly 5 digits
- kwp (REQUIRED): Solar panel capacity in kilowatt peak (kWp), range: 0.1 to 1000

EXAMPLES:
- "How much energy will my 5 kWp solar system generate in Berlin 10115?" → call with zip="10115", kwp=5
- "Solar forecast for my 10 kWp installation in Munich 80331" → call with zip="80331", kwp=10
- "Expected PV output for 3.5 kWp in Hamburg 20095" → call with zip="20095", kwp=3.5

Get solar energy generation forecast for a photovoltaic installation
- **get_stromkonto_balance**: Shows credits, green energy certificates, and account status.

USE WHEN:
- User asks about their electricity account balance
- User wants to check their Stromkonto status
- User needs information about their green energy credits or certificates
- User asks about their energy account

PARAMETERS:
- account (REQUIRED): Account identifier for the Stromkonto

EXAMPLES:
- "Check my Stromkonto balance for account 0x123abc" → call with account="0x123abc"
- "Show my energy account status" → call with account="USER_ACCOUNT_ID"

Get Stromkonto (electricity account) balance information


## Installation & Usage

To install and use the **Corrently Energy** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/corrently-energy](https://vinkius.com/mcp/corrently-energy)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
