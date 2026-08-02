# Kelley Blue Book Valuation MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/kelley-blue-book-valuation)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [data-analytics](../categories/data-analytics.md)

Get vehicle valuations and market data via Kelley Blue Book — search cars, get trade-in values, and fair market pricing.

## Description
Connect your AI agent to **Kelley Blue Book (KBB)**, the most trusted resource for vehicle valuation and automotive research. This integration allows you to retrieve real-time market values, trade-in estimates, and fair purchase ranges through natural conversation.

### What you can do

- **Vehicle Discovery** — Search for thousands of cars by make, model, and year to get precise KBB vehicle IDs
- **Accurate Valuation** — Get estimated trade-in and private party values by providing mileage, condition, and ZIP code
- **Configuration Details** — Access full technical specifications and trim levels for specific vehicle models
- **VIN Lookup** — Instantly retrieve vehicle data using the 17-character Vehicle Identification Number
- **Market Intelligence** — Monitor market trends and regional pricing shifts to make informed buying or selling decisions
- **Directory Access** — Explore available years, makes, and models stored in the comprehensive KBB database

### How it works

1. Subscribe to this server
2. Enter your **KBB API Key** (obtained via the KBB Developer Portal)
3. Start researching vehicle values and configurations through natural language

### Who is this for?

- **Car Buyers & Sellers** — quickly check fair market prices before a transaction
- **Auto Dealers** — retrieve trade-in values and configuration data for inventory management
- **Financial Analysts** — monitor automotive market trends and depreciation via AI assistance


## Available Tools (10)
- **get_vehicle_by_vin**: Lookup vehicle information using a VIN
- **get_market_trends**: Retrieve current market trends and pricing shifts
- **get_vehicle_valuation**: Retrieve the estimated market value for a specific vehicle
- **get_vehicle_details**: Get comprehensive configuration and pricing details for a vehicle
- **list_makes_by_year**: List all vehicle makes for a specific year
- **list_models_by_make**: List all vehicle models for a specific year and make
- **list_trim_styles**: g., Sedan, SUV) for the trim.

List specific body styles for a vehicle trim
- **list_vehicle_trims**: List all available trims for a specific vehicle model
- **list_available_years**: Retrieve a list of all years available in the KBB database
- **search_vehicles**: Search for vehicles by make, model, and year


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Kelley Blue Book Valuation** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is the trade-in value for a 2020 Honda Civic with 30,000 miles?"

**🤖 AI Agent:**
> Fetching KBB data... For a 2020 Honda Civic in 'Good' condition with 30k miles in ZIP 90210, the estimated trade-in value is between $18,500 and $20,200.

---

**👤 You:**
> "Search for vehicles models for Toyota in 2023."

**🤖 AI Agent:**
> Retrieving 2023 Toyota models... I found several models including Camry (ID: 123), Corolla (ID: 456), RAV4 (ID: 789), and Tacoma (ID: 012). Which one would you like to explore?


## ❓ FAQ

**Q: How do I get a KBB API Key?**
You must register at the [**KBB Developer Portal**](https://developer.kbb.com/) and request access to the 'InfoDriver Web Service'. Access is typically granted to business entities and automotive professionals.

**Q: Does this tool support international valuations?**
Kelley Blue Book primarily focuses on the North American market (USA and Canada). Valuations are based on regional data from these locations.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/kelley-blue-book-valuation](https://vinkius.com/mcp/kelley-blue-book-valuation)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Kelley Blue Book Valuation** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `kelley-blue-book-valuation` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Kelley Blue Book Valuation** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "kelley-blue-book-valuation": {
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
