# NCDC Climate Data Online MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/ncdc-climate-data-online)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [the-unthinkable](../categories/the-unthinkable.md)

Access authoritative historical weather and climate data via NCDC — track datasets, stations, and climate records directly from your AI agent.

## Description
Connect to the **National Climatic Data Center (NCDC)** API through your AI agent and explore a vast archive of authoritative historical weather and climate data using natural conversation.

### What you can do

- **Dataset Discovery** — List and inspect available climate datasets like GHCND (Daily Summaries) and GSOD (Global Summary of the Day).
- **Climate Records** — Fetch actual data records for specific locations and date ranges, including temperature and precipitation.
- **Station Lookup** — Locate weather stations globally and retrieve their complete metadata and coverage info.
- **Location Intelligence** — Browse location categories and specific IDs (Cities, Countries, States) to filter your data queries.
- **Categorical Analysis** — List high-level data categories and specific types (Max Temp, Snowfall) available in the system.
- **Temporal Flexibility** — Access data classes ranging from hourly to monthly summaries.

### How it works

1. Subscribe to this server
2. Enter your NCDC (NOAA) API Token (get one for free at ncdc.noaa.gov/cdo-web/token)
3. Start exploring historical climate data from Claude, Cursor, or any MCP client

### Who is this for?

- **Researchers & Scientists** — quickly retrieve historical weather data for climate modeling or environmental studies.
- **Data Analysts** — automate the gathering of weather trends for agricultural, energy, or insurance reporting.
- **Educators** — access authoritative public data for classroom projects and climate education.


## Available Tools (10)
- **list_stations**: List weather stations
- **list_locations**: List specific locations
- **get_climate_data**: Retrieve actual climate records
- **get_dataset**: Get specific dataset details
- **get_station**: Get specific station details
- **list_data_categories**: g., Temperature, Precipitation).

List data categories
- **list_data_classes**: g., Hourly, Daily, Monthly).

List data classes
- **list_data_types**: g., Max Temperature, Snowfall).

List specific data types
- **list_datasets**: g., GHCND, GSOD).

List NCDC climate datasets
- **list_location_categories**: g., City, County, State, Country).

List location categories


## 💬 Prompt Examples

Here are some examples of how you can interact with the **NCDC Climate Data Online** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all weather stations in the city of Asheville, NC."

**🤖 AI Agent:**
> I've retrieved the weather stations for Asheville, NC. There are several active stations, including 'ASHEVILLE REGIONAL AIRPORT, NC US' (GHCND:USW00003812) and 'ASHEVILLE 13 S, NC US'. Would you like the detailed metadata for the airport station?

---

**👤 You:**
> "Get daily temperature data for station GHCND:USW00003812 for January 2023."

**🤖 AI Agent:**
> Fetching climate records... For January 2023 at Asheville Regional Airport, the average maximum temperature was 52°F (11°C) and the minimum was 34°F (1°C). There were 15 days with recorded precipitation. Shall I provide the full daily breakdown?

---

**👤 You:**
> "What climate datasets are available for global daily summaries?"

**🤖 AI Agent:**
> Retrieving datasets... For daily summaries, the primary datasets are GHCND (Global Historical Climatology Network Daily) and GSOD (Global Summary of the Day). GHCND is generally recommended for its extensive station coverage. Would you like more info on GHCND?


## ❓ FAQ

**Q: Is the NCDC API Token free?**
Yes! You can request a free API token by providing your email address at https://www.ncdc.noaa.gov/cdo-web/token.

**Q: What is the GHCND dataset?**
GHCND stands for Global Historical Climatology Network - Daily. It is one of the most popular datasets, providing daily climate summaries (temperature, precipitation, etc.) from stations around the world.

**Q: How far back does the data go?**
NCDC archives contain data dating back to the 18th century for some locations, though the availability varies significantly by station and dataset.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/ncdc-climate-data-online](https://vinkius.com/mcp/ncdc-climate-data-online)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **NCDC Climate Data Online** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `ncdc-climate-data-online` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **NCDC Climate Data Online** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "ncdc-climate-data-online": {
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
