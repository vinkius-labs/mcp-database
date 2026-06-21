# Edmunds MCP Server

Access comprehensive automotive data via Edmunds — decode VINs, list car makes and models, inspect engine specs, and query vehicle styles directly from any AI agent.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/edmunds)

## Overview
**Category:** databases
**Tools Count:** 41

## Description
Connect your **Edmunds** API key to any AI agent and unlock deep automotive intelligence through natural conversation.

### What you can do

- **Vehicle Identification** — Decode full 17-digit VINs (`decode_vin`) or query vehicle details using Squish VINs (`get_squish_vin`)
- **Makes & Models** — List car makes (`list_makes`), get specific make details (`get_make_details`), and count total makes (`get_makes_count`)
- **Model Years & Styles** — Query model years (`list_model_years`), find years with styles (`get_years_with_styles`), and list styles (`list_styles`)
- **Technical Specs** — Fetch engine details (`get_engines`), transmission types (`get_transmissions`), colors (`get_color`), and equipment lists (`list_equipments`)

### How it works

1. Subscribe to this server
2. Enter your Edmunds API Key
3. Start querying automotive data from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Automotive Developers** — instantly retrieve vehicle specs and decode VINs directly inside your IDE
- **Data Analysts** — gather structured vehicle data, makes, models, and technical specifications effortlessly
- **Dealership & Fleet Managers** — query precise vehicle configurations, engine types, and equipment lists


## Available Tools
- **calculate_new_tmv**: Get TMV price for a new car
- **calculate_typically_equipped_used_tmv**: Get TMV price for a typically equipped used car
- **calculate_used_tmv**: Get TMV price for a used car
- **get_color**: Get color details by ID
- **get_dealer_reviews**: Get dealer ratings and reviews by dealer ID
- **get_dealership_franchises**: Find dealership franchises
- **get_editorial_make**: Get editorial make overview
- **get_editorial_model**: Get editorial model overview
- **get_editorial_model_year**: Get editorial model/year overview
- **get_editorial_road_tests**: Get editorial road tests overview
- **get_engines**: Get engines for a car style
- **list_equipments**: Get equipments list
- **get_expert_content**: Get expert content for make/model/year
- **find_certified_price**: Get TMV price for a certified vehicle
- **get_maintenance_schedule**: Get maintenance schedule by car model year ID
- **get_make_details**: Get details on a specific car make
- **get_makes_count**: Get total count of car makes
- **list_makes**: Get a list of car makes
- **get_makes_with_tco**: Get car makes with TCO value
- **list_model_years**: Get a list of model years
- **list_models**: Get a list of models
- **get_models_with_tco**: Get car models with TCO value
- **get_new_tco_details**: Get TCO details for new car
- **get_new_tco**: Get TCO for a new car
- **get_new_tmv_by_msrp_vin**: Get TMV price for a new car by MSRP and VIN
- **get_new_total_cash_price**: Get the Total Cash Price for a new car
- **get_photos_by_make_model_year**: Find photos by make/model/year
- **get_photos_by_style**: Find photos by style ID
- **get_recalls**: Get vehicle recalls by car model year ID
- **get_reviews_by_make_model_year**: Get car consumer ratings and reviews by make/model/year
- **get_reviews_by_style**: Get car consumer ratings and reviews by style ID
- **get_safety_by_make_model_year**: Get safety ratings by make/model/year
- **get_safety_by_style**: Get safety ratings by style ID
- **get_squish_vin**: Get vehicle details by Squish VIN
- **list_styles**: Get a list of styles
- **submit_dealer_review_comment**: Submit dealer review comment
- **submit_dealer_review**: Submit dealer review
- **get_transmissions**: Get transmissions for a car style
- **get_used_tco_details**: Get TCO details for used car
- **decode_vin**: Get vehicle details through VIN decoding
- **get_years_with_styles**: Get years with styles for a car make/model


## Installation & Usage

To install and use the **Edmunds** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/edmunds](https://vinkius.com/mcp/edmunds)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
