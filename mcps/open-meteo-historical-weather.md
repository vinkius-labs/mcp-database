# Open-Meteo Historical Weather MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/open-meteo-historical-weather)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [data-analytics](../categories/data-analytics.md)

Unlock 84 years of global weather history (1940–present): temperature, precipitation, wind, and snow data for any coordinate — the ultimate climate research companion.

## Description
Access **84 years of continuous weather records** from 1940 to today for any location on Earth.

### What you can do
- **Historical Hourly** — Temperature, humidity, precipitation, snowfall, weather codes, and wind for any past date range
- **Historical Daily** — Max/min temperatures, precipitation totals, sunshine duration, and dominant wind patterns
- **Temperature Trends** — Dedicated tool for long-term climate trend analysis with apparent temperature data

### Who is this for?
Climate researchers, agricultural analysts, insurance underwriters, real estate developers, and data scientists studying long-term weather patterns.


## Available Tools
- **get_historical_weather**: Provide latitude, longitude, start_date and end_date in YYYY-MM-DD format. Covers 84 years of global data.

Get historical weather for any date range (1940–present)
- **get_historical_daily**: Get historical daily weather aggregates
- **get_historical_temperature**: Includes hourly temperature, apparent temperature, and dewpoint.

Get historical temperature trends for climate analysis


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Open-Meteo Historical Weather** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What was the weather in London on D-Day, June 6, 1944?"

**🤖 AI Agent:**
> 🏛️ **London — June 6, 1944**

Max temp: 16.2°C | Min: 10.8°C
Precipitation: 2.1mm (light rain)
Wind: 28 km/h from the west
Cloud cover: Heavy overcast

Historical records confirm the famously poor weather conditions that nearly delayed the Normandy invasion.

---

**👤 You:**
> "Compare average temperatures in São Paulo between 1950 and 2020"

**🤖 AI Agent:**
> 📊 **São Paulo Temperature Trend (70 years)**

1950s avg: 19.2°C
1980s avg: 19.8°C
2010s avg: 20.6°C

A clear warming trend of +1.4°C over 70 years, consistent with global urban heat island effects.

---

**👤 You:**
> "How much rain fell in Mumbai during the 2005 flood?"

**🤖 AI Agent:**
> 🌧️ **Mumbai — July 26, 2005**

Daily precipitation: 944mm (one of the highest single-day totals ever recorded in India)
Hourly peak: 190mm between 14:00-15:00

This catastrophic flood event displaced over 20 million people.


## ❓ FAQ

**Q: How far back does the historical data go?**
All the way to **January 1, 1940** — that's 84 years of continuous, hourly global weather data powered by ERA5 reanalysis from ECMWF.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/open-meteo-historical-weather](https://vinkius.com/mcp/open-meteo-historical-weather)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Open-Meteo Historical Weather** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `open-meteo-historical-weather` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Open-Meteo Historical Weather** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "open-meteo-historical-weather": {
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
