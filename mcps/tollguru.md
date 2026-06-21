# TollGuru MCP Server

Calculate tolls and trip costs via TollGuru — get toll plaza details, fuel costs, and route optimization for any route across 50+ countries from any AI agent.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/tollguru)

## Overview
**Category:** data-analytics
**Tools Count:** 3

## Description
Connect your **TollGuru** toll calculation API to any AI agent and take full control of trip cost estimation, toll plaza tracking, route optimization, and fleet expense management across 50+ countries through natural conversation.

### What you can do

- **Toll Calculation** — Calculate toll costs for any route with detailed plaza-by-plaza breakdown including tag and cash prices
- **Fuel Cost Estimation** — Get fuel cost estimates based on vehicle efficiency and current fuel prices along the route
- **Driver Cost Analysis** — Calculate driver costs based on hourly wage or time value for complete trip budgeting
- **Multi-Stop Routes** — Calculate tolls for routes with multiple waypoints and optimize waypoint order to minimize tolls
- **Route Optimization** — Find the most cost-effective route between origin and destination with toll-aware routing
- **Polyline Toll Calculation** — Calculate tolls for existing routes from Google Maps, Here Maps, or Mapbox polylines
- **Vehicle-Specific Pricing** — Get accurate toll costs for any vehicle type from 2-axle cars to 9-axle commercial trucks
- **Multi-Currency Support** — View costs in USD, CAD, MXN, EUR, GBP, INR, AUD, and 12+ other currencies
- **Payment Method Breakdown** — Compare toll costs by payment method (tag, cash, prepaid card, license plate)
- **Global Coverage** — Calculate tolls across US, Canada, Mexico, Europe, Australia, India, and 50+ countries

### How it works

1. Subscribe to this server
2. Enter your TollGuru API key (free tier: 150 transactions/day with corporate email)
3. Start calculating toll costs from Claude, Cursor, or any MCP-compatible client

No more manually checking toll authority websites or estimating trip costs. Your AI acts as a dedicated toll analyst and trip budgeting assistant.

### Who is this for?

- **Fleet Managers** — calculate toll costs for delivery routes, optimize waypoint order, and manage trip expenses
- **Road Trippers** — estimate total trip costs including tolls, fuel, and driver time before heading out
- **Logistics Planners** — compare toll costs across route options and select the most cost-effective paths
- **Travel Budgeters** — get comprehensive cost breakdowns for any road trip with toll, fuel, and time costs


## Available Tools
- **calculate_toll_multi_stop**: Returns detailed breakdown of tolls at each plaza along the complete route, fuel costs, and optional driver costs. Supports waypoint optimization to minimize total toll costs. Essential for delivery route planning, multi-stop trip budgeting, and logistics optimization. AI agents should use this when users need toll calculations for routes with multiple stops, such as "calculate tolls from Chicago to Detroit with stops in Toledo and Ann Arbor" or "what are the toll costs for my delivery route with 5 waypoints".

Calculate tolls for a multi-stop route with multiple waypoints
- **calculate_toll_from_polyline**: This is useful when you already have a route from a mapping service and need toll calculations without re-routing. Returns the same detailed toll, fuel, and cost information as the route calculation. Supports all vehicle types, currencies, and payment methods. Essential for integrating with existing mapping applications, post-trip toll reconciliation, and GPS track-based toll analysis. AI agents should use this when users have an existing route polyline from Google Maps, Here Maps, or another service and need toll costs for that specific route.

Calculate tolls for a route defined by an encoded polyline from any mapping service
- **calculate_toll_route**: Returns detailed toll plaza information including plaza names, tag and cash costs, payment methods accepted, and route optimization suggestions. Also calculates fuel costs based on vehicle efficiency and current fuel prices, and optional driver costs based on time value. Supports all vehicle types including 2-axle cars, EVs, motorcycles, and commercial trucks (2-9+ axles). You can request route optimization to minimize toll costs, specify currency output (USD, CAD, MXN, EUR, GBP, INR, AUD, etc.), and choose mapping service (Here Maps, Google Maps, or TollGuru internal). Essential for fleet management, trip cost estimation, route planning, toll reconciliation, and travel budgeting. AI agents should use this when users ask "what are the tolls from New York to Boston", "calculate toll costs for my truck from LA to San Francisco", or need comprehensive trip cost breakdowns including tolls, fuel, and driver time.

Calculate tolls and total trip costs for a route with origin, destination, and optional waypoints


## Installation & Usage

To install and use the **TollGuru** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/tollguru](https://vinkius.com/mcp/tollguru)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
