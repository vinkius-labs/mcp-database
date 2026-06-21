# Amadeus MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/amadeus-alternative)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/amadeus-alternative-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/amadeus-alternative-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [industry-titans](../categories/industry-titans.md)

Manage your travel planning — audit flight offers, hotels, and destinations via AI.

## Description
Empower your AI agent to orchestrate your entire travel planning workflow with **Amadeus**, the global leader in travel technology. By connecting Amadeus to your agent, you transform complex logistics searches into a natural conversation. Your agent can instantly search for flight offers, audit hotel availability, and retrieve points of interest without you ever touching a booking site. Whether you are organizing a business trip or scouting vacation destinations, your agent acts as a real-time travel consultant, ensuring your itineraries are always optimized and data-driven.

### What you can do

- **Flight Auditing** — Search for real-time flight offers between any cities and retrieve detailed pricing and itinerary metadata.
- **Hotel Oversight** — Browse hotel options in specific cities and retrieve detailed offer metadata for any hotel ID.
- **Destination Discovery** — Query points of interest and recommended locations based on geographic coordinates to plan perfect stays.
- **Travel Intelligence** — Retrieve seat maps and direct destination data from any airport to maintain strict control over logistics.
- **Pricing Insights** — Query the cheapest flight dates and destinations from an origin to optimize your travel budget.

### How it works

1. Subscribe to this server
2. Enter your Amadeus API Key and API Secret
3. Start managing your travel intelligence through Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Travel Coordinators** — monitor flight options and hotel availability straight from your workflow.
- **Digital Nomads** — verify cheapest destinations and flight dates without manual searching.
- **Event Planners** — perform rapid audits of points of interest near venues through natural language.
- **Operations Leads** — automate travel logistics querying to orchestrate cross-functional teams smoothly.


## Available Tools
- **get_direct_destinations**: Get direct destinations from an airport
- **get_flight_dates**: Get cheapest flight dates
- **get_flight_destinations**: Get flight destinations from an origin
- **get_hotel_offers**: Get specific offers for a hotel ID
- **get_travel_recommendations**: Get recommended locations based on coordinates
- **get_seat_map**: Get seat map for a flight offer ID
- **search_cities**: Search for cities and locations
- **search_flights**: Search for flight offers
- **search_hotels**: Search for hotels by city code
- **search_poi**: Search for points of interest


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Amadeus** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Search for flights from NYC to LON on 2024-12-01 for 1 adult."

**🤖 AI Agent:**
> I've retrieved 5 flight offers. The cheapest one is a direct flight with British Airways for $550. Would you like the full itinerary or seat map options?

---

**👤 You:**
> "Find hotels in 'MAD' (Madrid)."

**🤖 AI Agent:**
> I've found 10 hotels in Madrid. Top-rated options include 'Westin Palace' and 'Hotel Ritz'. I can provide the specific offer IDs for these hotels if you'd like.

---

**👤 You:**
> "Show points of interest near latitude 48.8584, longitude 2.2945."

**🤖 AI Agent:**
> I've identified several POIs near those coordinates, including the Eiffel Tower and Trocadéro Gardens. Would you like more details or nearby recommendations?


## Installation & Usage

To install and use the **Amadeus** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/amadeus-alternative](https://vinkius.com/mcp/amadeus-alternative)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
