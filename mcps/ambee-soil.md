# Ambee Soil MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/ambee-soil)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [the-unthinkable](../categories/the-unthinkable.md)

Access real-time soil data via Ambee — monitor soil moisture, temperature, and properties globally for precision agriculture from any AI agent.

## Description
Connect your **Ambee Soil API** to any AI agent and take full control of real-time soil moisture tracking, temperature monitoring, historical trend analysis, and soil property assessment through natural conversation.

### What you can do

- **Real-Time Soil Data** — Get current soil moisture and temperature for any global location
- **Historical Trends** — Analyze soil moisture and temperature patterns over past days, weeks, or months
- **Radius Analysis** — Retrieve soil data for multiple points within a specified radius for spatial analysis
- **Soil Properties** — Access detailed soil composition including texture, organic carbon, pH, and bulk density
- **Grid Mapping** — Generate structured gridded soil data for GIS integration and precision agriculture mapping

### How it works

1. Subscribe to this server
2. Enter your Ambee Soil API key (from the developer dashboard)
3. Start analyzing soil conditions from Claude, Cursor, or any MCP-compatible client

No more manual soil sensor deployment or complex data extraction. Your AI acts as a dedicated soil scientist and agronomist assistant.

### Who is this for?

- **Farmers** — monitor soil moisture for irrigation scheduling and crop health assessment
- **Agronomists** — analyze soil properties, track historical trends, and advise on soil management
- **Researchers** — access global soil datasets for climate studies and agricultural research
- **Landscapers** — check soil conditions for planting optimization and maintenance planning


## Available Tools
- **get_grid_soil**: Returns gridded data points suitable for creating soil condition maps, GIS analysis, and spatial interpolation. Essential for precision agriculture mapping, variable rate application planning, and geospatial soil analysis. AI agents should use this when users ask "generate a soil moisture grid for mapping", "get gridded soil data for my field", or need structured spatial soil data for GIS integration.

Get soil data on a structured grid for spatial analysis and mapping
- **get_historical_soil**: Essential for analyzing soil condition trends, seasonal patterns, drought assessment, and long-term irrigation planning. AI agents should reference this when users ask "show me soil moisture trends over the past 30 days", "what was the soil temperature last week", or need historical soil data for agricultural analysis.

Get historical soil moisture and temperature data for trend analysis
- **get_latest_soil**: Essential for irrigation planning, crop monitoring, soil health assessment, and precision agriculture. AI agents should use this when users ask "what is the soil moisture at my farm", "check current soil temperature", or need immediate soil condition data for agricultural decision making.

Get real-time soil moisture and temperature for a specific location
- **get_soil_by_radius**: Returns an array of soil readings across the area, enabling spatial analysis of soil conditions. Essential for regional soil assessment, field variability analysis, and precision agriculture zone mapping. AI agents should use this when users ask "show me soil conditions within 10km of my location", "get soil data for my entire farm area", or need spatial soil moisture distribution analysis.

Get soil data for multiple points within a radius of a location
- **get_soil_properties**: Essential for soil classification, crop suitability analysis, fertilizer planning, and long-term soil health monitoring. AI agents should reference this when users ask "what is the soil type and pH at my location", "show me soil organic carbon content", or need comprehensive soil property data for agricultural planning.

Get detailed soil physical and chemical properties for a location


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Ambee Soil** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is the current soil moisture and temperature at my farm in Iowa (41.8780, -93.0977)?"

**🤖 AI Agent:**
> Fetching real-time soil data for Iowa coordinates... Current conditions: Soil Moisture is 32.4% (moderate, adequate for corn growth stage). Soil Temperature is 18.2°C (64.8°F), ideal for nutrient uptake. Data timestamp: 2026-04-07 14:00 UTC. Based on these readings, irrigation is not immediately required but should be monitored over the next 48 hours. Would you like historical trends for the past 30 days to see moisture patterns?

---

**👤 You:**
> "Show me soil moisture trends over the last 60 days for my location."

**🤖 AI Agent:**
> Analyzing 60-day soil moisture history... Day 1-15: Average 38% (post-rainfall recovery). Day 16-30: Dropped to 28% (dry spell). Day 31-45: Rebounded to 35% (irrigation applied). Day 46-60: Currently stabilizing at 32%. Overall trend shows a gradual drying pattern with one successful irrigation intervention. Soil moisture is currently in the moderate range. Recommended action: Schedule irrigation within 5-7 days if no rainfall is forecasted. Would you like a comparison with historical averages for this time of year?

---

**👤 You:**
> "What are the soil properties at my vineyard location? I need to know the pH and organic carbon."

**🤖 AI Agent:**
> Retrieving soil properties for your vineyard... Soil Composition: Sandy Loam (Sand: 62%, Silt: 24%, Clay: 14%). pH Level: 6.4 (slightly acidic, optimal for grape cultivation). Organic Carbon: 1.8% (good fertility level). Bulk Density: 1.42 g/cm3. Cation Exchange Capacity: 14.2 cmol/kg. Water Holding Capacity: 18%. Assessment: Your soil is well-suited for viticulture with good drainage and adequate nutrient retention. The slightly acidic pH is ideal for most grape varietals. Consider adding organic matter to boost carbon content above 2%. Would you like crop suitability recommendations based on these soil properties?


## ❓ FAQ

**Q: Can my AI check real-time soil moisture and temperature for my farm location?**
Yes! Use the `get_latest_soil` tool with your farm latitude and longitude coordinates. The API returns current soil moisture percentage and soil temperature in Celsius. This data is updated in near real-time using satellite and sensor fusion models, making it perfect for daily irrigation decisions and crop health monitoring.

**Q: How do I get historical soil moisture trends to analyze drought patterns?**
Use the `get_historical_soil` tool with your coordinates and the number of days you want to analyze (e.g., 30, 60, or 90 days). This returns daily soil moisture and temperature readings that you can use to identify drying trends, assess drought severity, and plan irrigation schedules based on historical patterns.

**Q: What soil properties are available and how can they help with crop planning?**
Use the `get_soil_properties` tool to access detailed soil composition data including sand/silt/clay percentages, organic carbon content, bulk density, pH, and cation exchange capacity (CEC). These properties help determine soil texture classification, drainage capacity, nutrient retention, and optimal crop selection for your land.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/ambee-soil](https://vinkius.com/mcp/ambee-soil)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Ambee Soil** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `ambee-soil` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Ambee Soil** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "ambee-soil": {
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
