# Parkopedia MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/parkopedia)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/parkopedia-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/parkopedia-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [iot-hardware](../categories/iot-hardware.md)

Global parking search, EV charging, and restrictions data via Parkopedia API.

## Description
Connect **Parkopedia** to any AI agent and access the world's most comprehensive parking data — on-street spots, off-street garages, EV charging stations, and real-time restrictions.

### What you can do
- **Global Search** — Find parking spots in 75+ countries via coordinates or bounding box
- **EV Charging** — Locate chargers, check connector types, and get operator details
- **Restrictions** — View legal parking limits, time restrictions, and resident-only zones
- **Pricing Data** — Access structured pricing from 12,000+ operator feeds
- **Occupancy** — Get real-time availability where supported
- **Amenities** — Find covered parking, restrooms, and valet services nearby
- **Analytics** — Access trends and historical data for location intelligence

### How it works
1. Subscribe to this server
2. Enter your Parkopedia API Key and Base URL
3. Start exploring urban mobility from Claude, Cursor, or any MCP-compatible client

### Who is this for?
- **Navigation Apps** — Integrate real-time parking availability into route planning
- **EV Drivers** — Find compatible chargers and check plug types instantly
- **Fleet Managers** — Optimize parking logistics for delivery and service vehicles


## Available Tools
- **search_amenities**: Search for nearby amenities related to parking
- **get_analytics**: Get parking analytics and trends for a location
- **search_by_bounds**: Search for parking spots within a geographic bounding box
- **get_spot_details**: Get detailed information about a specific parking spot
- **get_ev_charger_details**: Get detailed information about an EV charger
- **search_ev_charging**: Search for EV charging stations near a location
- **get_occupancy**: Get real-time occupancy status for a spot
- **get_pricing**: Get pricing data for a specific spot
- **get_parking_restrictions**: Get parking restrictions for a specific location
- **search_parking**: Search for parking spots near a location


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Parkopedia** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Find EV chargers near Central Park."

**🤖 AI Agent:**
> Found 5 EV chargers within 1km. 1. Tesla Supercharger (500m) — 8 stalls. 2. ChargePoint (800m) — CCS/CHAdeMO. 3. Blink Charging (1.2km) — Level 2.

---

**👤 You:**
> "Are there parking restrictions on 5th Ave right now?"

**🤖 AI Agent:**
> Current restrictions: No parking 4 PM - 7 PM (Rush Hour). Metered parking valid until 6 PM. Residential permit required after 8 PM.

---

**👤 You:**
> "What is the occupancy at the Times Square garage?"

**🤖 AI Agent:**
> Times Square Garage: 42 spaces available out of 500 (8% full). Current rate: $25/hr.


## Installation & Usage

To install and use the **Parkopedia** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/parkopedia](https://vinkius.com/mcp/parkopedia)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
