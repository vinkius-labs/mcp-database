# Edmunds MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/edmunds)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [databases](../categories/databases.md)

Access comprehensive automotive data via Edmunds — decode VINs, list car makes and models, inspect engine specs, and query vehicle styles directly from any AI agent.

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


## Available Tools (41)
- **get_safety_by_make_model_year**: All three parameters must be provided.

Get safety ratings by make/model/year
- **get_make_details**: Provide the make name.

Get details on a specific car make
- **get_makes_with_tco**: Do not query without specifying a required parameter.

Get car makes with TCO value
- **list_model_years**: Filter by makeNiceName and modelNiceName.

Get a list of model years
- **get_photos_by_style**: Pass the required style ID.

Find photos by style ID
- **get_dealership_franchises**: Provide the required Dealership ID.

Find dealership franchises
- **get_editorial_make**: Provide the make name.

Get editorial make overview
- **get_transmissions**: Provide the style ID.

Get transmissions for a car style
- **get_used_tco_details**: Supply the Style ID and ZIP Code.

Get TCO details for used car
- **list_styles**: Filter by makeNiceName and modelNiceName.

Get a list of styles
- **submit_dealer_review**: Ensure the body contains all required review data.

Submit dealer review
- **submit_dealer_review_comment**: Ensure the body contains all required comment data.

Submit dealer review comment
- **calculate_new_tmv**: Supply both the Style ID and ZIP Code.

Get TMV price for a new car
- **calculate_typically_equipped_used_tmv**: Supply both the Style ID and ZIP Code.

Get TMV price for a typically equipped used car
- **calculate_used_tmv**: Supply the Style ID, ZIP Code, and mileage.

Get TMV price for a used car
- **decode_vin**: Provide the full 17-digit VIN as the primary input.

Get vehicle details through VIN decoding
- **find_certified_price**: Supply both the Style ID and ZIP Code.

Get TMV price for a certified vehicle
- **get_color**: Provide the color ID.

Get color details by ID
- **get_dealer_reviews**: Provide the dealer ID.

Get dealer ratings and reviews by dealer ID
- **get_editorial_model**: Provide the make and model names.

Get editorial model overview
- **get_editorial_model_year**: Provide make, model, and year.

Get editorial model/year overview
- **get_editorial_road_tests**: Provide make, model, and year.

Get editorial road tests overview
- **get_engines**: Provide the style ID.

Get engines for a car style
- **get_expert_content**: Provide make, model, and year.

Get expert content for make/model/year
- **get_maintenance_schedule**: Use this tool only when the model year is known.

Get maintenance schedule by car model year ID
- **get_makes_count**: Get total count of car makes
- **get_models_with_tco**: Provide the Make ID.

Get car models with TCO value
- **get_new_tco**: Supply both the Style ID and ZIP Code.

Get TCO for a new car
- **get_new_tco_details**: Supply the Style ID and ZIP Code.

Get TCO details for new car
- **get_new_tmv_by_msrp_vin**: Provide all three values.

Get TMV price for a new car by MSRP and VIN
- **get_new_total_cash_price**: Supply both the Style ID and ZIP Code.

Get the Total Cash Price for a new car
- **get_photos_by_make_model_year**: Provide all three required vehicle identifiers.

Find photos by make/model/year
- **get_recalls**: Use this tool only when the model year is known.

Get vehicle recalls by car model year ID
- **get_reviews_by_make_model_year**: Provide the make, model, and year.

Get car consumer ratings and reviews by make/model/year
- **get_reviews_by_style**: Provide the style ID to proceed.

Get car consumer ratings and reviews by style ID
- **get_safety_by_style**: Provide the style ID to proceed.

Get safety ratings by style ID
- **get_squish_vin**: The VIN must be the first 11 digits minus the 9th digit.

Get vehicle details by Squish VIN
- **get_years_with_styles**: Provide all three identifiers.

Get years with styles for a car make/model
- **list_equipments**: Provide the style ID.

Get equipments list
- **list_makes**: Use makeNiceName to filter results.

Get a list of car makes
- **list_models**: Filter by makeNiceName if necessary.

Get a list of models


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Edmunds** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all available car makes."

**🤖 AI Agent:**
> I've retrieved the list of car makes. There are currently over 50 makes available, including Acura, Audi, BMW, Ford, Honda, Toyota, and more. Would you like to get details on a specific make?

---

**👤 You:**
> "Decode this VIN: 1FTFW1EF5CFAXXXXX"

**🤖 AI Agent:**
> Decoding VIN... This vehicle is identified as a Ford F-150. I can fetch more detailed specifications, engine options, or equipment lists for this model if you'd like.

---

**👤 You:**
> "Get the engine specifications for style ID 401234567."

**🤖 AI Agent:**
> Querying engine specs... For style ID 401234567, the engine is a 3.5L V6 EcoBoost. It features twin-turbocharging, direct injection, and produces 375 horsepower. Let me know if you need transmission or color details as well.


## ❓ FAQ

**Q: Can my AI decode a full 17-digit VIN using this server?**
Yes! Use the `decode_vin` tool with a full 17-digit VIN. Your agent will return detailed vehicle specifications, including make, model, year, and trim details.

**Q: How do I find the engine and transmission options for a specific car style?**
You can use the `get_engines` and `get_transmissions` tools by passing the unique `style_id` of the vehicle. This will retrieve complete technical specifications for that specific configuration.

**Q: What is a Squish VIN and how do I query it?**
A Squish VIN consists of the first 11 digits of a VIN minus the 9th digit (check digit). You can query it using the `get_squish_vin` tool to identify vehicle details when a full VIN is not available.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/edmunds](https://vinkius.com/en/ai-agent-connect/edmunds)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Edmunds** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `edmunds` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Edmunds** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "edmunds": {
      "url": "https://edge.vinkius.com/[TOKEN]/mcp"
    }
  }
}
```

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius connector registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
