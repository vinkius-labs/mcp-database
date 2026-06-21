# Corrently Energy MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/corrently-energy)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [data-analytics](../categories/data-analytics.md)

Access German energy market data — GrünstromIndex, CO₂ forecasts, solar predictions, electricity prices, and optimized scheduling for smart energy consumption.

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


## Available Tools (12)
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


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Corrently Energy** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is the renewable energy forecast for Berlin zip code 10115 today?"

**🤖 AI Agent:**
> I've fetched the GrünstromIndex forecast for Berlin 10115. Over the next 24 hours, renewable energy availability ranges from 45% to 78%. The greenest window is between 11:00-15:00 when solar generation peaks, with GSI values reaching 72-78. CO₂ intensity during this period drops to approximately 280 g/kWh.

---

**👤 You:**
> "When is the best 4-hour window to run my dishwasher in Munich 80331 to use the greenest energy?"

**🤖 AI Agent:**
> Analyzing the optimal window... The best 4-hour period for low-CO₂ energy in Munich 80331 is from 10:00 to 14:00. During this timeframe, solar generation is at its peak and grid CO₂ intensity drops to around 250 g/kWh. Starting your dishwasher at 10:00 AM will maximize renewable energy usage.

---

**👤 You:**
> "Show me current electricity market prices for Hamburg 20095 and tell me when it's cheapest today."

**🤖 AI Agent:**
> Fetching market data for Hamburg 20095... Current wholesale electricity prices range from 45 €/MWh to 120 €/MWh today. The cheapest hours are 12:00-15:00 (solar peak, ~48 €/MWh) and 02:00-05:00 overnight (~52 €/MWh). The most expensive period is 18:00-20:00 evening peak at ~115 €/MWh.


## ❓ FAQ

**Q: Do I need an API token to use the Corrently Energy MCP server?**
No! Most Corrently API endpoints work without authentication. An optional token is only needed if you want higher rate limits for heavy usage. Simply subscribe to the server and start querying energy data immediately.

**Q: What German zip codes are supported for energy forecasts?**
All German Postleitzahl (PLZ) 5-digit zip codes are supported — from 01067 (Dresden) to 80331 (Munich). Simply provide any valid German zip code and the API will return localized energy forecasts for that region's grid area.

**Q: Can I use this MCP server to optimize when I charge my electric vehicle?**
Absolutely! Use the `get_best_hour` tool to find optimal charging windows based on renewable energy availability or lowest CO₂ emissions. Then use `create_energy_schedule` to generate a full optimized charging plan. You can also use `get_phev_charge_or_fuel` if you drive a plug-in hybrid and need advice on whether to charge electrically or use fuel.

**Q: How accurate are the solar generation predictions for my photovoltaic system?**
The `get_solar_prediction` tool provides forecasts based on weather models and your system's kWp capacity. Accuracy depends on location, panel orientation, and weather conditions. It's best used for relative comparisons (e.g., "Will tomorrow be sunnier than today?") rather than absolute precision. For typical home systems (5-10 kWp), day-ahead forecasts are generally within 15-25% of actual generation.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/corrently-energy](https://vinkius.com/mcp/corrently-energy)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Corrently Energy** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `corrently-energy` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Corrently Energy** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "corrently-energy": {
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
