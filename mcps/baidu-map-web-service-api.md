# Baidu Map Web Service API MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/baidu-map-web-service-api)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [industry-titans](../categories/industry-titans.md)

Dominant mapping and LBS platform in China — retrieve coordinates, routing, and POI data via AI.

## Description
Empower your AI agent to orchestrate your geographic searches and location-based operations with **Baidu Map**, the premier mapping infrastructure in China. By connecting Baidu Map to your agent, you transform complex geocoding, route planning, and POI (Point of Interest) discovery into a natural conversation. Your agent can instantly convert addresses to coordinates, calculate optimal driving or transit routes, locate users by IP address, and audit local business areas without you ever needing to navigate a technical portal. Whether you are optimizing logistics or conducting market research across Chinese cities, your agent acts as a real-time geographic intelligence assistant, providing accurate and reliable spatial data from a single, unified source.

### What you can do

- **Geocoding Orchestration** — Convert physical addresses into precise latitude and longitude coordinates and vice versa.
- **Route Planning** — Retrieve detailed directions for driving, public transit, walking, and riding between any two points.
- **POI Discovery** — Search for hotels, restaurants, and other points of interest within specific regions or around coordinates.
- **IP Localization** — Monitor and audit user locations based on IP addresses to ensure regional compliance or targeting.
- **Business Area Insights** — Access detailed information about local commercial zones and business surroundings.

### How it works

1. Subscribe to this server
2. Enter your Baidu Map Access Key (AK) and optional Secret Key (SK)
3. Start managing your spatial data through Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Logistics Coordinators** — plan routes and verify addresses for delivery operations through natural language queries.
- **Market Researchers** — analyze business areas and POI density directly from your AI-powered workspace.
- **Travel Planners** — coordinate complex transit itineraries and discover local attractions via a unified AI interface.
- **Baidu Map Power Users** — integrate your existing LBS workflows into your AI-driven daily routines.


## Available Tools (10)
- **direction_driving**: Get driving directions
- **direction_riding**: Get riding directions
- **direction_transit**: Get transit directions
- **direction_walking**: Get walking directions
- **geocoding**: Convert address to coordinates
- **get_business_area**: Get business area info
- **get_suggestion**: Get place suggestions
- **ip_location**: Get location by IP
- **poi_search**: Search for Points of Interest
- **reverse_geocoding**: Convert coordinates to address


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Baidu Map Web Service API** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Find the coordinates for 'Baidu Building' in Beijing."

**🤖 AI Agent:**
> I've geocoded the address. The Baidu Building in Beijing is located at latitude 40.0574, longitude 116.3077. Would you like me to search for nearby points of interest or plan a route there?

---

**👤 You:**
> "Plan a driving route from 'Tsinghua University' to 'Peking University'."

**🤖 AI Agent:**
> I've planned the driving route. The distance is approximately 3.5 km and should take about 10 minutes in current traffic. The route primarily follows Chengfu Road. Would you like a step-by-step breakdown of the directions?

---

**👤 You:**
> "Search for 'Hotels' near these coordinates: 31.2304, 121.4737 (Shanghai)."

**🤖 AI Agent:**
> I've found 5 hotels near your coordinates in Shanghai, including 'The Langham' and 'The Westin Bund Center'. Would you like the addresses and contact numbers for these locations?


## ❓ FAQ

**Q: How do I find my Baidu Map Access Key (AK)?**
Log in to the [Baidu Map Open Platform Console](https://lbsyun.baidu.com/apiconsole/key), create an application, and your AK will be displayed. Ensure the application type is 'Server' for use with this MCP.

**Q: When do I need to provide a Secret Key (SK)?**
You only need to provide an SK if your Baidu Map application has 'SN verification' enabled in the settings. This server will automatically calculate the required signature (sn) for every request if the SK is provided.

**Q: Does this work for international locations?**
Baidu Map specialized services are highly optimized for mainland China. While some international data exists, for global coverage outside of China, other MCP servers like Google Maps or Mapbox might be more appropriate.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/baidu-map-web-service-api](https://vinkius.com/mcp/baidu-map-web-service-api)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Baidu Map Web Service API** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `baidu-map-web-service-api` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Baidu Map Web Service API** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "baidu-map-web-service-api": {
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
