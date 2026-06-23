# Google Air Quality MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/google-air-quality)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [industry-titans](../categories/industry-titans.md)

Universal air quality intelligence — get Google-powered AQI, pollutants, and health advice via AI.

## Description
Equip your AI agent with hyper-local environmental intelligence through the **Google Air Quality** MCP server. This integration provides real-time access to accurate air quality indexes, detailed pollutant concentrations, and actionable health recommendations for specific coordinates. Powered by Google's massive environmental data layer, your agent can retrieve the Universal Air Quality Index (UAQI), identify dominant pollutants (PM2.5, NO2, etc.), and access up to 30 days of historical data. Whether you are building health-tracking tools, planning outdoor events, or researching urban pollution, your agent acts as a dedicated environmental consultant through natural conversation.

### What you can do

- **Real-time AQI Lookup** — Get the current Universal Air Quality Index for any latitude/longitude.
- **Pollutant Breakdown** — Identify dominant pollutants and their concentrations in specific areas.
- **Historical Auditing** — Retrieve up to 720 hours of historical air quality data for trend analysis.
- **Health Advice** — Access tailored recommendations for children, elderly, and sensitive groups.

### How it works

1. Subscribe to this server
2. Enter your Google Maps API Key (ensure Air Quality API is enabled)
3. Start monitoring air quality from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Health-conscious Users** — monitor local conditions to protect themselves and their families.
- **Event Organizers** — verify air quality for outdoor festivals, sports, and gatherings.
- **Real Estate Professionals** — provide environmental insights for specific property locations.
- **Sustainability Researchers** — track urban air quality trends using Google's precise data.


## Available Tools (2)
- **get_air_quality_history**: Get historical air quality data
- **get_current_air_quality**: Get current air quality using Google Maps API


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Google Air Quality** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is the air quality in San Francisco right now?"

**🤖 AI Agent:**
> Retrieving data from Google Air Quality... The current UAQI in San Francisco is 82, which is 'Excellent'. The dominant pollutant is O3. No health restrictions are currently recommended for the general public.

---

**👤 You:**
> "Show me the air quality history for Tokyo for the last 24 hours."

**🤖 AI Agent:**
> I've retrieved the hourly history for Tokyo. The AQI peaked at 65 around 8 AM but has since improved to 78. I can provide the exact pollutant concentrations for each hour if you'd like.

---

**👤 You:**
> "Are there any health warnings for Beijing today?"

**🤖 AI Agent:**
> Analyzing Beijing's conditions... The UAQI is currently 32, categorized as 'Poor'. Dominant pollutant is PM2.5. For children and elderly, it is recommended to avoid prolonged outdoor activities. Would you like the full set of health recommendations?


## ❓ FAQ

**Q: What is the Universal Air Quality Index (UAQI)?**
The UAQI is Google's proprietary index that normalizes air quality measurements globally. It ranges from 0 to 100, where 100 is excellent and 0 is poor.

**Q: Can I check historical air quality for the past week?**
Yes. The `get_air_quality_history` tool allows you to retrieve up to 720 hours (30 days) of historical data for any coordinate.

**Q: Are there specific advice for outdoor sports?**
Yes. The health recommendations provide specific guidance for athletes and individuals performing intense physical activities outdoors based on the pollutant levels.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/google-air-quality](https://vinkius.com/mcp/google-air-quality)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Google Air Quality** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `google-air-quality` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Google Air Quality** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "google-air-quality": {
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
