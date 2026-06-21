# Climatiq Carbon Calculations MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/climatiq-carbon-calculations)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [data-analytics](../categories/data-analytics.md)

Calculate carbon footprints via Climatiq — search thousands of emission factors and estimate emissions for any activity.

## Description
Connect your AI agent to **Climatiq**, the leading platform for carbon calculation and emission factor data. This integration allows you to accurately estimate carbon footprints for everything from energy usage and transportation to procurement and industry classifications.

### What you can do

- **Factor Discovery** — Search through a massive database of scientifically validated emission factors by sector, region, and year
- **Precise Estimation** — Calculate CO2e for specific activities by providing parameters like weight, volume, or energy usage
- **Bulk Processing** — Perform up to 100 calculations in a single request for efficient data analysis
- **Industry Alignment** — Estimate emissions using standard classification codes like ISIC, NACE, and NAICS
- **Metadata Insights** — Explore available sectors, regions, categories, and units to build structured sustainability reports

### How it works

1. Subscribe to this server
2. Enter your **Climatiq API Key** (Bearer Token from the Climatiq dashboard)
3. Start calculating sustainability metrics directly through natural conversation

### Who is this for?

- **Sustainability Teams** — automate carbon reporting and footprint calculations
- **Supply Chain Managers** — analyze the environmental impact of logistics and procurement
- **Product Owners** — build carbon-aware applications using verified scientific data


## Available Tools
- **batch_estimate_emissions**: Provide calculations as a JSON array string.

Perform up to 100 emission calculations in a single request
- **estimate_by_classification**: Provide parameters as a JSON string.

Calculate emissions using industry classification codes (ISIC, NACE, etc.)
- **estimate_emissions**: Provide parameters as a JSON string.

Calculate carbon emissions for a specific activity
- **list_categories**: Retrieve a list of all available emission categories
- **list_regions**: Retrieve a list of all supported regions
- **list_sectors**: Retrieve a list of all available emission sectors
- **list_sources**: Retrieve a list of all data sources for emission factors
- **list_units**: ) accepted by the API.

Retrieve a list of all supported units of measure
- **list_years**: Retrieve a list of all years for which emission factors are available
- **search_emission_factors**: Search for emission factors in the Climatiq database


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Climatiq Carbon Calculations** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Search for electricity emission factors in the UK for 2023."

**🤖 AI Agent:**
> Searching Climatiq... I found several factors, including 'Electricity supplied from grid' (Activity ID: electricity-supply_grid-source_residual_mix). Would you like to use this for an estimation?

---

**👤 You:**
> "Estimate emissions for activity 'passenger_vehicle-vehicle_type_car-fuel_source_petrol-engine_size_na-vehicle_age_na-vehicle_standard_na' with 100 km distance."

**🤖 AI Agent:**
> Calculated! Traveling 100 km in this passenger vehicle results in approximately 17.5 kg of CO2e.


## ❓ FAQ

**Q: Where do I get a Climatiq API Key?**
You can sign up for a developer account at the [**Climatiq Dashboard**](https://www.climatiq.io/dashboard) to generate your API Bearer Token. They offer a free tier for testing and small-scale usage.

**Q: Which carbon equivalents are calculated?**
The API primarily returns CO2e (Carbon Dioxide Equivalent), which includes the combined global warming potential of various greenhouse gases, expressed in a single metric (usually kg or tonnes).


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/climatiq-carbon-calculations](https://vinkius.com/mcp/climatiq-carbon-calculations)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Climatiq Carbon Calculations** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `climatiq-carbon-calculations` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Climatiq Carbon Calculations** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "climatiq-carbon-calculations": {
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
