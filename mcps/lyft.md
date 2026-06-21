# Lyft MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/lyft)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/lyft-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/lyft-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [industry-titans](../categories/industry-titans.md)

AI ride management: request rides, estimate costs, and track trips via agents.

## Description
### What you can do

Connect AI agents to the Lyft platform for complete ride automation:

- **Get available ride types** (Lyft, XL, Lux) at any location
- **Estimate ride costs** across all products before booking
- **Compare pickup ETAs** to choose the fastest option
- **Request rides directly** with origin and destination coordinates
- **Track active rides** with driver info, vehicle details, and real-time status
- **Cancel rides** when plans change
- **View complete ride history** with pricing and route data
- **Save favorite locations** (Home, Work, custom places)

### How it works

1. **Connect your Lyft account** via Client ID and Secret from Lyft Developer Portal
2. **Ask your AI agent** to estimate rides, book trips, or check history
3. **No app navigation needed** — natural language commands execute all operations
4. **Automatic OAuth** — the MCP handles token generation using client credentials flow

### Who is this for?

Perfect for **frequent travelers**, **urban commuters**, **executive assistants**, **travel coordinators**, and **corporate teams** managing business transportation. Let AI agents handle ride booking, expense tracking via ride history, and location management. Ideal for professionals taking 10+ Lyft rides monthly who want streamlined booking workflows, instant price comparisons, and automated ride tracking.


## Available Tools
- **cancel_ride**: Cancellation policies vary based on ride status - cancellations after driver assignment may incur fees. Use this to cancel rides that were booked by mistake or are no longer needed.

Cancel an existing Lyft ride request
- **get_cost_estimate**: Prices are in local currency (USD). Use this to compare costs across different Lyft products before booking.

Get cost estimate for a Lyft ride between two locations
- **get_eta_estimate**: Use this to compare how quickly different Lyft services can reach you. Lower minutes mean faster pickups.

Get estimated arrival times for Lyft at a location
- **get_locations**: Returns location IDs, names, addresses, and coordinates. Use this to quickly reference saved locations for ride requests without typing full addresses.

Get saved locations for the Lyft account
- **get_ride_details**: Use this to track your active ride or review past ride details.

Get details of a specific Lyft ride
- **get_ride_history**: Returns ride date, status, origin/destination, ride type, driver, and cost. Use this to review past rides, calculate expenses, or find previous trip details.

Get ride history for the authenticated Lyft account
- **get_ride_types**: ) available at the specified latitude/longitude. Returns ride type IDs, display names, capacity, and descriptions. Use this to see which ride options are available before requesting price or time estimates.

Get available Lyft ride types at a location
- **request_ride**: Requires ride type ID (from get_ride_types), origin coordinates, and destination coordinates. Optionally include pickup/dropoff addresses for clarity. Returns the ride ID and status. Use this to book a ride after confirming price and availability.

Request a new Lyft ride
- **set_location**: Requires location ID, latitude, and longitude. Optionally include a display name. The location ID can be home, work, or any custom string. Returns the saved location details. Use this to manage your favorite pickup/dropoff spots.

Save or update a location for the Lyft account


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Lyft** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Get me a price estimate from JFK Airport to Times Square for a Lyft XL"

**🤖 AI Agent:**
> I'll get cost estimates for all available Lyft products between those locations.

---

**👤 You:**
> "Book me a Lyft from my home to San Francisco International Airport"

**🤖 AI Agent:**
> I'll check available ride types and pricing, then book the ride for you.

---

**👤 You:**
> "Show me my last 20 Lyft rides and total spending"

**🤖 AI Agent:**
> I'll pull your recent ride history and compile the spending summary.


## Installation & Usage

To install and use the **Lyft** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/lyft](https://vinkius.com/mcp/lyft)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
