# NCEI Climate Data Online (NOAA Archive) MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/ncei-climate-data-online-noaa-archive)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [government-public-data](../categories/government-public-data.md)

Access historical weather and climate data from NOAA's National Centers for Environmental Information archive.

## Description
Connect your AI agent to the **NCEI Climate Data Online** archive and explore decades of global environmental records through natural language.

### What you can do

- **Datasets & Categories** — Browse primary data groupings like Daily Summaries (GHCND) or Global Summary of the Month (GSOM) using `list_datasets` and `list_datacategories`.
- **Location Discovery** — Find specific geopolitical entities, cities, or zip codes using `list_locations` and `list_locationcategories` to narrow your search.
- **Station Metadata** — Identify weather observing platforms and stations worldwide with `list_stations` to find the exact source of climate records.
- **Data Type Inspection** — Query specific climate variables such as precipitation (PRCP), average temperature (TAVG), or snow depth using `list_datatypes`.
- **Historical Analysis** — Retrieve precise climate observations for specific timeframes and locations to power research or environmental reporting.

### How it works

1. Subscribe to this server
2. Request a free API Token from the NOAA NCEI portal
3. Start querying historical weather data directly from your AI client

### Who is this for?

- **Data Scientists & Researchers** — quickly locate and verify available climate datasets without manual API exploration
- **Environmental Consultants** — retrieve station metadata and location-specific weather history for impact reports
- **Developers** — integrate reliable, government-backed climate data into applications using natural language queries


## Available Tools (10)
- **list_datacategories**: List general types of data used to group similar data types
- **get_data**: Annual/Monthly data limited to 10-year range; other data limited to 1-year range.

Fetch actual observations and ancillary attributes
- **list_datatypes**: List specific types of data (e.g., TAVG, PRCP)
- **list_datasets**: g., Daily Summaries, Global Summary of the Month).

Find information about available NCEI datasets
- **list_locationcategories**: List groupings of similar locations (e.g., Countries, States)
- **list_locations**: List geopolitical entities or bounding areas
- **list_stations**: List weather observing platforms
- **search_data**: Discover data based on temporal and spatial parameters
- **search_datasets**: Discover datasets based on temporal and spatial parameters
- **get_service_data**: Access subset data in multiple formats


## 💬 Prompt Examples

Here are some examples of how you can interact with the **NCEI Climate Data Online (NOAA Archive)** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all available climate datasets from NCEI."

**🤖 AI Agent:**
> I've retrieved the available datasets. Key archives include 'Daily Summaries' (GHCND), 'Global Summary of the Month' (GSOM), and 'Precipitation Hourly' (PRECIP_HLY). Which one would you like to explore further?

---

**👤 You:**
> "Find weather stations located in London, UK."

**🤖 AI Agent:**
> Searching for stations in London... I found several platforms, including 'LONDON HEATHROW' (ID: GHCND:UKM00003772) and 'LONDON WEATHER CENTER'. Would you like to see the data types available for Heathrow?

---

**👤 You:**
> "What are the data types available for the Daily Summaries dataset?"

**🤖 AI Agent:**
> For the Daily Summaries (GHCND) dataset, available types include PRCP (Precipitation), SNOW (Snowfall), TAVG (Average Temperature), TMAX (Maximum Temperature), and TMIN (Minimum Temperature).


## ❓ FAQ

**Q: How do I find the specific ID for a weather station in a certain city?**
You can use the `list_stations` tool and provide a `locationid`. To find the correct location ID first, use the `list_locations` tool to search by city or state name.

**Q: What is the difference between a Data Category and a Data Type?**
Data Categories (retrieved via `list_datacategories`) are broad groups like 'Temperature' or 'Precipitation'. Data Types (retrieved via `list_datatypes`) are specific codes like 'TMAX' (Maximum temperature) or 'PRCP' (Precipitation amount).

**Q: Can I see what datasets are available for a specific date range?**
Yes, the `list_datasets` tool accepts `startdate` and `enddate` parameters. This allows you to filter the archive for datasets that have coverage during your period of interest.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/ncei-climate-data-online-noaa-archive](https://vinkius.com/mcp/ncei-climate-data-online-noaa-archive)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **NCEI Climate Data Online (NOAA Archive)** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `ncei-climate-data-online-noaa-archive` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **NCEI Climate Data Online (NOAA Archive)** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "ncei-climate-data-online-noaa-archive": {
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
