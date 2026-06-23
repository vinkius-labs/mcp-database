# Cabify MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/cabify)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [finance-accounting](../categories/finance-accounting.md)

AI ride management for business: book rides, track trips, and manage corporate mobility via agents.

## Description
### What you can do

Connect AI agents to the Cabify Business platform for enterprise mobility management:

- **Get price estimates** across all Cabify tiers (Lite, Executive, Taxi)
- **Compare trip durations** with real-time traffic data
- **Request rides directly** with pickup and dropoff coordinates
- **Track active rides** with driver info, vehicle details, and live ETA
- **Cancel rides** when plans change
- **View complete ride history** with business expense tracking
- **Manage saved locations** for frequent business destinations
- **Check available service tiers** at any location in Spain and LATAM

### How it works

1. **Connect your Cabify Business account** via API key from Cabify Empresas portal
2. **Ask your AI agent** to estimate rides, book trips, or check ride history
3. **No app navigation needed** — natural language commands execute all operations
4. **Business expense tracking** integrated with your corporate Cabify account

### Who is this for?

Perfect for **business travelers**, **corporate assistants**, **travel managers**, **HR coordinators**, and **companies** using Cabify Empresas in Spain, Portugal, and Latin America. Let AI agents handle employee transportation, manage business travel expenses via ride history, and coordinate executive mobility. Ideal for companies with 10+ monthly corporate rides who want streamlined booking workflows, centralized expense tracking, and automated ride management across multiple offices.


## Available Tools (9)
- **add_saved_location**: Common use cases: save office addresses, frequent client locations, hotels, airports. Returns the saved location details including the new location ID. Use this to build a library of frequently used destinations for faster ride booking.

Save a new location for the Cabify account
- **cancel_ride**: Cancellation policies vary based on ride status - cancellations after driver assignment may incur fees depending on Cabify Empresas policy. Use this to cancel rides that were booked by mistake or are no longer needed.

Cancel an existing Cabify ride request
- **get_available_products**: Returns product IDs, names, descriptions, capacity, and features. Use this to see which service options are available before requesting estimates or booking rides.

Get available Cabify service tiers at a location
- **get_price_estimate**: Prices are in local currency (EUR for Spain, local currency for LATAM). Use this to compare costs across different Cabify service tiers before booking.

Get price estimate for a Cabify ride between two locations
- **get_ride_details**: Use this to track your active ride or review past trip details.

Get details of a specific Cabify ride
- **get_ride_history**: Returns ride date, status, origin/destination, product type, driver, cost, and business expense category. Use this to review past rides, calculate business expenses, or find previous trip details.

Get ride history for the Cabify Business account
- **get_saved_locations**: Returns location IDs, names, addresses, and coordinates. Use this to quickly reference saved locations for ride requests without typing full addresses. Common for frequent business destinations.

Get saved locations for the Cabify account
- **get_time_estimate**: Accounts for current traffic conditions and typical route times. Use this to plan schedules and compare route efficiency across different pickup/dropoff points.

Get estimated trip duration for a Cabify ride
- **request_ride**: Requires origin and destination coordinates. Optionally specify product ID (from get_available_products), pickup address, and dropoff address for clarity. Returns the ride ID, driver assignment status, and estimated pickup time. Use this to book a ride after confirming price and availability.

Request a new Cabify ride


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Cabify** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Get me a price estimate from Madrid Airport to our office in Gran Vía for a Cabify Executive"

**🤖 AI Agent:**
> I'll get cost estimates for all available Cabify products between those locations.

---

**👤 You:**
> "Book a Cabify from the hotel to the conference center for 9am tomorrow"

**🤖 AI Agent:**
> I'll book the ride and send you the confirmation with driver details.

---

**👤 You:**
> "Show me all Cabify rides from last month with total business expenses"

**🤖 AI Agent:**
> I'll pull your ride history and compile the monthly expense summary.


## ❓ FAQ

**Q: Do I need a Cabify Business account to use this MCP?**
Yes, this MCP server requires a Cabify Empresas (Business) account with API access. Individual consumer accounts do not have API credentials. If your company uses Cabify for corporate transportation, contact your admin to request API access from the Cabify Empresas portal.

**Q: Which cities and countries does Cabify operate in?**
Cabify operates primarily in Spain (Madrid, Barcelona, Valencia, Seville), Portugal (Lisbon, Porto), and Latin America (Mexico, Colombia, Chile, Argentina, Peru, Uruguay, Panama, Costa Rica). Service availability and product types vary by city. Check coverage at cabify.com for your specific location.

**Q: Can this MCP integrate with expense management systems like Concur?**
The Cabify Business API supports integration with expense platforms like SAP Concur. The ride history tool returns structured expense data including cost breakdowns, business categories, and receipts. Your company's Cabify admin can configure Concur sync directly in the Cabify Empresas portal for automated expense reporting.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/cabify](https://vinkius.com/mcp/cabify)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Cabify** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `cabify` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Cabify** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "cabify": {
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
