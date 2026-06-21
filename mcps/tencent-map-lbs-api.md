# Tencent Map LBS API MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/tencent-map-lbs-api)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [industry-titans](../categories/industry-titans.md)

China's leading LBS platform — essential for WeChat Miniapps, providing precise mapping, routing, and POI data.

## Description
Empower your AI agent to orchestrate your geographic operations and location-based services with **Tencent Map** (腾讯地图), the dominant mapping infrastructure for the WeChat ecosystem. By connecting Tencent Map to your agent, you transform complex geocoding, route planning, and POI discovery into a natural conversation. Your agent can instantly convert addresses to coordinates, calculate optimal driving or transit routes, locate users by IP address, and audit administrative districts without you ever needing to navigate a technical console. Whether you are optimizing logistics for a WeChat Miniapp or conducting market research across Chinese cities, your agent acts as a real-time geographic intelligence assistant, providing accurate results from a single, unified source.

### What you can do

- **Geocoding Orchestration** — Convert physical addresses into precise latitude and longitude coordinates and vice versa.
- **Route Planning** — Retrieve detailed directions for driving, public transit, walking, and bicycling between any two points.
- **POI Discovery** — Search for hotels, restaurants, and other points of interest within specific boundaries or keywords.
- **IP Localization** — Monitor and audit user locations based on IP addresses to ensure regional accuracy.
- **Administrative Insights** — Access the full list of administrative districts in China for regional classification.

### How it works

1. Subscribe to this server
2. Enter your Tencent Map API Key and optional Secret Key (SK)
3. Start managing your LBS data through Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Miniapp Developers** — verify locations and plan routes for WeChat-integrated applications through natural language.
- **Logistics Coordinators** — optimize delivery routes and audit addresses directly from your AI-powered workspace.
- **Market Researchers** — analyze POI density and regional distribution via a unified AI interface.
- **Tencent Map Power Users** — integrate your existing mapping workflows into your AI-driven daily routines.


## Available Tools
- **direction_bicycling**: Get bicycling directions
- **direction_driving**: Get driving directions
- **direction_transit**: Get transit directions
- **direction_walking**: Get walking directions
- **geocoding**: Convert address to coordinates
- **get_district_list**: Get administrative districts
- **ip_location**: Get location by IP
- **poi_search**: Search for Points of Interest
- **poi_suggestion**: Get place suggestions
- **reverse_geocoding**: Convert coordinates to address


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Tencent Map LBS API** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Find the coordinates for 'Tencent Seafront Towers' in Shenzhen."

**🤖 AI Agent:**
> I've geocoded the address. The Tencent Seafront Towers in Shenzhen are located at latitude 22.5229, longitude 113.9351. Would you like me to plan a driving route there or search for nearby restaurants?

---

**👤 You:**
> "Search for 'Coffee' near 22.5229, 113.9351 within 1000 meters."

**🤖 AI Agent:**
> I've found 8 coffee shops within 1000 meters of those coordinates, including 'Starbucks' and 'Luckin Coffee'. Would you like the full list with addresses and contact numbers?

---

**👤 You:**
> "What is the best transit route from Shenzhen University to the Airport?"

**🤖 AI Agent:**
> I've planned the transit route. The best option is taking Metro Line 11 directly, which takes about 35 minutes. Would you like a step-by-step breakdown of the transit directions?


## ❓ FAQ

**Q: How do I find my Tencent Map API Key?**
Log in to the [Tencent Map Open Platform Console](https://lbs.qq.com/dev/console/key/manage), create an application, and your Key will be displayed. You can also configure the optional Secret Key (SK) in the key settings.

**Q: When should I provide the Secret Key (SK)?**
Provide the SK if you have enabled 'Signature Verification' (sig) in your Tencent Map key settings. This server will automatically calculate the MD5 signature for every request if the SK is provided.

**Q: Can I use this for international geocoding?**
Tencent Map is highly optimized for mainland China, Hong Kong, and Macau. While some international coverage exists, results outside these regions may be less detailed than local providers.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/tencent-map-lbs-api](https://vinkius.com/mcp/tencent-map-lbs-api)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Tencent Map LBS API** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `tencent-map-lbs-api` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Tencent Map LBS API** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "tencent-map-lbs-api": {
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
