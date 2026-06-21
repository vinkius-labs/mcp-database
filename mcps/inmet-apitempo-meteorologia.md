# INMET (Apitempo - Meteorologia) MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/inmet-apitempo-meteorologia)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [government-public-data](../categories/government-public-data.md)

Access official Brazilian meteorological data from INMET — stations, forecasts, and GOES-16 satellite imagery.

## Description
Connect to the **INMET (Instituto Nacional de Meteorologia)** API to retrieve comprehensive weather data across Brazil. This server allows AI agents to query a vast network of automatic and manual stations, providing precise atmospheric measurements and forecasts.

### What you can do

- **Meteorological Stations** — List all automatic (T) and manual (M) stations across the Brazilian territory.
- **Historical & Real-time Data** — Fetch daily or hourly measurements (temperature, humidity, pressure) for specific station IDs.
- **Regional Analysis** — Query data for all stations within specific Brazilian regions (N, NE, CO, SE, S) for a given date.
- **Weather Forecasts** — Get detailed forecasts for cities using IBGE codes or retrieve all available forecasts at once.
- **Satellite Imagery** — Access the latest GOES-16 satellite metadata and image URLs for visual weather monitoring.

### How it works

1. Subscribe to this server
2. Enter your INMET API Token (if required)
3. Start querying weather patterns directly from your AI assistant

### Who is this for?

- **Data Scientists & Researchers** — analyze climate trends and historical weather patterns in Brazil.
- **Logistics & Agriculture** — monitor local weather conditions and forecasts to optimize operations.
- **Developers** — integrate official Brazilian meteorological data into applications without complex API handling.


## Available Tools
- **get_all_forecasts**: Get weather forecasts for all supported cities
- **get_forecast_by_city**: Get weather forecast for a specific city
- **get_meteorological_data_by_date**: Get meteorological data by date for a station
- **get_meteorological_data_by_region**: Get meteorological data for all stations in a specific region
- **get_satellite_images**: Get latest GOES-16 satellite images
- **get_station_data_daily**: Get daily meteorological data for a specific station
- **get_station_data_hourly**: Get hourly data for a specific station and time
- **list_stations**: List meteorological stations by type


## 💬 Prompt Examples

Here are some examples of how you can interact with the **INMET (Apitempo - Meteorologia)** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all automatic weather stations in Brazil."

**🤖 AI Agent:**
> I've retrieved the list of automatic stations. There are hundreds across Brazil, such as A001 (Brasília) and A601 (Rio de Janeiro). Would you like to see data for a specific station ID?

---

**👤 You:**
> "What is the weather forecast for city code 3304557?"

**🤖 AI Agent:**
> Fetching forecast for Rio de Janeiro (3304557)... The forecast indicates clear skies with a maximum of 32°C and a minimum of 22°C for today. Would you like the hourly breakdown?

---

**👤 You:**
> "Show me the latest satellite images from GOES-16."

**🤖 AI Agent:**
> I've accessed the latest GOES-16 satellite data. I have several URLs for different channels (Infrared, Water Vapor, Visible). Which one would you like to view?


## ❓ FAQ

**Q: How can I get the weather forecast for a specific city in Brazil?**
You can use the `get_forecast_by_city` tool by providing the city's IBGE code. The agent will return detailed forecast information including temperature and conditions.

**Q: Can I access real-time satellite imagery of Brazil?**
Yes! Use the `get_satellite_images` tool to retrieve the latest metadata and URLs for GOES-16 satellite images covering the Brazilian territory.

**Q: How do I find the ID of a meteorological station?**
Use the `list_stations` tool with the type 'T' for automatic or 'M' for manual stations. This will provide a list of all stations and their respective IDs.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/inmet-apitempo-meteorologia](https://vinkius.com/mcp/inmet-apitempo-meteorologia)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **INMET (Apitempo - Meteorologia)** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `inmet-apitempo-meteorologia` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **INMET (Apitempo - Meteorologia)** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "inmet-apitempo-meteorologia": {
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
