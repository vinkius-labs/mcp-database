# BlaBlaCar MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/blablacar)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

AI carpool search: find rides, compare prices, and book shared journeys via agents.

## Description
### What you can do

Connect AI agents to the world's largest carpooling network for affordable, sustainable travel:

- **Search carpool rides** between any cities or GPS coordinates worldwide
- **Compare prices and schedules** across multiple drivers and departure times
- **Review driver profiles** with ratings, verification status, and vehicle details
- **Find bus trips** on BlaBlaCar Bus routes for longer distances
- **Search with flexible dates** to find cheapest travel days
- **International rides** across borders with country-specific filtering
- **Radius-based searches** for flexible pickup location options

### How it works

1. **Get your BlaBlaCar API key** from the developer portal
2. **Ask your AI agent** to search rides, compare options, or check driver profiles
3. **Natural language commands** replace manual website searches
4. **Instant comparisons** across dozens of available rides and schedules

### Who is this for?

Ideal for **budget travelers**, **students**, **eco-conscious commuters**, **travel planners**, and **digital nomads**. Let AI agents find the cheapest rides, compare schedules across dates, verify driver credibility, and plan multi-city carpool routes. Perfect for anyone taking 2+ intercity trips monthly who wants to save 40-60% vs trains while reducing carbon footprint through shared transportation.


## Available Tools
- **get_driver_profile**: Use this to verify driver credibility and read passenger reviews before booking a ride. Requires the driver user ID from a trip result.

Get driver profile and ratings on BlaBlaCar
- **get_trip_details**: Use this before booking to verify driver credibility, vehicle comfort, and exact pickup location.

Get complete details of a specific BlaBlaCar trip including driver and vehicle info
- **search_bus_trips**: BlaBlaCar operates both carpooling and bus services. Bus trips are operated by professional drivers on fixed routes. Returns bus departure/arrival times, prices, and availability. Use this for longer distance or when carpool options are limited.

Search BlaBlaCar Bus trips between two locations
- **search_flexible_dates**: Much larger result set than exact-date search. Useful when travel dates are not fixed and user wants to compare prices/availability across multiple days. Returns up to 50 results spanning several days.

Search carpool trips with flexible dates around a target date
- **search_international_trips**: Requires origin/destination coordinates plus country codes (e.g., FR, DE, ES, IT, PT). Returns all available international rides with driver details and pricing. Use this for trips crossing national borders.

Search international carpool trips between two countries on BlaBlaCar
- **search_trips_by_city**: More user-friendly than coordinate-based search. Returns all matching trips with departure/arrival points, times, prices, driver ratings, and available seats. Best for general city-to-city searches without needing exact coordinates.

Search carpool trips between two city names on BlaBlaCar
- **search_trips**: Requires latitude,longitude format for both points. Returns trip details including departure/arrival cities, times, price, driver info, and available seats. Use this for precise location-based searches when you know exact coordinates.

Search carpool trips between two GPS coordinates on BlaBlaCar
- **search_trips_with_radius**: Useful when exact pickup/dropoff locations are flexible. Larger radius returns more options but may require additional travel to reach departure points. Returns all rides within the specified radius.

Search carpool trips with flexible radius around coordinates


## 💬 Prompt Examples

Here are some examples of how you can interact with the **BlaBlaCar** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Find carpool rides from Paris to Lyon next Friday for 2 people"

**🤖 AI Agent:**
> I'll search all available carpool rides between Paris and Lyon for your date and show you the best options.

---

**👤 You:**
> "What's the cheapest day to travel from São Paulo to Rio next week?"

**🤖 AI Agent:**
> I'll search with flexible dates to compare prices across the entire week.

---

**👤 You:**
> "Show me both carpool and bus options from Madrid to Barcelona this weekend"

**🤖 AI Agent:**
> I'll search both carpool rides and BlaBlaCar Bus trips so you can compare all transportation options.


## ❓ FAQ

**Q: Can I book rides directly through this MCP server?**
This MCP server provides search, comparison, and driver verification tools. Booking requires redirecting to the BlaBlaCar website or app via the trip link returned in search results. The agent can find the perfect ride, but final booking happens on BlaBlaCar's platform for security.

**Q: Does this work for international trips between countries?**
Yes! BlaBlaCar operates across 22 countries including France, Spain, Italy, Germany, Brazil, Mexico, India, and more. The search_international_trips tool lets you filter by country codes for cross-border rides. Perfect for Europe where BlaBlaCar has extensive international networks.

**Q: How do I get a BlaBlaCar API key?**
BlaBlaCar provides API access through partnerships. Contact BlaBlaCar's developer relations team or check if you have access through aggregator services like TripGo. For testing, you can explore public API documentation and request access via their developer portal.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/blablacar](https://vinkius.com/mcp/blablacar)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **BlaBlaCar** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `blablacar` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **BlaBlaCar** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "blablacar": {
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
