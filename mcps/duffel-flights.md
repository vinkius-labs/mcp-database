# Duffel Flights MCP Server

Search and book flights via Duffel — list airlines, airports, and manage flight orders directly via AI.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/duffel-flights)

## Overview
**Category:** ecommerce
**Tools Count:** 8

## Description
Connect your AI agent to **Duffel**, the modern infrastructure for travel. This integration allows you to search for real-time flight offers, manage bookings (orders), and access a comprehensive directory of airlines, airports, and aircraft through natural conversation.

### What you can do

- **Flight Search** — Create offer requests to find the best flights based on origin, destination, dates, and cabin class
- **Booking Management** — Create flight orders (instant or hold) and retrieve detailed reservation information
- **Payment Processing** — Pay for flight orders that were previously held directly via the agent
- **Travel Directory** — List and inspect aircraft models, airlines, and airports worldwide with their respective IATA codes
- **Order Oversight** — List all flight bookings associated with your account to track your travel history

### How it works

1. Subscribe to this server
2. Enter your **Duffel Access Token** (obtained from the Duffel Dashboard)
3. Start searching and booking travel directly through natural language

### Who is this for?

- **Travel Agencies** — quickly search for offers and manage client bookings via AI assistance
- **Corporate Travel Managers** — oversee company flight orders and airport metadata
- **Travel Enthusiasts** — research flight options and track reservation statuses without leaving the chat


## Available Tools
- **create_flight_offer_request**: Provide passengers as a JSON array string.

Search for flight offers by specifying origin, destination, and passengers
- **create_flight_order**: Provide full passenger details as a JSON string.

Book a flight by selecting an offer and providing passenger details
- **pay_for_flight_order**: Process payment for a flight order that was previously put on hold
- **list_aircraft**: Retrieve a list of aircraft used by airlines
- **list_airlines**: Retrieve a list of airlines
- **list_airports**: Retrieve a list of airports
- **list_flight_offers**: Retrieve all available flight offers for a specific offer request
- **list_flight_orders**: Retrieve a list of all flight bookings (orders)


## Installation & Usage

To install and use the **Duffel Flights** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/duffel-flights](https://vinkius.com/mcp/duffel-flights)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
