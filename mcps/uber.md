# Uber MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/uber)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [industry-titans](../categories/industry-titans.md)

AI ride management: estimate prices, track trips, and manage locations via agents.

## Description
### What you can do

Connect your AI agents to the Uber platform for seamless ride management and trip planning:

- **Get available ride products** (UberX, Black, Comfort) at any location
- **Estimate prices** across all ride types before booking
- **Compare pickup times** to choose the fastest option
- **View complete trip history** with pricing and route data
- **Save and manage favorite places** (Home, Work, custom locations)
- **Autocomplete place searches** for accurate pickup/dropoff coordinates

### How it works

1. **Connect your Uber account** via Server Token from the Uber Developer Portal
2. **Ask your AI agent** to estimate rides, check history, or manage saved locations
3. **No app navigation needed** — natural language commands execute all operations
4. **Instant insights** on pricing and availability across all Uber products

### Who is this for?

Perfect for **frequent travelers**, **executive assistants**, **travel planners**, and **corporate teams** managing business transportation. Let AI agents handle ride planning, expense tracking via trip history, and location management. Ideal for professionals taking 10+ Uber rides monthly who want streamlined booking workflows and cost comparison automation.


## Available Tools
- **add_saved_place**: Requires alias name, latitude, and longitude. Optionally include a full address string. The alias can be home, work, or any custom string. Returns the saved place details.

Save a new place for the authenticated Uber user
- **get_trip_history**: Returns trip date, start/end locations, product used, distance, and price. Use this to review past rides, calculate expenses, or find a previous trip details.

Get trip history for the authenticated Uber user
- **get_user_profile**: Use this to verify authentication and confirm which Uber account is connected.

Get the authenticated Uber user profile
- **get_place_autocomplete**: Requires current user location to bias results. Returns place descriptions and structured address components. Use this to help users select valid pickup/dropoff locations before requesting rides.

Autocomplete place predictions for Uber locations
- **get_price_estimate**: Prices are in local currency. Use this to compare costs across different Uber ride types before booking.

Get price estimate for an Uber ride between two locations
- **get_products**: ) available at the specified latitude/longitude. Returns product IDs, display names, capacity, and descriptions. Use this to see which ride options are available before requesting a ride or price estimate.

Get available Uber products at a location
- **get_ride_estimate**: More specific than price estimates as it targets one product. Use this to get exact pricing before requesting a ride.

Get detailed ride estimate for a specific Uber product
- **get_saved_places**: Returns place aliases, addresses, and coordinates. Use this to quickly reference saved locations for ride requests or price estimates without typing addresses.

List saved places for the authenticated Uber user
- **get_time_estimate**: Use this to compare how quickly different Uber services can pick you up. Lower times mean faster pickups.

Get estimated pickup time for Uber at a location


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Uber** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Estimate the price for an UberX from my home to the airport at 3pm tomorrow"

**🤖 AI Agent:**
> I'll get price estimates for all Uber products between your locations right away.

---

**👤 You:**
> "Show me my last 10 Uber trips with total spending"

**🤖 AI Agent:**
> I'll pull your recent trip history and compile the spending summary.

---

**👤 You:**
> "What Uber products are available at my current location and how fast can they pick me up?"

**🤖 AI Agent:**
> I'll check available products and pickup times at your location.


## ❓ FAQ

**Q: Can this MCP server book rides automatically?**
This MCP server provides price estimates, time estimates, product availability, and trip history. Direct ride booking requires additional Uber API permissions (Requests API) available only to approved enterprise partners. Use this server for planning and comparison workflows.

**Q: What Uber API permissions do I need?**
You need a Server Token from the Uber Developer Portal with access to: Products, Price Estimates, Time Estimates, History, User Profile, and Places endpoints. These are available in the standard developer tier without special approval.

**Q: Does this work with Uber Eats deliveries?**
This MCP server focuses on Uber ride-sharing products (UberX, Black, Comfort, etc.). For Uber Eats merchant/delivery operations, a separate integration would be needed. Contact Uber for Eats API access.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/uber](https://vinkius.com/mcp/uber)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Uber** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `uber` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Uber** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "uber": {
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
